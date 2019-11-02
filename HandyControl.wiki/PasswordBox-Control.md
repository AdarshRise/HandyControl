PasswordBox is a control used for easily entering and handling passwords. It is essential to use this control whenever a user is prompted to enter a password.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:PasswordBox Password="123456"/>
```

### Attached Properties
You can use Attached Properties, if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:PasswordBox Password="123456" hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True"/>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ShowEyeButton  | By activating it you can see the content |
| ShowClearButton | By activating it you can empty the content |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/PasswordBox.jpg)