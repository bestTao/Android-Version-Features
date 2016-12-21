# Android各个版本的特性--持续更新
## 版本

### Android 2.0

- 增加`onBackPressed()`方法，专门用来back键的事件监听

### Android 4.4

- 沉浸式状态栏

### Android 5.0

- 沉浸式状态栏效果改进

### Android 6.0

- 动态权限

## 功能

### 通知Notification

- API < 11

```java
Notification notification = new Notification(int icon,CharSequence tichkerText,long when);  
```

- API >= 11

```java
Notification notification = new Notification.Builder(mContext)
               .setContentTitle("New mail from " + sender.toString())
               .setContentText(subject)
               .setSmallIcon(R.drawable.new_mail)
               .setLargeIcon(aBitmap)
               .getNotification();
```

其中 当 API >= 16时 构建可以用`build()`代替`getNotification()`
