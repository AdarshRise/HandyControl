There is just the one style in this library for DatePicker , however it does have a attached property for added a ‘clear’ button.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:DatePicker/>
```
you can change calendar ui culture:
```
ConfigHelper.Instance.SetLang("en-us");
```

### Attached Properties
You can use Attached Properties, if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:DatePicker hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True"/>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ShowClearButton                | By activating it you can empty the content.|

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/DataPicker.jpg)