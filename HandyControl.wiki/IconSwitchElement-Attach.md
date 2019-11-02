An attached property is intended to be used as a type of global property that is settable on any object. 

IconSwitchElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>GeometrySelected</td>
<td>Gets or sets the Geometry that describes the shape of this GeometryDrawing.</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<ToggleButton hc:IconSwitchElement.GeometrySelected="{StaticResources Home}"/>
```

## Usage in Code-Behind

```
IconSwitchElement.SetGeometrySelected(control, Geometry);

var geo = IconSwitchElement.GetGeometrySelected(control);
```
