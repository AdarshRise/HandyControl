This just replaces the standard MessageBox, nothing fancy to activate it. 

## Usage
```
MessageBox.Ask("Ask Question?");

```
| Available Method |
| :--------------- |
|Show|
| Ask |
| Error |
| Info |
| Fatal |
| Success |
| Warning |

## Override styles
you can override styles like this:
first in your app.xaml add this:
```
 <Style x:Key="MessageBoxCustom" TargetType="hc:MessageBox" BasedOn="{StaticResource {x:Type hc:MessageBox}}">
        <Setter Property="NonClientAreaBackground" Value="#262e2f"/>
        <Setter Property="OtherButtonHoverBackground" Value="#888580"/>
        <Setter Property="OtherButtonForeground" Value="White"/>
        <Setter Property="OtherButtonHoverForeground" Value="White"/>
        <Setter Property="NonClientAreaForeground" Value="White"/>
        <Setter Property="CloseButtonForeground" Value="White"/>
    </Style>
```
now you must set this style in your messagebox:
```
MessageBox.Show(new MessageBoxInfo
            {
                MessageBoxText = "Ask",
                Caption = "Title",
                Button = MessageBoxButton.YesNo,
                IconBrushKey = ResourceToken.AccentBrush,
                IconKey = ResourceToken.AskGeometry,
                Style = ResourceHelper.GetResource<Style>("MessageBoxCustom")
            });
```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/MessageBox.png)