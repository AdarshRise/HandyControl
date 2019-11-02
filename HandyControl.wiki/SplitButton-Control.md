It allows you to provide a list of items, acting as a button.


# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:SplitButton Content="Test" Command="{Binding SelectCmd}" CommandParameter="Command0">
                <hc:SplitButton.DropDownContent>
                    <StackPanel>
                        <MenuItem Header="Test 2" Command="{Binding SelectCmd}" CommandParameter="Command1"/>
                        <MenuItem Header="Test 3" Command="{Binding SelectCmd}" CommandParameter="Command2"/>
                        <MenuItem Header="Test 4" Command="{Binding SelectCmd}" CommandParameter="Command3"/>
                    </StackPanel>
                </hc:SplitButton.DropDownContent>
            </hc:SplitButton>
```
| **Available Properti**es | **Description**                                             |
| ------------------------ | ----------------------------------------------------------- |
| HitMode | Hover - Click                           |


| Available Styles |
| ------------------ |
| SplitButtonDefault [Available Only in Custom Version](https://github.com/ghost1372/HandyControls) |
| SplitButtonPrimary |
| SplitButtonDanger |
| SplitButtonWarning |
| SplitButtonInfo |
| SplitButtonSuccess |



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/SplitButton.png)