### RegistryHelper class for working with Registry

### Add Key [value can be everything (bool, int, string,...), default HKEYType is CurrentUser for other type you need Admin Access]
```
RegistryHelper.AddOrUpdateKey("myKey", "myFolder", value);
//OR
RegistryHelper.AddOrUpdateRegistryKey("myKey4", "myFolder", "test", HKEYType.LocalMachine);
```

### Get Key [you can cast value to any type you want]
```
RegistryHelper.GetKey<bool>("myKey", "myFolder");
RegistryHelper.GetKey<string>("myKey", "myFolder");
```

### Delete Key [default value for IsDeleteSubFolder is False]
```
RegistryHelper.DeleteKey("myKey", "myFolder");
// OR
RegistryHelper.DeleteKey("myKey", "myFolder", True);
```

***