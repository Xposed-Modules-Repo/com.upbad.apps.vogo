*I don't update my apps too often. Please [let me know](https://github.com/zehuanli/Google-Voice-Mark-Read/issues) if this module stops working on the latest version, and I'll update it.*

# Google Voice Mark Read
Up till now Google Voice does not provide the basic feature to mark messages as read in the notifications. Tired of going into the app and clicking on each unread message every time, I made this Xposed module to add a "mark as read" option to the Google Voice message notifications.

This module has been tested working for the current Google Voice version. It may stop working for the future versions since the package structure may change. However, it shouldn't be hard to tweak the module to support the new versions as long as there's no major change on the notification logics in Google Voice.

# A little bit details
The "mark as read" option utilizes a hidden notification action provided by Google Voice, which is highly likely to be used by Android Auto, since it's inside a bundle named `android.car.EXTENSIONS`. It is *possible* to implement the module without relying on this hidden action, but there definitely will be more reverse engineering work to do.
