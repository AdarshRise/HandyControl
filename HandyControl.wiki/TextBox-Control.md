TextBox control represents a TextBox that allows you to define a placeholder to be displayed when the content is empty and the control is not focused. This is useful when you want to display additional information when having an empty text input control.
# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:TextBox/>
```

### Attached Properties
You can use Attached Properties, if you want to use Placeholder and other features you should use **InfoElement** Attached Property, For more information about **InfoElement**, see [here](InfoElement-Attach)
```
<hc:TextBox hc:InfoElement.TitleWidth="140" hc:InfoElement.Placeholder="Please Enter Content" hc:InfoElement.TitleAlignment="Left" hc:InfoElement.Title="Title" hc:InfoElement.Necessary="True"/>
```
| **Available Properti**es | **Description**                                              |
| ------------------------ | ------------------------------------------------------------ |
| ShowClearButton  | By activating it you can empty the content |
| TextType  |By specifying it, you can control the input text |

| Available TextType | Available TextType | Available TextType |
| ------------------ | ------------------ | ------------------ |
| Mail               | NDouble            | Number             |
| Chinese            | NInt               | PDouble            |
| Common             | NnDouble           | PInt               |
| Digits             | NnInt              | Phone              |
| Double             | NpDouble           | Url                |
| Int                | NpInt              |                    |

***

![](https://github.com/HandyOrg/HandyOrgResource/blob/master/HandyControl/Resources/TextBox.jpg)