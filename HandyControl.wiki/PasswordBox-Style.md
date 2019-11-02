This just replaces the standard PasswordBox when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <PasswordBox Password="123456"/>
```
To use Attached Properties, you should set Style
```
<PasswordBox Password="123456" Style="{StaticResource PasswordBoxExtend}"/>

```
you can use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)

```
<PasswordBox hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title Demo" hc:InfoElement.Necessary="True" Style="{StaticResource PasswordBoxExtend}"/>

```

| Available styles |
| :--------------- |
|PasswordBoxExtend|



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/PasswordBox.jpg)