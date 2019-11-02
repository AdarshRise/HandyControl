An attached property is intended to be used as a type of global property that is settable on any object. 

DataGridAttach Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>TextColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the TextColumn Style.</td>
</tr>
<tr>
<td>EditingTextColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the EditingTextColumn Style.</td>
</tr>
<tr>
<td>ComboBoxColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the ComboBoxColumn Style.</td>
</tr>
<tr>
<td>EditingComboBoxColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the EditingComboBoxColumn Style.</td>
</tr>
<tr>
<td>CheckBoxColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the CheckBoxColumn Style.</td>
</tr>
<tr>
<td>EditingCheckBoxColumnStyle</td>
<td>Gets or sets a Style object representing the style to use for the EditingCheckBoxColumn Style.</td>
</tr>
<tr>
<td>ShowRowNumber</td>
<td>Gets or sets a value indicating whether the Row Numbers should be shown.</td>
</tr>
<tr>
<td>ApplyDefaultStyle</td>
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
<DataGrid hc:DataGridAttach.ShowRowNumber="True"/>
```

## Usage in Code-Behind
```
DataGridAttach.SetShowRowNumber(datagrid, true);

DataGridAttach.GetShowRowNumber(datagrid);
```
