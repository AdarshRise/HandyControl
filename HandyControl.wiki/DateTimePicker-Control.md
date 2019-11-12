There is just the two style in this library for DateTimePicker, however it does have a attached property for added a ‘clear’ button.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:DateTimePicker/>
```
you can change calendar ui culture:
```
ConfigHelper.Instance.SetLang("en-us");
```

### Attached Properties
for use Attached Properties, you should set Style<br>

 if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:DateTimePicker hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True"/>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ShowClearButton                | By activating it you can empty the content|
| Style | Set Style |

| Available Styles           |
| ---------------------------- |
| DateTimePickerExtend |
| DateTimePickerPlus    |

| Available Events           |
| ---------------------------- |
| Confirmed |

***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/DateTimePicker.png)