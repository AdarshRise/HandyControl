An attached property is intended to be used as a type of global property that is settable on any object. 

InfoElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Placeholder</td>
<td>Gets or sets text that appears in the textbox before the user has focused or entered any text.</td>
</tr>
<tr>
<td>Necessary</td>
<td>Gets or sets Displays an error message that reminds you to enter the entry</td>
</tr>
<tr>
<td>Symbol</td>
<td>Gets or sets The sign that will be displayed for mandatory input filling</td>
</tr>
<tr>
<td>ContentHeight</td>
<td>Gets or sets height of the box</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<ComboBox hc:InfoElement.Placeholder="Select Item" hc:InfoElement.Necessary="True" hc:InfoElement.Symbol="*" hc:InfoElement.ContentHeight="35"/>
```

## Usage in Code-Behind
```
InfoElement.SetPlaceholder(control, "Select Item");
InfoElement.SetNecessary(control, True);
InfoElement.SetSymbol(control, "*");
InfoElement.ContentHeight(control, 35);

InfoElement.GetPlaceholder(control);
...
```
