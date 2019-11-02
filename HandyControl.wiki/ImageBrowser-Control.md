With ImageBrowser control, you can display your own images, including features like zoom and rotation...

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:ImageViewer Background="{DynamicResource BackgroundBrush}" ImageSource="/HandyControlDemo;component/Resources/Img/1.jpg"/>
```
also you can use it in Code-Behind without using xaml
```
new ImageBrowser(new Uri("pack://application:,,,/Resources/Img/1.jpg")).Show();
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ImageBrowser.gif)