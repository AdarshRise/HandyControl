An attached property is intended to be used as a type of global property that is settable on any object. 

StatusSwitchElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>CheckedElement</td>
<td>Gets or sets </td>
</tr>
<tr>
<td>HideUncheckedElement</td>
<td>Gets or sets </td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
 <ToggleButton IsChecked="True" Style="{StaticResource ToggleButtonCustom}" hc:StatusSwitchElement.HideUncheckedElement="True">
                            <hc:StatusSwitchElement.CheckedElement>
                                <Border>
                                    <Ellipse Fill="{DynamicResource PrimaryBrush}" StrokeThickness="1" Stroke="{DynamicResource BorderBrush}"/>
                                </Border>
                            </hc:StatusSwitchElement.CheckedElement>
                            <Border>
                                <Ellipse Fill="{DynamicResource BorderBrush}" StrokeThickness="1" Stroke="{DynamicResource BorderBrush}"/>
                            </Border>
                        </ToggleButton>
```

## Usage in Code-Behind
```
StatusSwitchElement.SetHideUncheckedElement(control, True);
StatusSwitchElement.GetHideUncheckedElement(control);
```
