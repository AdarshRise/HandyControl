ProgressButton is animated progress bar activated by clicking button.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:ProgressButton Progress="0" Content="Upload"/>
```
or you can use ToggleButton instead of ProgressButton
```
<ToggleButton Style="{StaticResource ToggleButtonLoading}" Progress="0" Content="Upload"/>
```

### Styles
To use Brushes, you should set Style

| Available Styles  [ProgressButton]         | Available Styles [ToggleButton]          |
| ---------------------------- | ---------------------------- |
| ProgressButtonPrimary | ToggleButtonLoading |
| ProgressButtonSuccess    | ToggleButtonLoadingPrimary |
| ProgressButtonInfo | ToggleButtonLoadingSuccess |
| ProgressButtonWarning    | ToggleButtonLoadingInfo |
| ProgressButtonDanger | ToggleButtonLoadingWarning |
| ProgressButtonDefault [Available Only in Custom Version](https://github.com/ghost1372/HandyControls)  | ToggleButtonLoadingDanger |

| **Available Properti**es |
| ------------------------ |
| Style  |
| IsChecked |
| Progress |
| Content |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ProgressButton.png)