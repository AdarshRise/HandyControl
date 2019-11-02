# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Gravatar Id="User1"/>

```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Source  | you can set image in source but first you should set Style |

| Available Styles |
| ------------------------ |
| GravatarCircleImg |


### Source
you can set image in source but first you should set Style
```
<hc:Gravatar Style="{StaticResource GravatarCircleImg}">
 <Image Source="/HandyControlDemo;component/Resources/Img/Album/2.jpg"/>
</hc:Gravatar>

```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Gravatar.gif)