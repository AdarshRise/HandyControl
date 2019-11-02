Neon Label is a Styled and Animated Label (Source: https://github.com/Panuon/PanuonUI.Silver/blob/master/Panuon.UI.Silver/Controls/NeonLabel.xaml)

```
 <hc:NeonLabel x:Name="neon"
Content="I have to type these characters to make it longer."/>
```
then
```
neon.Next(NeonLabelType.FadeNext, "your new text");
// OR
neon.Next(NeonLabelType.SlideNext, "your new text");

// OR
neon.Next(NeonLabelType.ScrollToEnd, null, 4);
```

You can do this to create a better example
```
private DispatcherTimer _dispatcherTimer;
private int count = 0;

public Demo()
        {
            this.InitializeComponent();

            _dispatcherTimer = new DispatcherTimer() { Interval = TimeSpan.FromSeconds(1) };
            _dispatcherTimer.Tick += DispatcherTimer_Tick;
            _dispatcherTimer.Start();
        }
 private void DispatcherTimer_Tick(object sender, EventArgs e)
        {
            count++;
            switch (count)
            {
                case 1:
                case 2:
                case 3:
                case 4:
                    break;
                case 5:
                    count = 0;
                    break;
            }
            neon2.Next(NeonLabelType.FadeNext, Guid.NewGuid().ToString());
            neon3.Next(NeonLabelType.SlideNext, Guid.NewGuid().ToString());
            if (count == 1)
                neon.Next(NeonLabelType.ScrollToEnd, null, 4);
        }
```

***
![NeonLabel](https://github.com/ghost1372/HandyControls/blob/develop/Resources/NeonLabel.gif)
