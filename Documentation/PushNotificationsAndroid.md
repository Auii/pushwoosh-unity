# class PushNotificationsAndroid #

Provides specific features for Android platform.

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

[public void RegisterForPushNotifications()](#registerforpushnotifications)  
[public void UnregisterForPushNotifications()](#unregisterforpushnotifications)  
[public String[] GetPushHistory()](#getpushhistory)  
[public void ClearPushHistory()](#clearpushhistory)  
[public void StartTrackingBeaconPushes()](#starttrackingbeaconpushes)  
[public void StopTrackingBeaconPushes()](#stoptrackingbeaconpushes)  
[public void ClearLocalNotifications()](#clearlocalnotifications)  
[public int ScheduleLocalNotification(string message, int seconds)](#schedulelocalnotification)  
[public void ClearLocalNotification(int id)](#clearlocalnotification)  
[public void SetMultiNotificationMode()](#setmultinotificationmode)  
[public void SetSimpleNotificationMode()](#setsimplenotificationmode)  
[public void SetSoundNotificationType(int soundNotificationType)](#setsoundnotificationtype)  
[public void SetVibrateNotificationType(int vibrateNotificationType)](#setsoundnotificationtype)  
[public void SetLightScreenOnNotification(bool lightsOn)](#setlightscreenonnotification)  
[public void SetEnableLED(bool ledOn)](#setenableled)  


### RegisterForPushNotifications

Registers for push notifications. Called automatically in `Start` function.

```csharp
public void RegisterForPushNotifications()
```

---
### UnregisterForPushNotifications

Unregisters from push notifications.

```csharp
public void UnregisterForPushNotifications()
```

--
### GetPushHistory

Gets push history for the device (since the last `clearPushHistory` call).

```csharp
public String[] GetPushHistory()
```

--
### ClearPushHistory

Clears push history for the device.

```csharp
public void ClearPushHistory()
```

--
### StartTrackingBeaconPushes

Starts tracking iBeacon Push notifications

```csharp
public void StartTrackingBeaconPushes()
```

--
### StopTrackingBeaconPushes

Stops tracking iBeacon Push notifications

```csharp
public void StopTrackingBeaconPushes()
```

--
### ClearLocalNotifications

Clears all scheduled local notifications.

```csharp
public void ClearLocalNotifications()
```

--
### ScheduleLocalNotification

Schedules local notification.

```csharp
public int ScheduleLocalNotification(string message, int seconds)
public int ScheduleLocalNotification(string message, int seconds, string userdata)
```

* **message** - notification title
* **seconds** - timeout in seconds to display the message
* **userdata** - optional

--
### ClearLocalNotification

Clears specific local notification

```csharp
public void ClearLocalNotification(int id)
```

* **id** - notification id returned from `scheduleLocalNotification` function

--
### SetMultiNotificationMode

Allows multiple notifications in the tray.

```csharp
public void SetMultiNotificationMode()
```

--
### SetSimpleNotificationMode

Allows single notifications in the tray.

```csharp
public void SetSimpleNotificationMode()
```

--
### SetSoundNotificationType

Sets default sound notification type. Could be overriden from Pushwoosh Control Panel.
* 0 - default mode
* 1 - no sound
* 2 - always

```csharp
public void SetSoundNotificationType(int soundNotificationType)
```

--
### SetVibrateNotificationType

Sets default vibration notification type. Could be overriden from Pushwoosh Control Panel.
* 0 - default mode
* 1 - no vibration
* 2 - always

```csharp
public void SetVibrateNotificationType(int vibrateNotificationType)
```

--
### SetLightScreenOnNotification

Should the screen lit up itself when push notification arrives. Could be overriden from Pushwoosh Control Panel.

```csharp
public void SetLightScreenOnNotification(bool lightsOn)
```

--
### SetEnableLED

Enables LED blinking. Could be overriden from Pushwoosh Control Panel.

```csharp
public void SetEnableLED(bool ledOn)
```
