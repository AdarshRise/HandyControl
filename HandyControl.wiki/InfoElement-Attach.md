An attached property is intended to be used as a type of global property that is settable on any object. 

InfoElement Contains 

| Property | Description |
| -------- | ------- |
| Placeholder | Gets or sets text that appears in the textbox before the user has focused or entered any text. |
| Necessary | Gets or sets Displays an error message that reminds you to enter the entry |
| Symbol | Gets or sets The sign that will be displayed for mandatory input filling |
| ContentHeight | Gets or sets height of the box |
| MinContentHeight | Gets or sets Minimum Height of the Content |
| MaxContentHeight | Gets or sets Maximum Height of the Content |

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
