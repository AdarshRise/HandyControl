An attached property is intended to be used as a type of global property that is settable on any object. 

LinkElement Contains 

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Link</td>
<td>Gets or sets Link Address</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now
```
<hc:Shield controls:LinkElement.Link="https://github.com"/>
```

## Usage in Code-Behind
```
LinkElement.SetLink(control, "https://github.com");

LinkElement.GetLink(control);
```
