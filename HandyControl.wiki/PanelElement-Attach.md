An attached property is intended to be used as a type of global property that is settable on any object. 

PanelElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>FluidMoveBehavior</td>
<td>FluidMoveBehavior allows a component to move smoothly between two positions.</td>
</tr>
</table>

|Available Behaviors|
| ---------------- |
| BehaviorXY200 |
| BehaviorX200 |
| BehaviorY200 |
| BehaviorXY400 |
| BehaviorX400 |
| BehaviorY400 |

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<hc:WaterfallPanel hc:PanelElement.FluidMoveBehavior="{StaticResource BehaviorXY200}"/>

```

## Usage in Code-Behind
```
PanelElement.SetFluidMoveBehavior(control, FluidMoveBehavior);
PanelElement.GetFluidMoveBehavior(control);
```
