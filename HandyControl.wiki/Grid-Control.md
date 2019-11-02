Grid control with easy to use in rows or columns

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<StackPanel Margin="32">
            <hc:Row>
                <hc:Col>
                    <Border Background="{DynamicResource BorderBrush}"/>
                </hc:Col>
                <hc:Col>
                    <Border Background="{DynamicResource SecondaryBorderBrush}"/>
                </hc:Col>
            </hc:Row>
        </StackPanel>
```
You must use **hc:Row** to use the row and **hc:Col** for column

| **Available Properti**es for Col | **Available Properties for Row**                |
| ------------------------ | ------------------------------------------------------------ |
| Span | Gutter |
| Offset (Gets or sets a value that determines grid columns offset ) | |
| Layout (Gets or sets a value that determines grid columns for XS(extra small), SM(small), MD(medium), LG(large), XL(extra large) devices.) | |
| IsFixed | |

for using **Layout** (xs, sm, md, lg, xl, xxl, Auto)
```
 <hc:Col Layout="8, 6, 4, 3, 1}"/>

// OR

 <hc:Col Layout="8 6 4 3 1}"/>

// OR

//Add refrence
xmlns:extension="clr-namespace:HandyControl.Tools.Extension;assembly=HandyControl"

<hc:Col Layout="{extension:ColLayout Xs=8, Sm=6, Md=4, Lg=3, Xl=1}">
```

***

![](https://raw.githubusercontent.com/NaBian/HandyControl/master/Resources/Grid.gif)