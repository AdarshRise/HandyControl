This just replaces the standard ProgressBar when you drop in the library, nothing fancy to activate it. 

## Usage
```
 <ProgressBar Value="20"/>
```
To use brushes, you should set Style
```
<ProgressBar Value="20" Style="{StaticResource ProgressBarSuccess}"/>
```
| Available styles         |                          |
| ------------------------ | ------------------------ |
| ProgressBarSuccess       | ProgressBarSuccessStripe |
| ProgressBarInfo          | ProgressBarInfoStripe    |
| ProgressBarWarning       | ProgressBarWarningStripe |
| ProgressBarDanger        | ProgressBarDangerStripe  |
| ProgressBarPrimaryStripe | ProgressBarFlat          |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ProgressBar.gif)