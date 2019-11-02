An attached property is intended to be used as a type of global property that is settable on any object. 

VisualElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>HighlightBrush</td>
<td>Gets or sets </td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
 <Slider hc:VisualElement.HighlightBrush="Red"/>
```

## Usage in Code-Behind
```
VisualElement.SetHighlightBrush(control, Brushes.Red);
VisualElement.GetHighlightBrush(control);
```
