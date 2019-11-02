# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
 <hc:CoverFlow x:Name="CoverFlowMain" Width="500" Height="300"/>
```
now in your Code-behind
```
CoverFlowMain.AddRange(new []
            {
                new Uri(@"pack://application:,,,/Resources/Img/Album/1.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/2.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/3.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/4.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/5.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/6.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/7.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/8.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/9.jpg"),
                new Uri(@"pack://application:,,,/Resources/Img/Album/10.jpg")
            });
            CoverFlowMain.JumpTo(2);
```
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/CoverFlow.gif)