# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
 <Button hc:IconElement.Geometry="{StaticResource ThumbsUpGeometry}" Width="180">
                <hc:FloatingBlock.ContentTemplate>
                    <DataTemplate>
                        <Path Data="{StaticResource ThumbsUpGeometry}" Fill="{DynamicResource DangerBrush}" Width="16" Height="16"/>
                    </DataTemplate>
                </hc:FloatingBlock.ContentTemplate>
            </Button>
```
OR
```
<Button hc:IconElement.Geometry="{StaticResource ThumbsUpGeometry}" Width="180" Margin="0,10,0,0" hc:FloatingBlock.Duration="0:0:1" hc:FloatingBlock.VerticalOffset="-20" hc:FloatingBlock.ToX="50" hc:FloatingBlock.ToY="-80">
                <hc:FloatingBlock.ContentTemplate>
                    <DataTemplate>
                        <Path Data="{StaticResource ThumbsUpGeometry}" Fill="{DynamicResource DangerBrush}" Width="16" Height="16"/>
                    </DataTemplate>
                </hc:FloatingBlock.ContentTemplate>
            </Button>
```
| **Available Properti**es |
| ------------------------ |
| Content |
| Duration |
| VerticalOffset |
| ToX |
| ToY |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/FloatingBlock.gif)