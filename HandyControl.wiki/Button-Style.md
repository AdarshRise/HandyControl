This just replaces the standard button when you drop in the library, nothing fancy to activate it. 

## Usage
```
<Button Content="Default"/>
```
To use brushes, you should set Style
```
<Button Content="ButtonPrimary" Style="{StaticResource ButtonPrimary}"/>
```
if you want to use image inside button you should use **IconElement** Attached Property, For more information about **IconElement**, see [here](IconElement-Attach)

```
<Button hc:IconElement.Geometry="{StaticResource DeleteGeometry}"/>
```
| Available styles |
| ---------------- |
| ButtonDefault [Available Only in Custom Version](https://github.com/ghost1372/HandyControls) |
| ButtonPrimary    |
| ButtonSuccess    |
| ButtonInfo       |
| ButtonWarning    |
| ButtonDanger     |
| ButtonIcon       |
| ButtonCustom     |


***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Button.png)