This just replaces the standard DatePicker when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <DatePicker/>
```
you can change calendar ui culture:
```
ConfigHelper.Instance.SetLang("en-us");
```
To use Attached Properties, you should set Style
```
<DatePicker Style="{StaticResource DatePickerExtend}"/>
```
you can use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)

```
<DatePicker Style="{StaticResource DatePickerExtend}" hc:InfoElement.Title="Select Date"/>
```

| Available styles |
| :--------------- |
| DatePickerExtend   |



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/DataPicker.jpg)