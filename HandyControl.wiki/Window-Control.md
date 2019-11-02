To use the Window Control, you need to change Window to **BlurWindow** and set Style to **WindowWin10** or **WindowBlur** in your main window ([For more information about themes, see here](https://github.com/ghost1372/HandyControl/wiki/Themes-Usage-Instructions))
```
<hc:BlurWindow 
  Style={StaticResources WindowBlur}
...
```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/BlurWindow.png)

***
### Attached Properties

you can use **WindowAttach** Attached Property for dragging window or any control. For more information about **WindowAttach**, see [here](WindowAttach-Attach)
```
 <hc:BlurWindow WindowAttach:IsDragElement="True" 
...
/>
```

# Shortcut
you should use **GlobalShortcut.KeyBindings**
```
  <hc:GlobalShortcut.KeyBindings>
        <KeyBinding Modifiers="Control+Alt" Key="E" Command="{Binding GlobalShortcutErrorCmd}"/>
        <KeyBinding Modifiers="Control+Alt" Key="I" Command="{Binding Main.GlobalShortcutInfoCmd, Source={StaticResource Locator}}"/>
    </hc:GlobalShortcut.KeyBindings>
```
# Menu
If you want to use menus in the title bar, you should use **NonClientAreaContent** property
```
<hc:Window.NonClientAreaContent>
  <StackPanel VerticalAlignment="Stretch" Orientation="Horizontal">
        <Button Content="About" Style="{StaticResource ButtonCustom}"/>
        <Button Content="Help" Style="{StaticResource ButtonCustom}"/>
        <Menu>
            <MenuItem Header="Repository">
                <MenuItem Header="GitHub"/>
            </MenuItem>
        </Menu>
   </StackPanel>
</hc:Window.NonClientAreaContent>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| NonClientAreaBackground  | Specifies the title bar background |
| NonClientAreaForeground | Specifies the title bar foreground |
| OtherButtonHoverBackground  | Specifies the Maximize and Minimize Buttons background when mouse hover it |
| OtherButtonHoverForeground | Specifies the Maximize and Minimize Buttons foreground when mouse hover it |
| OtherButtonBackground | Specifies the Maximize and Minimize Buttons background |
| OtherButtonForeground | Specifies the Maximize and Minimize Buttons foreground |
| ShowNonClientArea | Specifies whether to display the title bar or not |
| NonClientAreaContent | You can put any objects or text in the title bar |
| NonClientAreaHeight | Specifies the title bar Height |
| CloseButtonBackground | Specifies the Close Button Background |
| CloseButtonForeground | Specifies the Close Button Foreground |
| CloseButtonHoverBackground | Specifies the Close Button Background when mouse hover it |
| CloseButtonHoverForeground | Specifies the Close Button Foreground when mouse hover it |
| ShowTitle | Specifies whether to display the program title in the title bar |

### NonClientAreaContent
If you want to put objects, you should use it in this way
```
<hc:Window.NonClientAreaContent>
  <!-- Put your objects here -->
</hc:Window.NonClientAreaContent>
```
### 
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/DarkTheme.png)