An attached property is intended to be used as a type of global property that is settable on any object. 

EdgeElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>LeftContent</td>
<td>Gets or sets the left content control</td>
</tr>
<tr>
<td>TopContent</td>
<td>Gets or sets the top content control</td>
</tr>
<tr>
<td>RightContent</td>
<td>Gets or sets the right content control</td>
</tr>
<tr>
<td>BottomContent</td>
<td>Gets or sets the bottom content control</td>
</tr>
<tr>
<td>ShowEdgeContent</td>
<td>Gets or sets Visiblity of Edge Content</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<Button hc:EdgeElement.LeftContent="Test" hc:EdgeElement.ShowEdgeContent="True"/>
```

## Usage in Code-Behind

```
BorderElement.SetLeftContent(control, "Test");
BorderElement.SetShowEdgeContent(control, True);

BorderElement.GetLeftContent(control);
```
