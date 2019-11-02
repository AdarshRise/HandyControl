this style contains style for **DataGridCheckBoxColumn**, **DataGridComboBoxColumn**, **DataGridTextColumn**, **DataGridHyperlinkColumn**.
## Usage
```
<DataGrid HeadersVisibility="All" RowHeaderWidth="60">
                    <DataGrid.RowHeaderTemplate>
                        <DataTemplate>
                            <CheckBox IsChecked="False"/>
                        </DataTemplate>
                    </DataGrid.RowHeaderTemplate>
                    <DataGrid.Columns>
                        <DataGridTextColumn/>                       
                        <DataGridCheckBoxColumn Header="Selected"/>
                        <DataGridComboBoxColumn Header="Type"/>
                    </DataGrid.Columns>
                </DataGrid>
```
if you want to generate row numbers you should use **DataGridAttach** Attached Property, For more information about **DataGridAttach**, see [here](DataGridAttach-Attach)

### Usage
First Remove **DataGrid.RowHeaderTemplate**

Then add this Attached Property
```
<DataGrid hc:DataGridAttach.ShowRowNumber="True"/>
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/DataGrid.png)