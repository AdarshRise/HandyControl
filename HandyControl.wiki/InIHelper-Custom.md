InIHelper class is for working with ini file in simple way.

### Add Value [you can use default **section** and **path**]
```
InIHelper.AddValue("key1", "test1");
                    InIHelper.AddValue("key2", "test2");
                    InIHelper.AddValue("key3", "test3", "mySection");
                    InIHelper.AddValue("file4", "test4", "mySection");
                    InIHelper.AddValue("file5", "test5", "mySection");
                    InIHelper.AddValue("file6", "test6", "mySection2", @"D:\config.ini");
```

### Read Value
```
MessageBox.Info(InIHelper.ReadValue("key1"));
// OR
MessageBox.Info(InIHelper.ReadValue("key3", "mySection"));
// OR
MessageBox.Info(InIHelper.ReadValue("key3", "mySection", @"D:\config.ini"));
```

### Delete Key [you can delete a **key** or **section**]
```
InIHelper.DeleteKey("key4", "mySection");
InIHelper.DeleteSection("mySection");
InIHelper.DeleteKey("key4", "mySection", @"D:\config.ini");
```
### Exist Key [you can check if a key exist or not]
```
MessageBox.Info(InIHelper.IsKeyExists("key4", "mySection"));
```
***