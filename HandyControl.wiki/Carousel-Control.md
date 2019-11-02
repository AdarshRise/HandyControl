Carousel control allows you to display the Data in a proper way and navigate between them.

# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:Carousel>
            <Image Source="/HandyControlDemo;component/Resources/Img/1.jpg"/>
            <Image Source="/HandyControlDemo;component/Resources/Img/2.jpg"/>
            <Grid Width="600">
                <Image Source="/HandyControlDemo;component/Resources/Img/3.jpg"/>
                <TextBlock Text="示例文本" Style="{StaticResource TextBlockDefault}"/>
            </Grid>
            <Image Source="/HandyControlDemo;component/Resources/Img/4.jpg"/>
            <Image Source="/HandyControlDemo;component/Resources/Img/5.jpg"/>
        </hc:Carousel>
```
| **Available Properti**es | **Description**                                 |
| ------------------------ | ----------------------------------------------- |
| AutoRun                  | Enabling it will automatically change the pages |
| IsCenter                 | put image in center screen                      |

***
![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/Carousel.gif)