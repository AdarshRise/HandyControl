The NumericUpDown control is used to increase or decrease a numeric value.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:NumericUpDown/>
```


### Attached Properties
To use Attached Properties, you should set Style

if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:NumericUpDown hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" Style="{StaticResource NumericUpDownPlus}" hc:InfoElement.Necessary="True"/>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Minimum  | By specifying a value for Minimum you can set the range for legal values. |
| Maximum | By specifying a value for Maximum you can set the range for legal values. |
| ShowClearButton | By activating it you can empty the content |
| DecimalPlaces | You can specify the number of decimal places |
| Style | Set Style |

| Available Styles           |
| ---------------------------- |
| NumericUpDownPlus |
| NumericUpDownExtend    |



***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/NumericUpDown.png)