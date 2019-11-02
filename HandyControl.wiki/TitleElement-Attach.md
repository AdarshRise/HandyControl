An attached property is intended to be used as a type of global property that is settable on any object. 

TitleElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Title</td>
<td>Gets or sets Controls Title</td>
</tr>
<tr>
<td>Background</td>
<td>Gets or sets Title Background color</td>
</tr>
<tr>
<td>Foreground</td>
<td>Gets or sets Title Foreground color</td>
</tr>
<tr>
<td>BorderBrush</td>
<td>Gets or sets Title BorderBrush</td>
</tr>
<tr>
<td>TitleAlignment</td>
<td>Gets or sets Title Alignment</td>
</tr>
<tr>
<td>TitleWidth</td>
<td>Gets or sets Title Width</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<hc:NumericUpDown Style="{StaticResource NumericUpDownExtend}" hc:TitleElement.Title="Groups" hc:TitleElement.TitleWidth="50" hc:TitleElement.TitleAlignment="Left"/>

```

## Usage in Code-Behind

```
TitleElement.SetTitle(control, "Groups");
TitleElement.SetTitleWidth(control, 50);
TitleElement.SetTitleAlignment(control, HandyControl.Data.TitleAlignment.Left);
TitleElement.GetTitle(control);
```
