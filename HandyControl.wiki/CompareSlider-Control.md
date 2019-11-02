With CompareSlider control, you can compare 2 objects.

CompareSlider control consists of 2 parts
### * SourceContent
### * TargetContent

In each of these content, we must specify the object.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:CompareSlider>
                    <hc:CompareSlider.TargetContent>
                        <Button Content="HandyControl" Style="{StaticResource ButtonWarning}" Width="140"/>
                    </hc:CompareSlider.TargetContent>
                    <hc:CompareSlider.SourceContent>
                        <Button Content="Github" Style="{StaticResource ButtonSuccess}" Width="140"/>
                    </hc:CompareSlider.SourceContent>
                </hc:CompareSlider>
```
| **Available Properti**es | **Description**                            |
| ------------------------ | ------------------------------------------ |
| Value             | Use this option to move the comparison location                        |
| Orientation          | By using this property, you can use it horizontally or vertically |

***
![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/CompareSlider-h.gif)
![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/CompareSlider-v.gif)