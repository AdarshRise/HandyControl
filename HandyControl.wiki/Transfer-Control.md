# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Transfer ItemsSource="{Binding DataList}">
            <hc:Transfer.ItemTemplate>
                <DataTemplate>
                    <TextBlock Text="{Binding Name}"/>
                </DataTemplate>
            </hc:Transfer.ItemTemplate>
        </hc:Transfer>
```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Transfer.png)