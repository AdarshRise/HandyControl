# Usage
first create new usercontrol like this
```
<Border x:Class="HandyControlDemo.UserControl.AppNotification"
             xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
             xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
             xmlns:hc="https://handyorg.github.io/handycontrol"
             Background="White"
             Width="320"
             Height="518">
    <hc:SimplePanel>
        <Path Margin="0,36,0,0" VerticalAlignment="Top" Width="70" Height="70" Data="{StaticResource LogoGeometry}" Fill="#f06632"/>
        <TextBlock Text="HandyControl" FontSize="30" Foreground="{StaticResource PrimaryBrush}" HorizontalAlignment="Center" Margin="0,122,0,0" VerticalAlignment="Top"/>
        <Button Command="hc:ControlCommands.CloseWindow" CommandParameter="{Binding RelativeSource={RelativeSource Self}}" Content="{x:Static hc:Lang.Close}" HorizontalAlignment="Stretch" VerticalAlignment="Bottom" Margin="10,0,10,10"/>
    </hc:SimplePanel>
</Border>

```
then in your cs class call notification
```
Notification.Show(new AppNotification(), ShowAnimation.Fade, True);
```
| Animation |
| --------- |
| Fade |
| HorizontalMove |
| verticalMove |
***