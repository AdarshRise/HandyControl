Growl control can be used when you want to arrange notification information from top to bottom in the right area of the window.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml Add a StackPanel container to the right side of the specified window
```
<hc:ScrollViewer VerticalScrollBarVisibility="Hidden" HorizontalAlignment="Right" IsEnableInertia="True" IsPenetrating="True">
 <StackPanel controls:Growl.GrowlParent="True" VerticalAlignment="Top" Margin="0,10,10,10"/>
</hc:ScrollViewer>
```
Call Growl the relevant interface to display the specified message
```
Growl.Warning(new GrowlInfo { Message = "Check Update"});
```
or
```
Growl.Success("Updated！");
```
## Display information notifications in any container
give the StackPanel container a message tag: SuccessMsg
```
< ScrollViewer  VerticalScrollBarVisibility = "Hidden"  HorizontalAlignment = "Right" > 
< StackPanel hc:Growl.Token = "SuccessMsg" VerticalAlignment = "Top" Margin = "0,10,10,10" />
 </ ScrollViewer >
```
Use the message tag: SuccessMsg, and call Growl the relevant interface to display the specified message
```
Growl.Success("Updated！", "SuccessMsg");
```
You can change the text of the confirmation and cancellation buttons
```
Growl.Info(new GrowlInfo {
                        Message = "we found new version",
                        CancelStr = "later",
                        ConfirmStr = "lets do this"
                    });
```
# Handle Confirm or Cancel Event
Use **ActionBeforeClose** property to handle Confirm or Cancel event 
```
Growl.Info(new GrowlInfo {
                        Message = "we found new version",
                        ActionBeforeClose = isConfirm =>
                        {
                            if (isConfirm)
                                MessageBox.Show("Confirmed");
                            else
                                MessageBox.Show("Canceled");
                            return true;
                        }
                    });
```

***
***
### Update:
now you can use growl in desktop
```
Growl.InfoGlobal("GrowlInfo");
//OR
Growl.SuccessGlobal("GrowlSuccess");
// OR
Growl.WarningGlobal(new GrowlInfo
            {
                Message = "GrowlWarning",
                CancelStr = "Ignore",
                ActionBeforeClose = isConfirmed =>
                {
                    Growl.InfoGlobal(isConfirmed.ToString());
                    return true;
                }
            });
// OR
Growl.ErrorGlobal("GrowlError");
// OR
Growl.AskGlobal("GrowlAsk", isConfirmed =>
            {
                Growl.InfoGlobal(isConfirmed.ToString());
                return true;
            });
// OR
Growl.FatalGlobal(new GrowlInfo
            {
                Message = "GrowlFatal",
                ShowDateTime = false
            });
// And for Clearing growls
Growl.ClearGlobal();
```

# Properties
|Member Name|Type|Description|Default|
|--- |--- |--- |--- |
|Message|string|Notification content|-|
|ShowDateTime|bool| Whether to display notification time|true|
|WaitTime|int|Wait for automatic shutdown time|6|
|CancelStr|string|Cancel String|Lang.Cancel|
|ConfirmStr|string|Confirm String|Lang.Confirm|
|ActionBeforeClose|Func<bool, bool>|Delegate before closing|-|
|StaysOpen|bool|Keep open|false|
|IsCustom|bool|Customize behavior|false|
|Type|InfoType|Message Type|InfoType.Success|
|IconKey|string|icon key name|-|
|IconBrushKey|string|icon brush key name|-|
|ShowCloseButton|bool| Whether to display the close button|true|
|Token|string|Message tag|-|

# Attribute
|name|Description|
|--- |--- |
|Token|Used to set message tags|
|GrowlParent|Used to set up a message container|

# Method
|name|Description|
|--- |--- |
|Success(string)|Display a success notification|
|Success(string, string)|Display a success notification with the specified message tag|
|Success(GrowlInfo)|Use a full message initialization model to display a success notification|
|Info(string)|Display a message notification|
|Info(string, string)|Display a message notification with the specified message tag|
|Info(GrowlInfo)|Display a message notification using the full message initialization model|
|Warning(string)|Display a warning notification|
|Warning(string, string)|Display a warning notification with the specified message tag|
|Warning(GrowlInfo)|Display a warning notification using the full message initialization model|
|Error(string)|Show an error notification|
|Error(string, string)|Display an error notification with the specified message tag|
|Error(GrowlInfo)|Use the full message initialization model to display an error notification|
|Fatal(string)|Show a serious notification|
|Fatal(string, string)|Display a critical notification with the specified message tag|
|Fatal(GrowlInfo)|Use a full message initialization model to display a serious notification|
|Ask(string, Func<bool, bool>)|Display a query|
|Ask(string, Func<bool, bool>, string)|Display a query notification with the specified message tag|
|Ask(GrowlInfo)|Use a full message initialization model to display a query notification|
|Register(string, Panel)|Register a message tag for the specified container|
|Unregister(string, Panel)|Unregister the message tag for the specified container|
|Unregister(Panel)|Unregister if the container is registered with a message tag|
|Clear( )|Clear the message in the currently used message container|
|Clear(string)|Empty the message in the message container with the specified message tag|

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Growl.gif)