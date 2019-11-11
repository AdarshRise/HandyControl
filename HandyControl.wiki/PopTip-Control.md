The Popup control provides a way to display content in a separate window that floats over the current application window relative to a designated element or screen coordinate. This topic introduces the Popup control and provides information about its use.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<Button Margin="8,0" Tag="0" Style="{StaticResource Button4PoptipStyle}">
  <hc:Poptip.Instance>
     <hc:Poptip Content="Text" Placement="TopLeft"/>
 </hc:Poptip.Instance>
</Button>
```
or
```
<Button Margin="8,0" Tag="1" Style="{StaticResource Button4PoptipStyle}">
 <hc:Poptip.Instance>
   <hc:Poptip Placement="Top">
        <hc:Poptip.Content>
          <Path Width="100" Height="100" Fill="#f06632" Data="{StaticResource LogoGeometry}"/>
        </hc:Poptip.Content>
   </hc:Poptip>
  </hc:Poptip.Instance>
</Button>
```
or
```
<Button hc:Poptip.Content="Text" hc:Poptip.Placement="TopRight" Margin="8,0" Tag="2" Style="{StaticResource Button4PoptipStyle}"/>
```
or
```
 <ToggleButton hc:Poptip.HitMode="None" hc:Poptip.IsOpen="True" hc:Poptip.Content="Text" hc:Poptip.Placement="RightTop" Margin="8,16" Tag="3" Style="{StaticResource ToggleButton4PoptipStyle}"/>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| HitMode | Includes Click, Hover, Focus, None|
| IsInstance |  |
| Content |   |
| ContentTemplate |   |
| ContentStringFormat |  |
| ContentTemplateSelector |  |
| Offset | |
| Placement | Includes LeftTop, Left, LeftBottom, TopLeft, Top, TopRight, RightTop, Right, RightBottom, BottomLeft, Bottom, BottomRight |
| IsOpen | |
| Target | |
| Instance | |
