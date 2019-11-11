RelativePanel is a layout container that is useful for creating UI that do not have a clear linear pattern; that is, layouts that are not fundamentally stacked, wrapped, or tabular, where you might naturally use a StackPanel or Grid. 
If your UI consists of multiple nested panels, RelativePanel is a good option to consider.
[[Layout Source](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.controls.relativepanel#remarks)]

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml

```
 <hc:RelativePanel>
  <Rectangle x:Name="RedRect" Fill="{DynamicResource DangerBrush}" MinHeight="100" MinWidth="100" />
    <Rectangle x:Name="BlueRect" Fill="{DynamicResource PrimaryBrush}" MinHeight="100" MinWidth="100"
                       hc:RelativePanel.RightOf="RedRect" />
    <Rectangle x:Name="GreenRect" Fill="{DynamicResource SuccessBrush}" MinHeight="100" Margin="0,5,0,0"
                       hc:RelativePanel.Below="RedRect" hc:RelativePanel.AlignLeftWith="RedRect"
                       hc:RelativePanel.AlignRightWith="BlueRect" />
    <Rectangle Fill="Yellow" MinHeight="100" hc:RelativePanel.Below="GreenRect" hc:RelativePanel.AlignLeftWith="BlueRect"
                       hc:RelativePanel.AlignRightWithPanel="True" />
 </hc:RelativePanel>
```
or another sample
```
 <hc:RelativePanel>
   <Rectangle x:Name="RedRect2" Fill="{DynamicResource DangerBrush}" Width="44" Height="44" />
   <Rectangle x:Name="BlueRect2" Fill="{DynamicResource PrimaryBrush}" Width="88" Height="44"
              hc:RelativePanel.RightOf="RedRect2" />
   <Rectangle x:Name="GreenRect2" Fill="{DynamicResource SuccessBrush}" Height="44" hc:RelativePanel.Below="RedRect2"
              hc:RelativePanel.AlignLeftWith="RedRect2" hc:RelativePanel.AlignRightWith="BlueRect2" />
   <Rectangle Fill="{DynamicResource WarningBrush}" hc:RelativePanel.Below="GreenRect2" 
              hc:RelativePanel.AlignLeftWith="BlueRect2" hc:RelativePanel.AlignRightWithPanel="True"
              hc:RelativePanel.AlignBottomWithPanel="True" />
 </hc:RelativePanel>
```
or another one
```
<hc:RelativePanel>
  <Rectangle x:Name="Red" Fill="{DynamicResource DangerBrush}" Width="50" Height="50"
    hc:RelativePanel.AlignHorizontalCenterWithPanel="True" hc:RelativePanel.AlignVerticalCenterWithPanel="True"/>
  <Rectangle x:Name="Green" Fill="{DynamicResource SuccessBrush}" Width="50" Height="50"
            hc:RelativePanel.Above="Red" hc:RelativePanel.AlignLeftWith="Red"/>
  <Rectangle x:Name="Yellow" Fill="Yellow" Width="50" Height="50" hc:RelativePanel.Below="Red"
            hc:RelativePanel.AlignLeftWith="Red"/>
  <Rectangle x:Name="Blue" Fill="{DynamicResource PrimaryBrush}" Width="50" Height="50"
            hc:RelativePanel.LeftOf="Red" hc:RelativePanel.AlignBottomWith="Red"/>
  <Rectangle x:Name="Olive" Fill="Olive" Width="50" Height="50" hc:RelativePanel.RightOf="Red"
            hc:RelativePanel.AlignBottomWith="Red"/>
  <Rectangle x:Name="Orchid" Fill="Orchid" Width="50" Height="50" hc:RelativePanel.Above="Green"
            hc:RelativePanel.LeftOf="Green"/>
  <Rectangle x:Name="Orange" Fill="{DynamicResource WarningBrush}" Width="50" Height="50" hc:RelativePanel.Below="Olive"
            hc:RelativePanel.RightOf="Olive"/>
  <Rectangle x:Name="Black" Fill="Black" Width="50" Height="50" hc:RelativePanel.AlignTopWithPanel="True"/>
  <Rectangle x:Name="DodgerBlue" Fill="{DynamicResource InfoBrush}" Width="50" Height="50" 
            hc:RelativePanel.AlignTopWithPanel="True" hc:RelativePanel.AlignRightWithPanel="True"/>
  <Rectangle x:Name="SeaGreen" Fill="SeaGreen" Width="50" Height="50" hc:RelativePanel.AlignBottomWithPanel="True"
            hc:RelativePanel.AlignLeftWithPanel="True"/>
  <Rectangle x:Name="Navy" Fill="Navy" Width="50" Height="50" hc:RelativePanel.AlignBottomWithPanel="True"
            hc:RelativePanel.AlignRightWithPanel="True"/>
 </hc:RelativePanel>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| AlignLeftWithPanel | Gets or sets a value that indicates whether this element’s left edge is touching the panel’s left edge.            |
| AlignTopWithPanel | Gets or sets a value that indicates whether this element’s top edge is touching the panel’s top edge.           |
| AlignRightWithPanel | Gets or sets a value that indicates whether this element’s right edge is touching the panel’s right edge.                  |
| AlignBottomWithPanel | Gets or sets a value that indicates whether this element’s bottom edge is touching the panel’s bottom edge.    |
| AlignLeftWith | Gets or sets a target element that this element's left edge is aligned with. |
| AlignTopWith | Gets or sets a target element that this element's top edge is aligned with. |
| AlignRightWith | Gets or sets a target element that this element's right edge is aligned with. |
| AlignBottomWith | Gets or sets a target element that this element's bottom edge is aligned with. |
| LeftOf | Gets or sets a target element that this element is positioned to the left of. |
| Above | Gets or sets a target element that this element is positioned above. |
| RightOf | Gets or sets a target element that this element is positioned to the right of. |
| Below | Gets or sets a target element that this element is positioned below. |
| AlignHorizontalCenterWithPanel | Gets or sets a value that indicates whether this element’s horizontal axis is touching the panel’s horizontal axis. |
| AlignHorizontalCenterWith | Gets or sets a target element that this element's horizontal center is aligned with. |
| AlignVerticalCenterWithPanel | Gets or sets a value that indicates whether this element’s vertical axis is touching the panel’s horizontal axis. |
| AlignVerticalCenterWith | Gets or sets a target element that this element's vertical center is aligned with. |


***
![relativepanel](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.controls/images/controls/relativepanelbasic.png)