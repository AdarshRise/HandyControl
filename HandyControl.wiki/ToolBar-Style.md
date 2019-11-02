This just replaces the standard ToolBar when you drop in the library, nothing fancy to activate it. 

## Usage
```
  <ToolBarTray>
            <ToolBar Header="Title">
                <CheckBox IsChecked="True"/>
                <Separator Margin="10,0,0,0"/>
                <RadioButton/>
                <StackPanel Orientation="Horizontal">
                    <RadioButton IsChecked="True"/>
                    <RadioButton />
                </StackPanel>
                <Button Content="Button"/>
                <Button Content="Button" Style="{StaticResource ButtonPrimary}"/>
            </ToolBar>
            <ToolBar Band="1" >
                <ComboBox ItemsSource="{Binding DataList}" SelectedIndex="0"/>
                <TextBox Text="Text"/>
            </ToolBar>
        </ToolBarTray>
```

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/ToolBar.png)