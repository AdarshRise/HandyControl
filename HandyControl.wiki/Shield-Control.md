Shield is Concise, consistent, and legible badges.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Shield Subject=".net" Status=">=4.0" Color="#1182c3"/>
```

### Attached Properties
you can use Attached Properties
if you want to use Link, you should use **LinkElement** Attached Property, For more information about **LinkElement**, see [here](LinkElement-Attach)

```
<hc:Shield Subject="chat" Status="on gitter" Color="#4eb899" Command="hc:ControlCommands.OpenLink" hc:LinkElement.Link="https://github.com"/>

```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Subject  | Specifies the Subject of Shield |
| Status | Specifies the Status of Shield |
| Color | Specifies the color of the shield Status |
| Command | By Using it, The command executes by clicking on the shield |
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Shield.png)