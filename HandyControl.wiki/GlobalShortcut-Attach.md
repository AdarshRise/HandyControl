With this property you can use shortcut keys

<table>
<tr>
<td><b>Property</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Host</td>
<td>Enable shortcuts in the desired window</td>
</tr>
</table>

## Usage in Xaml
First add HandyControl NameSpace
```
xmlns:hc="https://handyorg.github.io/handycontrol"
```
Now in windows or other type of view add
```
hc:GlobalShortcut.Host="True"

```
then add KeyBindings
```
  <hc:GlobalShortcut.KeyBindings>
        <KeyBinding Modifiers="Control+Alt" Key="I" Command="{Binding GlobalShortcutInfoCmd}"/>
        <KeyBinding Modifiers="Control+Alt" Key="E" Command="{Binding GlobalShortcutWarningCmd}"/>
    </hc:GlobalShortcut.KeyBindings>
```
