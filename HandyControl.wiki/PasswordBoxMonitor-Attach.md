An attached property is intended to be used as a type of global property that is settable on any object. 

PasswordBoxMonitor Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>PasswordLength</td>
<td>Gets or sets Length of Characters</td>
</tr>
<tr>
<td>IsMonitoring</td>
<td>Gets or sets IsMonitoring</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<PasswordBox hc:PasswordBoxMonitor.PasswordLength="10" hc:PasswordBoxMonitor.IsMonitoring="True"/>

```

## Usage in Code-Behind
```
PasswordBoxMonitor.SetPasswordLength(control, 10);
PasswordBoxMonitor.IsMonitoring(control, True);

PasswordBoxMonitor.GetPasswordLength(control);
```
