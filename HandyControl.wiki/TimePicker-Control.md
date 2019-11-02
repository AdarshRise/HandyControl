TimePicker is a convenient way to get rid of boring time parsing and data validation. TimePicker is easy and simple, but yet essential way to improve end-user experience.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:TimePicker/>
```
## ListClock
you can use another design for clock like list
```
<hc:TimePicker Style="{StaticResource TimePickerPlus}">
    <hc:TimePicker.Clock>
        <hc:ListClock/>
    </hc:TimePicker.Clock>
</hc:TimePicker>
```

### Attached Properties
for use Attached Properties, you should set Style

 if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:TimePicker hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True"/>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ShowClearButton  | By activating it you can empty the content |


| Available Styles           |
| ---------------------------- |
| TimePickerExtend |
| TimePickerPlus |

***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/TimePicker.jpg)