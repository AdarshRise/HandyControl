This just replaces the standard GroupBox when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <GroupBox Header="Groups"/>
```
To use Attached Properties, you should set Style
```
<GroupBox Style="{StaticResource GroupBoxTab}"/>
```
you can use **TitleElement** Attached Property, For more information about **TitleElement**, see [here](TitleElement-Attach)

```
<GroupBox Style="{StaticResource GroupBoxOriginal}" hc:TitleElement.TitleAlignment="Left"/>

```

| Available styles |
| :--------------- |
| GroupBoxOriginal   |
| GroupBoxTab   |


***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/GroupBox.png)