You can use TransitioningContentControl control if you want your content to run with animation.

# Usage
First add HandyControl refrence
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
then in your xaml
```
<hc:TransitioningContentControl>
 <Grid>

 </Grid>
</hc:TransitioningContentControl>
```
| **Available Property** | **Description**                                             |
| ---------------------- | ----------------------------------------------------------- |
| Transition | Page loading animation [**DefaultTransition**, **Normal**, **UpTransition**, **DownTransition**]                                        |
