This just replaces the standard RadioButton when you drop in the library, nothing fancy to activate it. 

## Usage
```
<StackPanel>
                    <RadioButton Content="RadioButton"/>
                    <RadioButton Content="RadioButton2" IsChecked="True"/>
                    <RadioButton Content="RadioButton3"/>
                    <RadioButton Content="RadioButton4"/>
</StackPanel>
```
if you want to use image inside RadioButton you should use **IconElement** Attached Property, For more information about **IconElement**, see [here](IconElement-Attach) also you should set Style to ```RadioButtonIcon```

```
 <UniformGrid Rows="2" Columns="2">
                    <RadioButton Background="{DynamicResource SecondaryRegionBrush}" hc:IconElement.Geometry="{StaticResource CalendarGeometry}" Style="{StaticResource RadioButtonIcon}" Content="RadioButton"/>
                    <RadioButton Background="{DynamicResource SecondaryRegionBrush}" Style="{StaticResource RadioButtonIcon}" Content="RadioButton2" IsChecked="True"/>
                    <RadioButton BorderThickness="1" hc:IconElement.Geometry="{StaticResource CalendarGeometry}" Style="{StaticResource RadioButtonIcon}" Content="RadioButton3"/>
                    <RadioButton BorderThickness="1" Style="{StaticResource RadioButtonIcon}" Content="RadioButton4"/>
                </UniformGrid>
```
also there is 2 more style for RadioButton just follow this:
```
<controls:RadioGroup>
                <RadioButton Content="RadioButton" IsChecked="True"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
            </controls:RadioGroup>
```
### RadioGroupSolid
```
            <controls:RadioGroup Style="{StaticResource RadioGroupSolid}">
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton" IsChecked="True"/>
            </controls:RadioGroup>
```
this styles also have horizontal and vertical capabilities just set Orientation

```
<controls:RadioGroup Style="{StaticResource RadioGroupSolid}" Orientation=""Vertical">
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton"/>
                <RadioButton Content="RadioButton" IsChecked="True"/>
            </controls:RadioGroup>
```

| Available styles |
| ---------------- |
| RadioButtonIcon  |
| RadioGroupSolid  |

***


![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/RadioButton.png)