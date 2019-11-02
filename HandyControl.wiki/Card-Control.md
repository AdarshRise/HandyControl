# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml you can use like this
```
<ListBox Style="{StaticResource WrapPanelHorizontalListBox}" ItemsPanel="{StaticResource FluidMoveBehaviorWrapPanelItemsPanelTemplate}" ItemsSource="{Binding DataList}">
            <ListBox.ItemTemplate>
                <DataTemplate DataType="data:CardModel">
                    <hc:Card MaxWidth="240" Footer="{Binding Footer}">
                        <!--<hc:Card.HeaderTemplate>
                            <DataTemplate>
                                <TextBlock HorizontalAlignment="Left" {Binding}"/>
                            </DataTemplate>
                        </hc:Card.HeaderTemplate>-->
                        <Border CornerRadius="4,4,0,0" Style="{StaticResource BorderClip}">
                            <Image Width="240" Height="240" Source="{Binding Content}" Stretch="Uniform"/>
                        </Border>
                        <hc:Card.FooterTemplate>
                            <DataTemplate>
                                <StackPanel Margin="10">
                                    <TextBlock Text="{Binding DataContext.Header,RelativeSource={RelativeSource AncestorType=hc:Card}}"/>
                                    <TextBlock Text="{Binding}"/>
                                </StackPanel>
                            </DataTemplate>
                        </hc:Card.FooterTemplate>
                    </hc:Card>
                </DataTemplate>
            </ListBox.ItemTemplate>
        </ListBox>   
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Card.png)