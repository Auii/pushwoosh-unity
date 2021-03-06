# class PushNotificationsIOS #

Provides specific features for iOS platform.

## Base class methods

[public string PushToken](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#pushtoken)  
[public string HWID](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#hwid)   
[public void SetIntTag(string tagName, int tagValue)](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#setinttag)  
[public void SetStringTag(string tagName, string tagValue)](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#setstringtag)  
[public void SetListTag(string tagName, List<object> tagValues)](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#setlisttag)  
[public void StartTrackingGeoPushes()](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#starttrackinggeopushes)  
[public void StopTrackingGeoPushes()](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#stoptrackinggeopushes)  
[public void ClearNotificationCenter()](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#clearnotificationcenter)  
[static public void SetBadgeNumber(int number)](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#setbadgenumber)  
[static public void AddBadgeNumber(int deltaBadge)](https://github.com/Pushwoosh/pushwoosh-unity/blob/master/Documentation/Pushwoosh.md#addbadgenumber)  

## Methods

[public void registerForPushNotifications()](#registerforremotenotifications)  
[public void unregisterForPushNotifications()](#unregisterforremotenotifications)  


### registerForRemoteNotifications

Registers for push notifications. Called automatically in `Start` function.

```csharp
public void registerForRemoteNotifications()
```

---
### unregisterForRemoteNotifications

Unregisters from push notifications.

```csharp
public void unregisterForRemoteNotifications()
```
