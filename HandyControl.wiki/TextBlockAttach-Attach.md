An attached property is intended to be used as a type of global property that is settable on any object. 

TextBlockAttach Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>AutoTooltip</td>
<td>Get or Set Tooltip</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<TextBlock hc:TextBlockAttach.AutoTooltip="True" Width="300" Text="Test" Style="{StaticResource TextBlockDefaultSuccess}"/>
```

## Usage in Code-Behind

```
TextBlockAttach.SetAutoTooltip(control, True);

TextBlockAttach.GetAutoTooltip(control);
```
