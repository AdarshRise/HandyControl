# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:PreviewSlider Value="500" Maximum="1000"/>
```
if you want to show value, you should use **PreviewContent** like this
```
<hc:PreviewSlider Name="PreviewSlider" Value="500" Maximum="1000">
            <hc:PreviewSlider.PreviewContent>
                <Label Style="{StaticResource LabelPrimary}" Content="{Binding PreviewPosition,ElementName=PreviewSlider}" ContentStringFormat="{}{0:#0.0}"/>
            </hc:PreviewSlider.PreviewContent>
        </hc:PreviewSlider>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Value  | slider value |
| Maximum | maximum value |

***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/PreviewSlider.gif)