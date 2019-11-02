you can use UpdateHelper for checking application updates

| Available Methods | Description |
|------------------ | ----------- |
| CheckForUpdate | Use an uploaded xml file on the web to check if the update is available |
| CheckForUpdateGithubRelease | Use the GitHab Release Page to check if the update is available |


## CheckForUpdate 

first you must create xml file like this:
```
<?xml version="1.0" encoding="utf-8"?>
  <AppVersion>
    <version>2.5.100.0</version>
    <url>https://github.com/ghost1372/HandyControls/releases</url>
    <changelog>
    Added UpdateHelper
    </changelog>
  </AppVersion>
```
then you must upload this file to github or any host that support raw view. example for [github](https://raw.githubusercontent.com/ghost1372/HandyControls/develop/Updater.xml)

Whenever your program is updated, just modify this file

now we can check for update
```
var ver = UpdateHelper.CheckForUpdate("https://raw.githubusercontent.com/ghost1372/HandyControls/develop/Updater.xml");
            if(ver.IsExistNewVersion)
            {
                Growl.InfoGlobal("New Version Found!");
                lblUrl.Content = ver.URL;
                txtChangelog.Text = ver.ChangeLog;
            }
            else
            {
                Growl.ErrorGlobal("you are using latest version");
            }
```

## CheckForUpdateGithubRelease 

first you must create a new release tag in [github repository](https://github.com/ghost1372/HandyControls/releases/new):

_**note: tag version must be in this format : 1.0.0.0**_

now we can check for update with github username and github repository
```
var ver = UpdateHelper.CheckForUpdateGithubRelease("ghost1372", "MoalemYar");
            if(ver.IsExistNewVersion)
            {
                Growl.InfoGlobal("New Version Found!");
                    lblUrl2.Text = ver.Url;
                    lbl1.Text = ver.CreatedAt.ToString();
                    lbl2.Text = ver.PublishedAt.ToString();
                    
                    //Asset is List so maybe there is more than one file you can use forech or increase index
                    lbl3.Text = ver.Asset[0].browser_download_url;
                    lbl4.Text = ver.IsPreRelease.ToString();
                    lbl5.Text = ver.Asset[0].size.ToString();
                    lbl6.Text = ver.Version;
                    txtChangelog2.Text = ver.Changelog;
            }
            else
            {
                Growl.ErrorGlobal("you are using latest version");
            }
```
