**Smallest problem possible** :

**Sending data from one android phone to another** :

| S.No. | Task | Description | Link |
| --- | --- | --- | --- |
| 1 |
- Get the GPS (latitude,longitude) co-ordinates of the android device
  | Google Android Developer resources | **STEPS LINK** : [https://developer.android.com/guide/topics/location/strategies.html#BestPerformance](https://developer.android.com/guide/topics/location/strategies.html#BestPerformance) |
|   |   | Sample Code that does the trick | [http://www.androidauthority.com/get-use-location-data-android-app-625012/](http://www.androidauthority.com/get-use-location-data-android-app-625012/)  [http://javapapers.com/android/get-current-location-in-android/](http://javapapers.com/android/get-current-location-in-android/)(GOOD   [http://www.androidhive.info/2015/02/android-location-api-using-google-play-services/](http://www.androidhive.info/2015/02/android-location-api-using-google-play-services/)(good.)  [https://www.quora.com/How-can-I-get-my-location-latitude-longitude-using-Location-Manager-in-Android-Studio](https://www.quora.com/How-can-I-get-my-location-latitude-longitude-using-Location-Manager-in-Android-Studio)(looks pretty good &amp; easy..) – START WITH EASY …here..  |
|   |   |   | [http://stackoverflow.com/questions/17519198/how-to-get-the-current-location-latitude-and-longitude-in-android](http://stackoverflow.com/questions/17519198/how-to-get-the-current-location-latitude-and-longitude-in-android)(Go to 2
# nd
 answer..) [https://developers.google.com/android/reference/com/google/android/gms/location/FusedLocationProviderApi#getLastLocation(com.google.android.gms.common.api.GoogleApiClient)](https://developers.google.com/android/reference/com/google/android/gms/location/FusedLocationProviderApi#getLastLocation(com.google.android.gms.common.api.GoogleApiClient))(latest version…) |
| 2 |
- Send the data collected from the OS of the android device to another android device via. GSM/GPRS?
 |   | Adf |
|   |
-
 |   | [http://stackoverflow.com/questions/8797613/how-to-send-data-from-one-android-device-to-another](http://stackoverflow.com/questions/8797613/how-to-send-data-from-one-android-device-to-another)  [http://stackoverflow.com/questions/30989859/is-there-any-way-to-transfer-data-over-gsm-without-sim](http://stackoverflow.com/questions/30989859/is-there-any-way-to-transfer-data-over-gsm-without-sim)  [http://stackoverflow.com/questions/16244663/is-gsm-data-sending-between-2-phones-impossible](http://stackoverflow.com/questions/16244663/is-gsm-data-sending-between-2-phones-impossible)(This looks pretty good…also use vehicle tracking check solution &amp; see..) [https://www.reddit.com/r/androiddev/comments/364ktz/is\_it\_possible\_to\_send\_data\_between\_2\_phones/?st=iyl4ncq8&amp;sh=6ba3e8c2](https://www.reddit.com/r/androiddev/comments/364ktz/is_it_possible_to_send_data_between_2_phones/?st=iyl4ncq8&amp;sh=6ba3e8c2)  [http://security.stackexchange.com/questions/82238/is-there-any-secure-way-to-transfer-data-between-mobile-phones-without-internet](http://security.stackexchange.com/questions/82238/is-there-any-secure-way-to-transfer-data-between-mobile-phones-without-internet)(advanced..avolid for now) [http://stackoverflow.com/questions/7153501/send-data-over-gsm-radio](http://stackoverflow.com/questions/7153501/send-data-over-gsm-radio)(Try SMS??) |

**NOTE** : Lower priority – check whether android network location or gps is more accurate – alternatively you might check whether IRNSS /NAVIC is available.

START w. GPS – base.

N/w location provider is specialized for indoor use…it returns nearest tower – whereas uses GPS service … so GPS is most optimal &amp; accurate for My context/application

NAVIC – requires special receiver hardware on phone…which is not yet commercially available – so not in current pjt scope.

**STEPS for GPS co-ordinates** :

1. Add classes – location Manager, location Listener
2. Define callback methods for location Listener that location Manager will call whenever there is a change in the location
3. Register the location Listener with the Manager
4. Add permissions to manifest file. (access coarse\_location or fine\_location &amp; the hardware permission)

**Note** : Add hardware permission if you&#39;re targeting android device w. 5.0 +
