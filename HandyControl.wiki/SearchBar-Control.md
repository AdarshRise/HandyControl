# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:SearchBar/>
```

### Attached Properties
To use Attached Properties, you should set Style

if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
 <hc:SearchBar controls:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" Style="{StaticResource SearchBarPlus}" hc:InfoElement.Necessary="True"/>
```

| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| IsRealTime  | By Using it you can search when you type in realtime, without need to click on search button or hit enter |
| ShowClearButton | By Using it you can empty the content |
| TextType | By specifying it, you can control the input text |

| Available TextType | Available TextType | Available TextType |
| ------------------ | ------------------ | ------------------ |
| Mail               | NDouble            | Number             |
| Chinese            | NInt               | PDouble            |
| Common             | NnDouble           | PInt               |
| Digits             | NnInt              | Phone              |
| Double             | NpDouble           | Url                |
| Int                | NpInt              |                    |


| Available Styles           | Available Events |
| ---------------------------- | ---------------------------- |
| SearchBarPlus | SearchStarted |
| SearchBarExtend    |          |

***
![](https://github.com/handyorg/HandyControl/blob/master/Resources/SearchBar.png)