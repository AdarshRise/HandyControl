This just replaces the standard ToggleButton when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <ToggleButton IsChecked="True" Content="Default"/>
```
To use Attached Properties, you should set Style
```
<ToggleButton Content="Default" Style="{StaticResource ToggleButtonPrimary}"/>
```
you can use **IconElement**, **StatusSwitchElement**, **IconSwitchElement** Attached Properties, For more information about **IconElement**, **StatusSwitchElement**, **IconSwitchElement**, see [here](IconElement-Attach), [here](StatusSwitchElement-Attach), [here](IconSwitchElement-Attach)

```
<ToggleButton IsChecked="True" Content="Primary" hc:IconElement.Geometry="{StaticResource ClockGeometry}" Style="{StaticResource ToggleButtonPrimary}"/>
```


| Available styles        |                             |
| ----------------------- | --------------------------- |
| ToggleButtonSuccess     | ToggleButtonIconInfo        |
| ToggleButtonInfo        | ToggleButtonIconWarning     |
| ToggleButtonWarning     | ToggleButtonIconDanger      |
| ToggleButtonDanger      | ToggleButtonIconTransparent |
| ToggleButtonIcon        | ToggleButtonCustom          |
| ToggleButtonIconPrimary | ToggleButtonSwitch          |
| ToggleButtonIconSuccess | ToggleButtonPrimary         |
| ToggleButtonFlip | ToggleButtonDefault [Available Only in Custom Version](https://github.com/ghost1372/HandyControls) |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ToggleButton.png)