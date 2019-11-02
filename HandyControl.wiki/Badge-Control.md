Badge Control Renders a badge overlay on a control.


# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Badge Value="100">
 <Button Content="Comment"/>
</hc:Badge>
```
| **Available Properti**es | **Description**                                             |
| ------------------------ | ----------------------------------------------------------- |
| Value                    | Defines badge status in int value                           |
| Text                     | Defines badge status in string value                        |
| BadgeMargin              | Specifies the badge margin in control                       |
| Status                   | you can set Status as **Dot** or **Processing** or **Text** |
| Style                    | To use Brushes, you should set Style                        |

| Available Styles |
| ------------------ |
| BadgeSuccess       |
| BadgeInfo          |
| BadgeWarning       |
| BadgeDanger        |
| BadgePrimary       |



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Badge.png)