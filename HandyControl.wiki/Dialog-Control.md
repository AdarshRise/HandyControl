# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml first create a usercontrol like this
```
<Border 
...
xmlns:hc="https://handyorg.github.io/handycontrol"
        CornerRadius="10"
        Background="{DynamicResource RegionBrush}">
    <Grid>
        <TextBlock Text="PleaseWait"/>
        <Button Width="22" Height="22" Command="hc:ControlCommands.Close" Style="{StaticResource ButtonIcon}" Foreground="{DynamicResource PrimaryBrush}" hc:IconElement.Geometry="{StaticResource ErrorGeometry}"/>    
    </Grid>
</Border>
```
now when you want to show a dialog
```
<Button Click="Button_Click"/>
```
and in click event
```
Dialog.Show(new TextDialog());
```
***

![](https://github.com/handyorg/HandyControl/blob/master/Resources/Dialog.png)