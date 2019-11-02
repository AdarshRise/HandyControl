Run only one version of the program at a time

write the following code in the App.cs file
```
InstanceHelper.IsSingleInstance();
```
The above method returns true or false, However, it does everything automatically (closing app, focusing running app, showing message)
You can also change the message text or not display the message
```
InstanceHelper.IsSingleInstance(false, "bye!");
```