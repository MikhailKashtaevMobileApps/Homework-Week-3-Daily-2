# Homework-Week-3-Daily-2

Broadcast Receivers
There are 2 types of Broadcast Receivers. First is manifest declared and the other is registered in context. These are used to get notifified when a system wide event occurs or you can create your own broadcasts within your application. Also you can set permissions for your broadcast to receive or to send with certain parameters. For application wide broadcasts you can use LocalBroadcastManager from the Support Library. Context declaration of the broadcast receiver is preferred. Do not broadcast sensitive information via broadcast because other apps can read it. The namespace for broadcast actions is global and therefore special care is needed when choosing name of action. onReceive() method runs on the main thread and therefore should not be computationally intensive.

Services
Services can perform long tasks in the background and they can persist indefinitely. There are 3 types of services: Foreground, Background, Bound. If the system kills the service, you can choose what to do with it using flags: START_NOT_STICKY(To not restart the service), START_STICKY(To restart the service without last intent), START_REDELIVER_INTENT(To restart the service with the last intent). Services have their own lifecycle and therefore should be killed by themselves with stopSelf() method.
