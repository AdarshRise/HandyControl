This just replaces the standard ProgressBar when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <ProgressBar Value="20"/>
```
To use brushes, you should set Style
```
<ProgressBar Value="20" Style="{StaticResource ProgressBarSuccess}"/>
```
| Available styles         |                          |
| ------------------------ | ------------------------ |
| ProgressBarSuccess       | ProgressBarSuccessStripe |
| ProgressBarInfo          | ProgressBarInfoStripe    |
| ProgressBarWarning       | ProgressBarWarningStripe |
| ProgressBarDanger        | ProgressBarDangerStripe  |
| ProgressBarPrimaryStripe | ProgressBarFlat          |

***

## How  to edit the color

*short-method*

```
<ProgressBar Style="{StaticResource ProgressBarPrimaryStripe}" Value="50">
    <ProgressBar.Resources>
        <Color x:Key="DarkPrimaryColor">Black</Color>
    </ProgressBar.Resources>
</ProgressBar>
```

*long-method*
```
<ProgressBar Value="50" Style="{StaticResource ProgressBarPrimaryStripe}">
           <ProgressBar.Foreground>
               <DrawingBrush Viewport="0,0,20,32" TileMode="Tile" ViewportUnits="Absolute" Stretch="None">
                   <DrawingBrush.Transform>
                       <TransformGroup>
                           <RotateTransform Angle="20"/>
                           <TranslateTransform x:Name="MyTransform" X="0"/>
                       </TransformGroup>
                   </DrawingBrush.Transform>
                   <DrawingBrush.Drawing>
                       <GeometryDrawing>
                           <GeometryDrawing.Brush>
                               <LinearGradientBrush EndPoint="1,0" StartPoint="0,0">
                                   <GradientStop Color="Black" Offset="0"/>
                                   <GradientStop Color="Black" Offset="0.5"/>
                                   <GradientStop Color="White" Offset="0.5"/>
                                   <GradientStop Color="White" Offset="1"/>
                               </LinearGradientBrush>
                           </GeometryDrawing.Brush>
                           <GeometryDrawing.Geometry>
                               <RectangleGeometry Rect="0,0,20,32"/>
                           </GeometryDrawing.Geometry>
                       </GeometryDrawing>
                   </DrawingBrush.Drawing>
               </DrawingBrush>
           </ProgressBar.Foreground>
       </ProgressBar>
```

---
![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ProgressBar.gif)

