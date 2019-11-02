SideMenu is Menu that provides navigation for your app.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:SideMenu>
<hc:SideMenuItem Header="Overview">
            <hc:SideMenuItem.Icon>
                <Image Source="/HandyControlDemo;component/Resources/Img/DevOps/DevOps-Overview.png" Width="24" Height="24"/>
            </hc:SideMenuItem.Icon>
            <hc:SideMenuItem Header="Summary">
                <hc:SideMenuItem.Icon>
                    <TextBlock Text="&#xf2cb;" Style="{StaticResource TextBlockFabricIcons}"/>
                </hc:SideMenuItem.Icon>
            </hc:SideMenuItem>
            <hc:SideMenuItem Header="Dashboards">
                <hc:SideMenuItem.Icon>
                    <TextBlock Text="&#xf246;" Style="{StaticResource TextBlockFabricIcons}"/>
                </hc:SideMenuItem.Icon>
            </hc:SideMenuItem>
        </hc:SideMenuItem>

<hc:SideMenuItem Header="Test Plans">
            <hc:SideMenuItem.Icon>
                <Image Source="/HandyControlDemo;component/Resources/Img/DevOps/DevOps-TestPlans.png" Width="24" Height="24"/>
            </hc:SideMenuItem.Icon>
            <hc:SideMenuItem Header="Test Plans">
                <hc:SideMenuItem.Icon>
                    <TextBlock Text="&#xf3ab;" Style="{StaticResource TextBlockFabricIcons}"/>
                </hc:SideMenuItem.Icon>
            </hc:SideMenuItem>
        </hc:SideMenuItem>
</hc:SideMenu>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ExpandMode  | You can specify that all menus are open or just an open category |
| Header  | Side menu header text |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/SideMenu.png)