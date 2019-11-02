## Usage
you can use brush in ```Background``` or any other property that use brush
```
<Label Content="DarkPrimaryBrush" Background="{DynamicResource DarkPrimaryBrush}" Foreground="White"/>
<Label Content="DangerBrush" Style="{StaticResource LabelDanger}"/>
```
To automatically change the brushes by changing the application's theme You should use ```DynamicResource``` in ```Background``` otherwise you can use ```StaticResources```

| Available Brushes| |||
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
|PrimaryBrush| DarkWarningBrush | AccentBrush | ReverseTextBrush |
|DarkPrimaryBrush| InfoBrush | DarkAccentBrush | TextIconBrush |
|DangerBrush| DarkInfoBrush | PrimaryTextBrush | BorderBrush |
|DarkDangerBrush| SuccessBrush | SecondaryTextBrush | SecondaryBorderBrush |
|WarningBrush| DarkSuccessBrush | ThirdlyTextBrush | BackgroundBrush |
|RegionBrush| SecondaryRegionBrush | ThirdlyRegionBrush | TitleBrush |
|DefaultBrush| DarkDefaultBrush | DarkMaskBrush | DarkOpacityBrush |
***

![](https://github.com/handyorg/HandyOrgResource/blob/master/HandyControl/Resources/Brush.png)