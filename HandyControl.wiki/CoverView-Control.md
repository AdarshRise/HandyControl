# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:CoverView>
            <hc:CoverViewItem>
                <hc:CoverViewItem.Header>
                    <Image Source="/HandyControlDemo;component/Resources/Img/Album/1.jpg"/>
                </hc:CoverViewItem.Header>
               <TextBlock Text="Content"/>
            </hc:CoverViewItem>

<hc:CoverViewItem>
                <hc:CoverViewItem.Header>
                    <Image Source="/HandyControlDemo;component/Resources/Img/Album/2.jpg"/>
                </hc:CoverViewItem.Header>
               <TextBlock Text="Content"/>
            </hc:CoverViewItem>
</hc:CoverView>
```

## ItemSource
if you want to bind your data to ItemsSource you can do it like this
```
 <hc:CoverView ItemWidth="160" ItemHeight="160" ItemsSource="{Binding DataList}">
            <hc:CoverView.ItemHeaderTemplate>
                <DataTemplate>
                    <Image Source="{Binding ImgPath}"/>
                </DataTemplate>
            </hc:CoverView.ItemHeaderTemplate>
            <hc:CoverView.ItemTemplate>
                <DataTemplate>
                     <TextBlock Text="Content" VerticalAlignment="Center" HorizontalAlignment="Center" Foreground="White"/>
                </DataTemplate>
            </hc:CoverView.ItemTemplate>
        </hc:CoverView>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ItemWidth                | Specifies the width of the item                              |
| ItemHeight               | Specifies the length of the item                             |
| ItemContentHeight        | Specifies the length of the opened item                      |
| ItemContentHeightFixed   | Specifies the length of the opened item                      |
| ItemSource               | if you want to bind your data to ItemsSource you can do it like this |
| ShowContent | Show or Hide Content when selected items, Only Available in [Custom Version](https://github.com/ghost1372/handyControls) |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/CoverView.gif)