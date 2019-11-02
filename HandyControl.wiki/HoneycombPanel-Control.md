# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<ListBox Style="{StaticResource ListBoxCustom}">
                    <ListBox.ItemsPanel>
                        <ItemsPanelTemplate>
                            <hc:HoneycombPanel hc:PanelElement.FluidMoveBehavior="{StaticResource BehaviorXY200}"/>
                        </ItemsPanelTemplate>
                    </ListBox.ItemsPanel>
                    <ListBox.ItemTemplate>
                        <DataTemplate DataType="data:CardModel">
                            <hc:Gravatar Style="{StaticResource GravatarCircle}" Margin="10" Source="{Binding Content}"/>
                        </DataTemplate>
                    </ListBox.ItemTemplate>
                </ListBox>
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/HoneycombPanel.png)