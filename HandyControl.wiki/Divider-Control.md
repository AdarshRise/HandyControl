A Divider control draws a line, horizontal or vertical, between items in controls


# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Divider/>
```
or
```
 <StackPanel Orientation="Horizontal" Margin="0,16,0,0">
                    <Button Content="Button"/>
                    <hc:Divider LineStrokeThickness="2" Orientation="Vertical" MaxHeight="16"/>
                    <Button Content="Button"/>
                    <hc:Divider LineStrokeThickness="2" Orientation="Vertical" MaxHeight="16"/>
                    <Button Content="Button"/>
                </StackPanel>
```
| **Available Properti**es |
| ------------------------ | 
| Content                    | 
| Padding                     | 
| LineStrokeThickness              | 
| LineStroke                   | 
| LineStrokeDashArray                    | 
| HorizontalContentAlignment |
| Orientation |




***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Divider.png)