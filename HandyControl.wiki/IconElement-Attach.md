An attached property is intended to be used as a type of global property that is settable on any object. 

IconElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Geometry</td>
<td>Gets or sets the Geometry that describes the shape of this GeometryDrawing.</td>
</tr>
<tr>
<td>Width</td>
<td>Gets or sets the suggested Width of the Geometry.</td>
</tr>
<tr>
<td>Height</td>
<td>Gets or sets the suggested height of the Geometry.</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<Button hc:IconElement.Geometry="{StaticResources Home}" hc:IconElement.Width="120" hc:IconElement.Height="80"/>
```

## Usage in Code-Behind

```
IconElement.SetGeometry(button, Geometry);
IconElement.SetHeight(button, 50);
IconElement.SetWidth(button, 60);

var geo = IconElement.GetGeometry(button);
```
