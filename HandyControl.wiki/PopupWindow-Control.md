# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your cs
```
PopupWindow popup = new PopupWindow()
                {
                    MinWidth = 400,
                    Title = "Title",
                    WindowStartupLocation = WindowStartupLocation.CenterScreen,
                    ShowInTaskbar = true,
                    AllowsTransparency = true,
                    WindowStyle = WindowStyle.None
                };

                TextBox txtUsername = new TextBox();

popup.PopupElement = mainStack;
popup.ShowDialog();
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| PopupElement | Popup Children |

***