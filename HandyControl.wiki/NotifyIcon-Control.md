This is an alternative implementation of a NotifyIcon (system tray icon) for the WPF platform.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
 <hc:NotifyIcon Name="notify" Text="HandyControl">
                <hc:NotifyIcon.ContextMenu>
                    <ContextMenu FlowDirection="RightToLeft" FontFamily="{StaticResource IRANSans}">
                        <MenuItem Command="hc:ControlCommands.PushMainWindow2Top" Header="Open"/>
                        <MenuItem Command="hc:ControlCommands.ShutdownApp" Header="Exit"/>
                    </ContextMenu>
                </hc:NotifyIcon.ContextMenu>
            </hc:NotifyIcon>
```
or you can use like this
```
<hc:NotifyIcon x:Name="NotifyIconContextContent" Text="HandyControl" Icon="/HandyControlDemo;component/Resources/Img/icon-white.ico">
                <hc:NotifyIcon.ContextContent>
                    <Border>
                        <StackPanel VerticalAlignment="Center" Margin="16">
                            <Path Width="100" Height="100" Fill="#f06632" Data="{StaticResource LogoGeometry}"/>
                            <StackPanel Margin="0,16,0,0" HorizontalAlignment="Center" Orientation="Horizontal">
                                <Button Click="ButtonPush_OnClick" Command="hc:ControlCommands.PushMainWindow2Top" MinWidth="100" Content="OpenPanel"/>
                                <Button Command="hc:ControlCommands.ShutdownApp" Margin="16,0,0,0" MinWidth="100" Style="{StaticResource ButtonPrimary}" Content="Exit"/>
                            </StackPanel>
                        </StackPanel>
                    </Border>
                </hc:NotifyIcon.ContextContent>
                
            </hc:NotifyIcon>
```
you can use ```hc:ControlCommands``` for exit app or open it. or you can use event instead of it.
```
private void ButtonPush_OnClick(object sender, RoutedEventArgs e) => NotifyIconContextContent.CloseContextControl();
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| IsBlink | By setting IsBlink to True, The application icon starts blinking |
| Text | NotifyIcon Text showing when mouse hover it |
| Visibility | Show or hide NotifyIcon |
| Icon | NotifyIcon icon |

## BallonTip
```
NotifyIcon.ShowBalloonTip("HandyControl", "Hello", NotifyIconInfoType.None, ContextMenuIsShow ? MessageToken.NotifyIconDemo : MessageToken.NotifyIconContextDemo);

```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/NotifyIcon.png)