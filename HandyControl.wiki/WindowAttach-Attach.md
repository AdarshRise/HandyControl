An attached property is intended to be used as a type of global property that is settable on any object. 

WindowAttach Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>IsDragElement</td>
<td>Gets or sets Objects Draggable</td>
</tr>
<tr>
<td>IgnoreAltF4</td>
<td>Gets or sets Ability to close Windows with Alt+F4</td>
</tr>
<tr>
<td>ShowInTaskManagerProperty</td>
<td></td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
 <Border hc:WindowAttach.IsDragElement="True"/>
```
and for IgnoreAltF4
```
 hc:WindowAttach.IgnoreAltF4="True"
```

## Usage in Code-Behind

```
WindowAttach.SetIsDragElement(control, True);
WindowAttach.GetIsDragElement(control);
```
