# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:WaterfallPanel>
  <TextBlock Text="Content"/>
</hc:WaterfallPanel>
```

### Attached Properties
you can use Attached Properties

if you want to use FluidMoveBehavior, you should use **PanelElement** Attached Property, For more information about **PanelElement**, see [here](PanelElement-Attach)
```
<hc:WaterfallPanel Groups="3" hc:PanelElement.FluidMoveBehavior="{StaticResource BehaviorXY200}">
 <TextBlock Text="Content"/>
<TextBlock Text="Content"/>
<TextBlock Text="Content"/>
<TextBlock Text="Content"/>
</hc:WaterfallPanel>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Groups  | Number of items to be placed in each column (if you set Orientation to Horizontal) or Row (if you set Orientation to Vertical) |
| Orientation  | Specifies the position of the items inside the panel |

| Available Behavior       |
| ---------------------------- |
| BehaviorX200 |
| BehaviorX400 |
| BehaviorY200 |
| BehaviorY400 |
| BehaviorXY200 |
| BehaviorXY400 |
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/WaterfallPanel.png)