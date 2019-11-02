Rate is a flexible UI component that allows users to intuitively rate by selecting number of items [stars] from a predefined number of items.
# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Rate Value="2"/>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Count  | By setting a value you can easily choose number of items the user can rate from |
| DefaultValue | Sets the default value |
| AllowHalf | You can give it a half score by enabling it |
| AllowClear | By Using it, the rating can not be changed |
| Icon | You can change the default Icon by this Property, Be careful that you should use geometric images |
| ShowText | Displays the score of the selected item |
| Foreground | You can change the brush color of the image |

| **Available Event** | 
| -- |
| ValueChanged |
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Rate.png)