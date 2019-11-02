This just replaces the standard TextBox when you drop in the library, nothing fancy to activate it. 

## Usage
```
<TextBox Text="Content"/>
```
To use Attached Properties, you should set Style
```
<TextBox Style="{StaticResource TextBoxExtend}" Text="Content"/>
```
if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)

```
<TextBox hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content}" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True" Style="{StaticResource TextBoxExtend}"/>

```
| Available styles |
| ---------------- |
|TextBoxExtend|


***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/TextBox.jpg)