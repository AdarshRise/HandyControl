

| Available Window Control        |  Style needed |
| ----------------------- | --------------------------- |
| BlurWindow     | WindowBlur        |
| Window     |     WindowWin10     |

## Window
```
<hc:Window 
  Style={StaticResources WindowWin10}
...
```
## BlurWindow
```
<hc:BlurWindow 
  Style={StaticResources WindowBlur}
...
```
Create a function in your App.cs file like this:
```
using HandyControl.Data;
public static SystemVersionInfo GetSystemVersionInfo()
        {
            var managementClass = new ManagementClass("Win32_OperatingSystem");
            var instances = managementClass.GetInstances();
            foreach (var instance in instances)
            {
                if (instance["Version"] is string version)
                {
                    var nums = version.Split('.').Select(int.Parse).ToList();
                    var info = new SystemVersionInfo(nums[0], nums[1], nums[2]);
                    return info;
                }
            }
            return default(SystemVersionInfo);
        }
```
now in your app.cs file and OnStartup func add this line:
```
ConfigHelper.Instance.SetSystemVersionInfo(GetSystemVersionInfo());
```
then in your window make sure your Controls background is **Transparent**

```Background="Transparent"```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/BlurWindow.png)

***

# Dark & Light & Violet Mode
there is 3 accent color that you can use in your application. for start you must create a function

```
internal void UpdateSkin(SkinType skin)
        {
             Resources.MergedDictionaries.Clear();
            Resources.MergedDictionaries.Add(new ResourceDictionary
            {
                Source = new Uri($"pack://application:,,,/HandyControl;component/Themes/Skin{skin.ToString()}.xaml")
            });
            Resources.MergedDictionaries.Add(new ResourceDictionary
            {
                Source = new Uri("pack://application:,,,/HandyControl;component/Themes/Theme.xaml")
            });
        }
```

now you can change your accent color from every where Do that in this way:

### Light Mode
```UpdateSkin(SkinType.Default);```

### Dark Mode
```UpdateSkin(SkinType.Dark);```

### Violet Mode
```UpdateSkin(SkinType.Violet);```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/DarkTheme.png)