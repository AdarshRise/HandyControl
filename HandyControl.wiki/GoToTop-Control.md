GoToTop allow you to easily scroll back to the top of your Content with One click of the button.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:ScrollViewer Name="ScrollViewerDemo" IsEnableInertia="True">
            <Border Height="2000" Margin="8,0">
                <Border.Background>
                    <LinearGradientBrush EndPoint="0.5,1" StartPoint="0.5,0">
                        <GradientStop Color="White" Offset="0"/>
                        <GradientStop Color="Black" Offset="1"/>
                    </LinearGradientBrush>
                </Border.Background>
            </Border>
        </hc:ScrollViewer>
        <hc:GotoTop Animated="True" AutoHiding="True" AnimationTime="500" Target="{Binding ElementName=ScrollViewerDemo}" HorizontalAlignment="Right" VerticalAlignment="Bottom" Margin="0,0,20,20"/>

```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Animated        | Scroll to top with animation     |
| AnimationTime | animation time for scroll        |
| AutoHiding | Auto hide Button when focus lost |
| Target | bind to control |

***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/GoToTop.gif)