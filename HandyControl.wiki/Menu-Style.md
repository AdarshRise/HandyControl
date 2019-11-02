This just replaces the standard Menu when you drop in the library, nothing fancy to activate it. 

## Usage
### Simple
```
 <Border Background="Transparent">
                 <Border.ContextMenu>
                     <ContextMenu>
                    <MenuItem Header="Menu item 1" />
                    <MenuItem Header="Menu item 2" />
                    <Separator />
                    <MenuItem Header="Menu item 3" />
                </ContextMenu>
                 </Border.ContextMenu>
             </Border>
```

### Binding
```
 <Border Background="Transparent">
                 <Border.ContextMenu>
                     <ContextMenu ItemsSource="{Binding DataList}">
                         <ContextMenu.ItemTemplate>
                             <HierarchicalDataTemplate ItemsSource="{Binding DataList}">
                                 <TextBlock Text="{Binding Name}"/>
                             </HierarchicalDataTemplate>
                         </ContextMenu.ItemTemplate>
                     </ContextMenu>
                 </Border.ContextMenu>
             </Border>
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ContextMenu.png)