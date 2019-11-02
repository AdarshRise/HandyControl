The ColorPicker is an editor that allows a user to pick a color from predefined color palettes.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:ColorPicker/>
```
also you can use it in Code-behind without using xaml
```
var picker = SingleOpenHelper.CreateControl<ColorPicker>();
            var window = new PopupWindow
            {
                PopupElement = picker
            };
            picker.SelectedColorChanged += delegate { window.Close(); };
            picker.Canceled += delegate { window.Close(); };
 window.Show(OpenButton, false);
```
| Available Events           |
| ---------------------------- |
| SelectedColorChanged |
| Canceled    |



***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ColorPicker.gif)