# Usage
First add HandyControl refrence
```
 xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your app.xaml copy this style
```
<Style x:Key="CirclePanelButton" BasedOn="{StaticResource ButtonCustom}" TargetType="Button">
        <Setter Property="UseLayoutRounding" Value="False"/>
        <Setter Property="Height" Value="77"/>
        <Setter Property="Width" Value="36.06"/>
        <Setter Property="Template">
            <Setter.Value>
                <ControlTemplate TargetType="Button">
                    <Grid>
                        <Path Data="{StaticResource CirclePanelDemoGeometry}" Fill="{DynamicResource PrimaryBrush}" Height="77" Width="36.06"/>
                        <Path Data="{StaticResource CirclePanelRightGeometry}" Stretch="Uniform" Margin="12" Fill="White"/>
                    </Grid>
                    <ControlTemplate.Triggers>
                        <Trigger Property="IsMouseOver" Value="True">
                            <Setter Property="Opacity" Value=".9"/>
                        </Trigger>
                        <Trigger Property="IsPressed" Value="True">
                            <Setter Property="Opacity" Value=".6"/>
                        </Trigger>
                        <Trigger Property="IsEnabled" Value="False">
                            <Setter Property="Opacity" Value="0.4"/>
                        </Trigger>
                    </ControlTemplate.Triggers>
                </ControlTemplate>
            </Setter.Value>
        </Setter>
    </Style>
```
now in your xaml
```
  <hc:CirclePanel>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
            <Button Style="{StaticResource CirclePanelButton}"/>
   </hc:CirclePanel>
```
| **Available Properti**es | **Description**                                        |
| ------------------------ | ------------------------------------------------------ |
| Diameter                 | The size of the panel can be specified by its diameter |
***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/CirclePanel.jpg)