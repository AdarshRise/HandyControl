The TabControl represents a TabControl that offers a different navigation style than the standard TabControl to reach the extra tabs.

# Usage
First add HandyControl refrence
```
xmlns:controls="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:TabControl>
                    <hc:TabItem Header="TabItem1">
                        <Grid Background="White"/>
                    </hc:TabItem>
                    <hc:TabItem Header="TabItem2">
                        <Grid Background="{DynamicResource DarkDangerBrush}"/>
                    </hc:TabItem>
                    <hc:TabItem Header="TabItem3" IsSelected="True">
                        <Grid Background="{DynamicResource PrimaryBrush}"/>
                    </hc:TabItem>
                </hc:TabControl>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| IsEnableTabFill  | By Using it you can fit the tab in the entire content |
| ShowCloseButton  | By Using this property, tabs have the ability to close |
| IsDraggable  | With this property, you can drag and drop tabs with the mouse |
| IsEnableAnimation  | With this property, you can enable or disable animation when Displaying tab content, opening and closing tabs |
| IsScrollable  | With this property, you can enable or disable scrollable tabs |
| ShowOverflowButton  | show tabs in a list |
| ShowScrollButton  | show or hide scroll button |
| ShowContextMenu | show or hide Context Menu |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/TabControl.gif)