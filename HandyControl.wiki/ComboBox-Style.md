This just replaces the standard ComboBox when you drop in the library, nothing fancy to activate it. 

## Usage
```
<ComboBox/>
```
To use Attached Properties, you should set Style
```
<ComboBox Style="{StaticResource ComboBoxExtend}"/>
```
if you want to use watermark or you want to show a message that user must select combobox, you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)

```
<ComboBox hc:InfoElement.Placeholder="Please Select Content}" hc:InfoElement.Title="Groups" Style="{StaticResource ComboBoxExtend}" hc:InfoElement.Necessary="True"/>
```

| Available styles |
| :--------------- |
| ComboBoxExtend   |



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ComboBox.jpg)