# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:RunningBlock Content="Text"/>
```
OR you can put any content
```
<hc:RunningBlock Duration="0:0:20" IsRunning="True">
                <StackPanel Orientation="Horizontal">
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/1.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/2.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/3.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/4.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/5.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/6.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/7.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/8.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/9.gif" Margin="10,0"/>
                    <hc:GifImage Uri="/HandyControlDemo;component/Resources/Img/QQ/10.gif" Margin="10,0"/>
                </StackPanel>
            </hc:RunningBlock>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| Duration | Specifies the duration of the animation motion  |
| IsRunning | Get or Set Move object |
| AutoReverse | Get or Set Object Move Reverse or not |
| Orientation | Get or Set Object Move Orientation |
| Runaway |  |
| AutoRun | Get or Set Autorun Object |


***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/RunningBlock.png)