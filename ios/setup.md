---
layout: default
title: Setup
parent: iOS
nav_order: 1
---

If you use Cocoapods you can add Azbouki to your project by adding this to your Podfile:

```
pod `azbouki`
```

Before using the SDK you need to create an Application instance in the dashboard, then use its `id` too initialize the SDK:

```
import azbouki

...

func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
    ...
    AzboukiClient.configure(appId: "<your-app-id>", userId: "<user-id-string>")
    ...
}
```



