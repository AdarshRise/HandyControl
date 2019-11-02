An attached property is intended to be used as a type of global property that is settable on any object. 

BorderElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>CornerRadius</td>
<td>Gets or sets Rounding the corners of the controls.</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<Button hc:BorderElement.CornerRadius="2"/>
```

## Usage in Code-Behind

```
BorderElement.SetCornerRadius(control, new System.Windows.CornerRadius(2));

BorderElement.GetCornerRadius(control);
```
