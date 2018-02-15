# there's a new APP now : go to https://spike-app.com/

connects to xDrip, G5, BluKon and BlueReader
can also work as Follower


xdrip/xbridge/G5/Bluereader/Blukon for iOS devices - 

* Alerts
* Chart
* Always on notification (not really always but almost always) that allows to see the current value by just lifting up the phone.
* Upload to Nightscout
* store values in HealthKit
* upload to Dexcom Share
* speak Bloodglucose readings, languages Dutch, English, French, Portugese, Spanish. If more languages needed send me an e-mail please (xdrip@proximus.be)
* export readings to SiDiary format

* Follower mode : using NightScout, the app can be used in follower mode.

Alerts

Alerts are configured in the Settings. 
Possible alerts are
 * High
 * Very High
 * Low
 * Very Low
 * Missed Reading
 * Phone Muted (warns you if your phone is muted)
 * Calibration Request
 * Battery Low

Each Alert requires an Alert Type.

__Per Alert Type define__
 * enabled or disabled : Example between 8 in the morning and midnight I don't need a low alert. For me the Low alert has a disabled alert type between 8 and midnight. There's
 always an alert named "No Alert" created by the application which is disabled. You can use that one for all cases where you want a disabled alert type.
 * Name : name of the alert type
 * Vibration enabled yes or no : if yes the device will vibrate when the alert goes off
 * Snooze from notification yes or no : if yes, you can do a quick snooze of an alert from the home screen (why would I say 'no' ? because many times during the night when an alarm goes off, I just snooze it and continue sleeping without doing something about my values - if I have to unlock my device for snoozing then I'm sure I'll be awake)
 * Snooze period (in minutes) : value used when you snooze from the home screen
 * Repeat yes or no : it's an iOS thing, if yes the notification will repeat every minute until you open the notification or snooze it. In any case the alert will go off again 5 minutes later if you haven't snoozed it and if it's still applicable
 * Sound : the sound to use. 
   The phone will not generate any sound if it's in silent mode.
   At the time of writing there are three options
   * "No Sound" : you will not hear anything
   * "Default iOS Sound" : the sound generated by iOS
   * "xDrip Sound" : it's a copy of the sound generated by the Android version

__Next step : the Alerts__

For each alert (except 'Always on Notification' and 'Additional Calibration Request'), you can define for each moment of the type which Alert Type needs to be used. 
For example you could say 
* between 00:00 and 08:00, the Low Value alert needs to use an Alert Type with vibration, with the xDrip sound, without a snooze possibility on the home screen.
* between 08:00 and 23:59, the Low Value alert only needs to vibrate, no sound, with a possibility to snooze on the Home Screen.
In such case you would need two Alert Types, and assign each of them to the correct interval.
You can create as many Alert Types and intervals as you want.
Alert Types can be re-used for different types of alerts.



To compile (only if you want to develop):
- install Flash Builder 4.7 with latest FLex SDK (contact me and I'll share you a folder for OSX or Windows)
- If you don't have an iOS developer account, I can create you a certificate that will allow you to compile. Full explanation : http://help.adobe.com/en_US/flex/mobileapps/WS064a3073e805330f6c6abf312e7545f65e-8000.html
- clone the repository
- you will need the native extensions, I can share you the ANE's so send me an e-mail.
