An attached property is intended to be used as a type of global property that is settable on any object. 

BackgroundSwitchElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>MouseHoverBackground</td>
<td>Gets or sets the background color of the Controls.</td>
</tr>
<tr>
<td>MouseDownBackground</td>
<td>Gets or sets the background color of the Controls.</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<Button hc:BackgroundSwitchElement.MouseHoverBackground="Red"/>
```

## Usage in Code-Behind
```
BackgroundSwitchElement.SetMouseHoverBackground(control, Brushes.Red);
BackgroundSwitchElement.SetMouseDownBackground(control, Brushes.Red);

BackgroundSwitchElement.GetMouseHoverBackground(control);
BackgroundSwitchElement.GetMouseDownBackground(control);
```
