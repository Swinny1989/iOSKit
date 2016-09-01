# iOSKit - Coming to Unity Asset store soon -In Progress-

iOSKit is a framework in development to be released on the Unity Asset Store.

##Documentation


###Single Button Alert

Show an iOS `UIAlertController` with a single Ok button. If the device is running iOS 7 then a UIAlertView will be used.

```csharp
public static void ShowPopup(string title, string message, System.Action<string> callback) 
```

**Example**

```csharp
iOSKitManager.ShowPopup("Test Title", "Test Message", buttonPressed => { 
			Debug.Log("Button Pressed: " + buttonPressed);
		});
```

###Multiple Button Alert
Show an iOS `UIAlertController` with multiple buttons. If the device is running iOS 7 then a UIAlertView will be used.

```csharp
public static void ShowPopup(string title, string message, string[] buttons, System.Action<string> callback) 
```

**Example**

```csharp
iOSKitManager.ShowPopup("Test Title", "Test Message", new string[]{"Button One", "Button Two"}, buttonPressed => { 
			Debug.Log("Button Pressed: " + buttonPressed);
		});
```

