Follow these steps to use the HandyControl in your application.

## Easy Way
just download and install handycontrol template from marketplace.
in this way you dont need to add anything after installing hc, create new project with handycontrol template

![HandyControl-VSIX](https://github.com/ghost1372/HandyControls/blob/develop/Resources/vsixTemplate.png)

| [HandyControl](https://marketplace.visualstudio.com/items?itemName=HandyOrg.handycontrolforvs2019) | [HandyControls (Custom Version)](https://marketplace.visualstudio.com/items?itemName=MahdiHosseini.HandyControls) |
| ------------- | --------- |



## Install HandyControl from Nuget
[Install-Package HandyControl](https://www.nuget.org/packages/HandyControl)
```
Install-Package HandyControl
```
or you can use custom version based on handycontrol

[Install-Package HandyControls](https://www.nuget.org/packages/HandyControls)
```
Install-Package HandyControls
```
### Add code in App.xaml as follows
```XML
<Application.Resources>
    <ResourceDictionary>
        <ResourceDictionary.MergedDictionaries>
            <ResourceDictionary Source="pack://application:,,,/HandyControl;component/Themes/SkinDefault.xaml"/>
            <ResourceDictionary Source="pack://application:,,,/HandyControl;component/Themes/Theme.xaml"/>
        </ResourceDictionary.MergedDictionaries>
    </ResourceDictionary>
</Application.Resources>
```

### Change Window to BlurWindow and set Style to WindowBlur in your main window
```XML
<hc:BlurWindow x:Class="WpfApplication.MainWindow"
                      xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
                      xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
                      xmlns:hc="https://handyorg.github.io/handycontrol"
                      Title="MainWindow"
                      Style="{StaticResource WindowBlur}"
                      Height="600"
                      Width="800">
  <Grid>

    <!-- your content -->

  </Grid>
</hc:BlurWindow>
```

```csharp
namespace WpfApplication
{
  public partial class MainWindow
  {
    public MainWindow()
    {
      InitializeComponent();
    }
  }
}
```
