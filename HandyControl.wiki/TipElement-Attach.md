An attached property is intended to be used as a type of global property that is settable on any object. 

TipElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Visibility</td>
<td>Gets or sets Visibility of Tip</td>
</tr>
<tr>
<td>Placement</td>
<td>Gets or sets Tip Alignment</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
 <Slider hc:TipElement.Visibility="Visible"/>
```

## Usage in Code-Behind
```
TipElement.SetVisibility(control, System.Windows.Visibility.Collapsed);
TipElement.SetPlacement(control, HandyControl.Data.TipPlacement.BottomRight);
TipElement.GetVisibility(control);
```
