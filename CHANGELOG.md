# v6.0.0

This version is effectively a re-write with the goal of splitting every module into it's own package (simplifies maintenance
for contributors and also installation for users) and bringing each Firebase module up to 100% testing coverage and 100%
Firebase API Coverage.

Many of the manual native installation steps for Android & iOS have been removed / internally automated
and most modules can now be used just by linking it (e.g. `react-native link @react-native-firebase/analytics`).

The following modules are completed and published to NPM and ready to be consumed (as patch versions only, until all modules are ready, at which point they will all be published starting from v6.0.0):

| Name                                                     |                                                                                            Downloads                                                                                            |                                                                Coverage                                                                 |
| -------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------: |
| [Analytics](/packages/analytics)                         |           [![badge](https://img.shields.io/npm/dm/@react-native-firebase/analytics.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/analytics)           |           [![badge](https://api.rnfirebase.io/coverage/analytics/badge)](https://api.rnfirebase.io/coverage/analytics/detail)           |
| [App](/packages/app)                                     |                 [![badge](https://img.shields.io/npm/dm/@react-native-firebase/app.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/app)                 |                 [![badge](https://api.rnfirebase.io/coverage/app/badge)](https://api.rnfirebase.io/coverage/app/detail)                 |
| [App Indexing](/packages/indexing)                       |            [![badge](https://img.shields.io/npm/dm/@react-native-firebase/indexing.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/indexing)            |            [![badge](https://api.rnfirebase.io/coverage/indexing/badge)](https://api.rnfirebase.io/coverage/indexing/detail)            |
| [Cloud Functions](/packages/functions)                   |           [![badge](https://img.shields.io/npm/dm/@react-native-firebase/functions.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/functions)           |           [![badge](https://api.rnfirebase.io/coverage/functions/badge)](https://api.rnfirebase.io/coverage/functions/detail)           |
| [Cloud Firestore](/packages/firestore)                   |           [![badge](https://img.shields.io/npm/dm/@react-native-firebase/firestore.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/firestore)           |           [![badge](https://api.rnfirebase.io/coverage/firestore/badge)](https://api.rnfirebase.io/coverage/firestore/detail)           |
| [Cloud Storage](/packages/storage)                       |             [![badge](https://img.shields.io/npm/dm/@react-native-firebase/storage.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/storage)             |             [![badge](https://api.rnfirebase.io/coverage/storage/badge)](https://api.rnfirebase.io/coverage/storage/detail)             |
| [Cloud Messaging](/packages/messaging)                   |           [![badge](https://img.shields.io/npm/dm/@react-native-firebase/messaging.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/messaging)           |           [![badge](https://api.rnfirebase.io/coverage/messaging/badge)](https://api.rnfirebase.io/coverage/messaging/detail)           |
| [Crashlytics](/packages/crashlytics)                     |         [![badge](https://img.shields.io/npm/dm/@react-native-firebase/crashlytics.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/crashlytics)         |         [![badge](https://api.rnfirebase.io/coverage/crashlytics/badge)](https://api.rnfirebase.io/coverage/crashlytics/detail)         |
| [Dynamic Links](/packages/dynamic-links)                 |       [![badge](https://img.shields.io/npm/dm/@react-native-firebase/dynamic-links.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/dynamic-links)       |       [![badge](https://api.rnfirebase.io/coverage/dynamic-links/badge)](https://api.rnfirebase.io/coverage/dynamic-links/detail)       |
| [In-app Messaging](/packages/in-app-messaging)           |    [![badge](https://img.shields.io/npm/dm/@react-native-firebase/in-app-messaging.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/in-app-messaging)    |    [![badge](https://api.rnfirebase.io/coverage/in-app-messaging/badge)](https://api.rnfirebase.io/coverage/in-app-messaging/detail)    |
| [Instance ID](/packages/iid)                             |                 [![badge](https://img.shields.io/npm/dm/@react-native-firebase/iid.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/iid)                 |                 [![badge](https://api.rnfirebase.io/coverage/iid/badge)](https://api.rnfirebase.io/coverage/iid/detail)                 |
| [ML Kit Natural Language](/packages/ml-natural-language) | [![badge](https://img.shields.io/npm/dm/@react-native-firebase/ml-natural-language.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/ml-natural-language) | [![badge](https://api.rnfirebase.io/coverage/ml-natural-language/badge)](https://api.rnfirebase.io/coverage/ml-natural-language/detail) |
| [ML Kit Vision ](/packages/ml-vision)                    |           [![badge](https://img.shields.io/npm/dm/@react-native-firebase/ml-vision.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/ml-vision)           |           [![badge](https://api.rnfirebase.io/coverage/ml-vision/badge)](https://api.rnfirebase.io/coverage/ml-vision/detail)           |
| [Performance Monitoring](/packages/perf)                 |                [![badge](https://img.shields.io/npm/dm/@react-native-firebase/perf.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/perf)                |                [![badge](https://api.rnfirebase.io/coverage/perf/badge)](https://api.rnfirebase.io/coverage/perf/detail)                |
| [Realtime Database](/packages/database)                  |            [![badge](https://img.shields.io/npm/dm/@react-native-firebase/database.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/database)            |            [![badge](https://api.rnfirebase.io/coverage/database/badge)](https://api.rnfirebase.io/coverage/database/detail)            |
| [Remote Config](/packages/remote-config)                 |       [![badge](https://img.shields.io/npm/dm/@react-native-firebase/remote-config.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/remote-config)       |       [![badge](https://api.rnfirebase.io/coverage/remote-config/badge)](https://api.rnfirebase.io/coverage/remote-config/detail)       |
| [Utils](/packages/utils)                                 |               [![badge](https://img.shields.io/npm/dm/@react-native-firebase/utils.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/utils)               |               [![badge](https://api.rnfirebase.io/coverage/utils/badge)](https://api.rnfirebase.io/coverage/utils/detail)               |

---

The following modules are currently **migration only** for now (migrated from v5 to v6 with minimal changes), what this means:

- no new work done on them (other than migrating to v6 internals)
- no new tests added for them (but all existing tests pass)
- flow types missing (but have TS types)

More work on these will be done in a later pre-v6 release.

| Name                             |                                                                             Downloads                                                                             |                                                 Coverage                                                  |
| -------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| [Authentication](/packages/auth) | [![badge](https://img.shields.io/npm/dm/@react-native-firebase/auth.svg?style=for-the-badge&logo=npm)](https://www.npmjs.com/package/@react-native-firebase/auth) | [![badge](https://api.rnfirebase.io/coverage/auth/badge)](https://api.rnfirebase.io/coverage/auth/detail) |

> If a module you use is not yet listed above please refrain from using v6 for now - attempting to use v6 alongside v5 can cause issues with dependencies.

Please tag any GitHub issues regarding v6 with `[v6]` in the title.

## Migrating from v4 & v5

With the size of the changes mentioned above, it's recommended that you remove all native code/changes previously added
for `react-native-firebase` (except for firebase initialisation code (e.g. `[FIRApp configure];` ios, `apply plugin: 'com.google.gms.google-services'` android).

Additionally, it's recommended to remove any native Firebase dependencies (the Firebase Android/iOS SDKs) in your iOS
`Podfile` and your `android/app/build.gradle` file, e.g. `pod 'Firebase/Core', '~> 5.15.0'` or `implementation "com.google.firebase:firebase-core:16.`,
as we now manage these dependencies and their versions internally.

Once all the old native installation changes have been removed you can follow the install guide below.

> If you're migrating from v4, please ensure you've read up on any breaking changes from v4 to v5 [here](https://rnfirebase.io/docs/v5.x.x/releases/v5.0.0).

### Installing

1. Install the [@react-native-firebase/app](https://github.com/invertase/react-native-firebase/tree/master/packages/app) NPM package (all modules have a hard dependency requirement on this package):

```bash
yarn add @react-native-firebase/app
react-native link @react-native-firebase/app
```

2. Install the NPM packages for the Firebase services you'd like to use, e.g. for analytics install [@react-native-firebase/analytics](https://github.com/invertase/react-native-firebase/tree/master/packages/analytics). Repeat this step for each Firebase service you require.

```bash
yarn add @react-native-firebase/analytics
react-native link @react-native-firebase/analytics
```

3. Some Firebase services such as Performance Monitoring require some minor additional native code steps for Android or iOS that can't be abstracted away, e.g. Perf on Android requires the `com.google.firebase.firebase-perf` gradle plugin. Please see the readme for each module (see the table above for links) where these changes are documented; these will later be moved to the new documentation hub.

#### Usage Example

```js
// import the app module
import firebase from '@react-native-firebase/app';

// import the modules you'd like to use
import '@react-native-firebase/analytics';
import '@react-native-firebase/functions';

// use them
await firebase.analytics().setUserId('12345678');
```

Optionally; you can also consume a module directly without needing the default export of `@react-native-firebase/app`, e.g.:

```js
import { firebase } from '@react-native-firebase/analytics';

// use analytics
await firebase.analytics().setUserId('12345678');

// ---- OR ----
import analytics from '@react-native-firebase/analytics';

// use analytics
await analytics().setUserId('12345678');
```

## All Modules

- [INTERNAL] Improved error codes & handling for all Firebase services;
  - Standardised native error to JS conversion
  - [DEVEX] Native promise rejection errors now contain additional properties to aid debugging
  - All React Native Firebase native methods should now always return an Error to JS - even if the Error occurred due to native code.
- [BUGFIX] All native events are now queued natively until a JS listener is registered. This fixes several race conditions for events like `onMessage`, `onNotification`, `onLink` etc where the event would trigger before JS was ready.
- [NEW][🔥] In an effort to further reduce manual native code changes when integrating and configuring React Native Firebase; we have added support for configuring various Firebase services & features via a `firebase.json` file in your project root.
- [NEW][ios] CocoaPods static framework support for all modules (you can use `use_frameworks!` without issues relating to this lib)
- [NEW][ios] Implemented a CocoaPods Firebase React Native modules auto-loader script for your Podfile; you only need to change your Podfile once (to add the script); this script will then automatically include all React Native Firebase modules found in your `node_modules` directory as Pods, manage additional required build phases (e.g. auto adds the crashlytics build phase (`/Fabric/Run`)), and allows the `firebase.json` functionality to work. [Example Podfile](https://github.com/invertase/react-native-firebase/blob/master/tests/ios/Podfile) with script included and sample `pod install` logs:
  ![pod install image](https://i.imgur.com/XOqw5Jq.png)

---

## App (app)

- [NEW] Added `appConfig` & method support for `setAutomaticDataCollectionEnabled` & `automaticResourceManagement`
- [NEW] Added app `options` support for `gaTrackingId`
- [NEW] The `[DEFAULT]` Firebase app can now be safely initialised in JS, however this has some caveats;
  - Firebase services such as Performance Monitoring & Remote Config require the default app to be initialised through the plist/json file.
- [BREAKING] Waiting for apps to init via `.onReady()` has been removed. `initializeApp()` now returns a promise to the same effect
- [BREAKING] Trying to initialise the `[DEFAULT]` Firebase app in JS when it was already initialised natively will now throw an error (formerly warned)

---

### AdMob (WIP)

AdMob has undergone a full rewrite to keep up-to-date with the latest changes and APIs. The JavaScript API interface has been modified from v5 to provider a simpler, cleaner way to manage ads.

- [NEW] A new `AdsConsent` helper has been added to handle user ads consent, required under GDPR regulations. See the [documentation](https://invertase.io/oss/react-native-firebase/v6/admob/european-user-consent) for more information.
- [NEW] Global settings can be applied to AdMob via `setRequestConfiguration`.
  - `maxAdContentRating`, `tagForChildDirectedTreatment` & `tagForUnderAgeOfConsent` are now set a global configuration settings.
- [NEW] `RewardedAd` interface used the new Google Mobile Ads SDK beta API. Rewarded ads can now be controlled from the user dashboard, supporting both video and interactive ads.
- [NEW] Added support for requesting only non-personalized ads via the `requestNonPersonalizedAdsOnly` request options.
- [NEW] Added support for custom network extras on ad requests via `networkExtras`.
  - The user reward is now pre-fetched when the ad is loaded.
- [BREAKING] The API interface for interacting with AdMob has undergone a full re-write.
- [BUGFIX] Ads can now work during React Native debugging. 

---

## App Indexing (indexing) - **[NEW]**

Support for handling an incoming app index URL has been added to React Native Firebase.

- [NEW] Handle the app opening via an app indexing URL with `indexing().getInitialURL()`.
- [NEW] Setup a realtime event listener to handle app indexing URL opening whilst the app is active with `indexing().onOpenURL()`.

> Support for Android events will be integrated post-v6 release. For now this is purely a wrapper around `Linking` in React Native.

## App Invites (invites)

- [BREAKING] this module has been deprecated by Firebase and now been removed, you should migrate to Dynamic Links.

---

## Analytics (analytics)

- [NEW] Added support for `resetAnalyticsData()`
- [INTERNAL] `setUserProperties` now iterates properties natively (formerly 1 native call per property)
- [BREAKING] all analytics methods now return a Promise, rather than formerly being 'fire and forget'

---

## Crashlytics (crashlytics)

> **Blog post announcement**: [[Firebase Crashlytics for React Native](https://invertase.io/blog/firebase-crashlytics-for-react-native?utm_source=github&utm_medium=changelog)]

- [NEW] JavaScript stack traces now automatically captured and parsed
  ![js stack trace preview](https://pbs.twimg.com/media/D07RPDMW0AA7TTv.jpg:large)
- [NEW] Optionally enable automatic reporting of JavaScript unhandled Promise rejections
- [NEW] Added support for `setUserName(userName: string)`
- [NEW] Added support for `setUserEmail(userEmail: string)`
- [NEW] Added support for `isCrashlyticsCollectionEnabled: boolean`
- [NEW][android] Added support for [Crashlytics NDK](https://docs.fabric.io/android/crashlytics/ndk.html#using-gradle) reporting. This allows Crashlytics to capture Yoga related crashes generated from React Native.
- [NEW][🔥] Added `firebase.json` support for `crashlytics_ndk_enabled`, this toggles NDK support as mentioned above, defaults to `true`
- [NEW][🔥] Added `firebase.json` support for `crashlytics_debug_enabled`, this toggles Crashlytics native debug logging, defaults to `false`
- [NEW][🔥] Added `firebase.json` support for `crashlytics_auto_collection_enabled`, this toggles Crashlytics error reporting, this is useful for user opt-in first flows, e.g. set to `false` and when your user agrees to opt-in then call `setCrashlyticsCollectionEnabled(true)` in your app, defaults to `true`
- [BUGFIX][android] `crash()` now correctly crashes without being caught by React Native's RedBox
- [BREAKING] `setBoolValue`, `setFloatValue`, `setIntValue` & `setStringValue` have been removed and replaced with two new methods (the Crashlytics SDK converted all these into strings internally anyway):
  - `setAttribute(key: string, value: string): Promise<null>` - set a singular key value to show alongside any subsequent crash reports
  - `setAttributes(values: { [key: string]: string }): Promise<null>` - set multiple key values to show alongside any subsequent crash reports
- [BREAKING] all methods except `crash`, `log` & `recordError` now return a `Promise` that resolves when complete
- [BREAKING] `recordError(code: number, message: string)`'s fn signature changed to `recordError(error: Error)` - now accepts a JS Error class instance
- [BREAKING] `setUserIdentifier()` has been renamed to `setUserId()` to match analytics implementation
- [BREAKING] `enableCrashlyticsCollection()`'s fn signature changed to `setCrashlyticsCollectionEnabled(enabled: boolean)`
  - This can be used in all scenarios (formerly only able to use this when automatic initialization of crashlytics was disabled)
  - Changes do not take effect until the next app startup
  - This persists between app restarts and only needs to be called once, can be used in conjunction with `isCrashlyticsCollectionEnabled` to reduce bridge startup traffic - though calling multiple times is still allowed

---

## Cloud Firestore (firestore)

Cloud Firestore has undergone a complete overhaul of both JavaScript & native code, including a re-write of bridge serialisation, support for new features & heavy test coverage.

- [NEW] Added support for collection group queries (`firestore().collectionGroup()`).
- [NEW] Added support for `isEqual()` across most classes.
- [NEW] Added support for `SetOptions.mergeFields` (`DocumentReference.set()` / `Transaction.set()`).
- [NEW] Added support for handling snapshot metadata via the `includeMetadataChanges` flag which can be passed to `CollectionReference.onSnapshot()` and `QuerySnapshot.docChanges()` to return additional results from query snapshot listeners.
- [NEW] Cache size can now be set to unlimited using the `CACHE_SIZE_UNLIMITED` static when passed to `firestore().settings()` (also added in v5.4).
- [BUGFIX] Remove Metro circular reference warnings.
- [BUGFIX] `DocumentReference` and `CollectionReference` snapshot observers now correctly handle the same args as the Web SDK.
- [BUGFIX] Validate transaction gets must also have a write command (matches Web SDK).
- [BUGFIX] Setting a negative infinity value (`-Infinity`) now correctly works as expected.
- [BUGFIX] `QuerySnapshot.forEach()` can now correctly takes an optional context argument.
- [BUGFIX] Snapshot metadata now correctly returns a `SnapshotMetadata` class (as per Web SDK).
- [BUGFIX] `CollectionReference` now correctly extends a `Query` class. In v5 it is possible to chain calls from `Query` → `CollectionReference` which isn't possible on the Web SDK.
- [BUGFIX] `onSnapshot()` calls now take the correct arguments, allowing for `SnapshotListenOptions`, inline function callbacks or an object containing next/error callbacks (as per the Web SDK).
- [BUGFIX] Setting a `Date` on Firestore was setting an incorrect value. Date objects are now converted to a `Timestamp` as per the Web SDK.
- [BUGFIX] Cursor queries in v5 (`startAt`, `startAfter`, `endAt`, `endBefore`) were incorrectly handling a `DocumentSnapshot` argument. It is now possible to perform a cursor query directly on a snapshot, or on snapshot fields, as per the Web SDK, for example ending at a specific snapshot with no order.
- [BREAKING] Blob can no longer be constructed manually, as per the Web SDK.
- [BREAKING] The v6 release includes **a lot** of additional JavaScript validation. This is more consistent with the Web SDK and helps catch native errors/crashes which may occur due to false-positive data being sent over the bridge.
  - Specifically, the `Query` class has undergone a rewrite, and includes a lot of additional checks which are not present in v5. Please check your Firestore queries once upgraded.
- [BREAKING] Removed the `Query.where` single equals operator (`=`) as per the Web SDK. Use `==` instead.
- [BREAKING] previously deprecated `setTimestampsInSnapshotsEnabled` on settings has now been removed.
- [PERFORMANCE][🔥] [ANDROID] Data serialisation logic is now correctly performed off the main UI thread. This will help increase performance and reduce activity on the UI thread when sending large volumes of data to Firestore and back to the device.
- [PERFORMANCE][🔥] The data serialisation logic has undergone a large rewrite for performance.
  - JavaScript data being sent over the native bridge has to be converted to it's native counterpart, and visa versa. When dealing with a large number of documents and/or large amounts document data, this process can be both time consuming and resource intensive. The rewrite keeps data being sent over the bridge at a minimum; mapping data types to smaller serialisation format that can be parsed by JS and Native code.
  - Sample comparisons against v5 have shown:
    - Data size sent over the bridge has been reduced by ~58%.
    - On large queries (4x documents with 1500 nested array items (containing all data types)) are over ~50% faster on v6. Smaller queries (1x document with 1500 nested array items) are over ~15% quicker.

---

## Dynamic Links (dynamicLinks)

- [BREAKING] the namespace for this module has changed, replace all usages of `firebase.links()` with `firebase.dynamicLinks()`
- [BREAKING] `onLink` & `getInitialLink` now return a `DynamicLink` object with multiple properties, formally just provided just the url as a string
- [NEW][ios][🔥] Manually adding `AppDelegate` methods to support receiving Dynamic Link open events is no longer required, we swizzle this at runtime and automatically intercept the required events.
- [BUGFIX] Links should now always be accessible via `onLink` & `getInitialLink`
  - This fix is a 'side-effect' of the bugfix mentioned above in the `all modules` section ('`All native events are now queued natively`')
- [BREAKING] Creating a Dynamic Link builder via `new firebase.links.DynamicLink(link, domainURIPrefix)` has been deprecated, use a plain object instead as an arg for `buildLink()` & `buildShortLink()`.
- [BREAKING] Some previously allowed parameter configurations will now throw an argument error, e.g. trying to set any `DynamicLinkIOSParameters` param without providing an iOS bundle id will now error.
  - these configurations were incorrect to begin with but were never flagged to user code so may have gone unnoticed

---

## Functions (functions)

- [BUGFIX] Fixed an issue where `useFunctionsEmulator` does not persist natively (Firebase iOS SDK requires chaining this method before other calls and does not modify the instance, Android however persists this)

---

## In-App Messaging (inAppMessaging) - **[NEW]**

- [NEW] Added support for `firebase.inAppMessaging().isMessagesDisplaySuppressed: boolean;`
- [NEW] Added support for `firebase.inAppMessaging().setMessagesDisplaySuppressed(enabled: boolean): Promise<null>;`
- [NEW] Added support for `firebase.inAppMessaging().isAutomaticDataCollectionEnabled: boolean;`
- [NEW] Added support for `firebase.inAppMessaging().setAutomaticDataCollectionEnabled(enabled: boolean): Promise<null>;`

---

## Instance Id (iid)

- [NEW] Instance Id now supports multiple Firebase apps, e.g. `firebase.app('fooApp').iid().get()`

---

## Cloud Messaging (messaging)

- [NEW] added support for `onSendError` events, an event that indicates a message (with id) failed to send
- [NEW] added support for `onMessageSent` events, an event that indicates a message (with id) was successfully sent
- [NEW] added support for `onDeletedMessages` events, an event that indicates the FCM server deleted pending messages
  - when your app instance receives this event, it should perform a full sync with your app server if it relies on message data
- [NEW] `getToken` & `deleteToken` now optionally support `authorizedEntity` & `scope` arguments
  - `authorizedEntity` - defaults to `firebase.app().options.messagingSenderId`
  - `scope` - defaults to `FCM`
- [NEW][ios] added support for `isRegisteredForRemoteNotifications: boolean;`
- [NEW][ios] added support for `unregisterForRemoteNotifications(): Promise<void>;`
- [NEW][ios] `requestPermission` on iOS 12+ devices now uses the `UNAuthorizationOptionProvisional` option to request permission
  - this allows you to immediately start sending 'quiet' notifications to your users without their explicit permission, i.e., on a trial basis. `requestPermission` with this option will no longer show a permission request dialog to your user. [Learn More](http://iosbrain.com/blog/2018/07/05/new-in-ios-12-implementing-provisional-authorization-for-quiet-notifications-in-swift/)
  - [[WWDC 2018 Video]](https://developer.apple.com/videos/play/wwdc2018/710/) (30:00 onwards)
- [NEW] added support for `isAutoInitEnabled: boolean;`
- [NEW] added support for `setAutoInitEnabled(enabled: boolean): Promise<void>;`
- [NEW] added support for disabling messaging auto initialisation via the new `firebase.json` configuration file
  - `messaging_auto_init_enabled`: `true/false`
- [NEW][android] added support for configuring the background Headless task timeout via the new `firebase.json` configuration file
  - `messaging_android_headless_task_timeout`: `number` - milliseconds
- [NEW][android] added support for registering the background message headless task via `firebase.messaging().setBackgroundMessageHandler(handler: Function)`
- [BREAKING][android] manually registering the background message headless task handler via `AppRegistry.registerHeadlessTask` is no longer supported. Call `firebase.messaging().setBackgroundMessageHandler(handler: Function)` instead.
  - This is a pre-emptive change that will allow us to support background tasks for iOS in a future release (as it won't be via RN Headless Tasks as it's not supported on iOS)
- [BREAKING][android] the manually added `RNFirebaseMessagingService` service in your `AndroidManifest.xml` file is no longer required - you can safely remove it.
  - Many manual code changes that existed in v5 are now automatically handled for you in v6
- [BREAKING][ios] any the manually added `AppDelegate.m` changes for messaging on v5 are longer required - you can safely remove them (search for `RNFirebaseMessaging` in your `AppDelegate`)
  - Many manual code changes that existed in v5 are now automatically handled for you in v6
- [BREAKING] constructing a `RemoteMessage` instance via `new firebase.messaging.RemoteMessage()` is no longer supported, use `firebase.messaging().newRemoteMessage()` to retrieve an new remote message builder instance.
- [BREAKING][ios] the minimum supported iOS version is now 10

  - iOS 9 or lower only accounts for 0.% of all iPhone devices
  - to see a detailed device versions breakdown see [this link](https://david-smith.org/iosversionstats/)
  - community contributions that add iOS 9 support are welcome

---

## Performance Monitoring (perf)

The Performance Monitoring API has had a significant API change as originally highlighted would happen in the v5.x.x docs:
![image](https://user-images.githubusercontent.com/5347038/58876674-b633b780-86c6-11e9-8a74-6b6194c8ab05.png)

- [BREAKING] All `Trace` & `HttpMetric` methods (except for `start` & `stop`) are now synchronous and no longer return a Promise, extra attributes/metrics now only get sent to native when you call `stop`
- [BREAKING] `firebase.perf.Trace.incrementMetric` will now create a metric if it could not be found
- [BREAKING] `firebase.perf.Trace.getMetric` will now return 0 if a metric could not be found
- [NEW] Added support for `firebase.perf().isPerformanceCollectionEnabled: boolean`
- [NEW] Added `firebase.perf().startTrace(identifier: string): Promise<Trace>;` as a convenience method to create and immediately start a Trace

---

## Realtime Database (database)

The Realtime Database module has had a large re-write, fixing various inconsistencies against the web SDK, along with improving data serialization on the native side by moving intensive serialization work off the UI thread.

- [BREAKING][bugfix] The `Reference` class now extends a `Query` class (to match the web SDK). Currently in v5 everything is within the `Reference` class, allowing for incorrect behaviour such as chaining a reference only method to a query, e.g. `ref().orderByKey().once()`. This is now not possible and will cause a standard JavaScript error.
- [BREAKING][bugfix] Internal validation for all methods has now been added. With v5 in some cases, incorrect values would be passed along to native and causing native exceptions/potential crashes.
- [BREAKING][bugfix] All query based modifiers are now validated as per the Web SDK spec. In v5 it is possible to chain queries which are not allowed together causing native errors (e.g. `.orderByKey().orderByPriority()`, `.startAt('foo', 'bar').orderByKey()` etc). Doing so in v6 will now throw an error to keep it in-line with the Web SDK.
- [BREAKING][bugfix] `Reference.push` now correctly mimics the Web SDK, returning a thenable reference.
- [NEW] `DatabaseSnapshot.forEach` now returns the current index key.
- [NEW] Many methods were missing an `onComplete` handler, which is now implemented as per the Web SDK.
- [BUGFIX] `DatabaseSnapshot.forEach` correct iterates over "array" fields in the database.

---

## Remote Config (remoteConfig)

The Remote Config API has had a significant API change as originally highlighted would happen in the v5.x.x docs:
![image](https://user-images.githubusercontent.com/5347038/58876587-7c62b100-86c6-11e9-81f9-95c26e1485a1.png)

- [BREAKING] Module namespace has been renamed to `.remoteConfig()`, replace all usages of `firebase.config` with the new name.
- [BREAKING] All Remote Config values can now be accessed synchronously in JS, see `getValue(key: string): ConfigValue` & `getAll(): ConfigValues` below
  - [BREAKING] These replace all the original async methods: `getValue`, `getValues`, `getKeysByPrefix`
- [BREAKING] `setDefaultsFromResource` now returns a Promise that resolves when completed, this will reject with code `config/resouce_not_found` if the file could not be found
- [BREAKING] `setDefaultsFromResource` now expects a resource file name for Android to match iOS, formerly this required a resource id (something you would not have in RN as this was generated at build time by Android)
  - And example for both platforms can be found in the tests. We'll writeup up a guide for this at some point to show how to use the plist/xml defaults files on each platform.
- [BREAKING] `enableDeveloperMode` has been removed, you can now use `setConfigSettings({ isDeveloperModeEnabled: boolean })` instead
- [BREAKING] `setDefaults` now returns a Promise that resolves when completed
- [NEW] Added a new `fetchAndActivate` method - this fetches the config and activates it without the need to call `activate()` separately
- [NEW] Added the following properties to `firebase.remoteConfig()`; `lastFetchTime`, `lastFetchStatus` & `isDeveloperModeEnabled`
- [NEW] Added a new `setConfigSettings` method - this allows setting `isDeveloperModeEnabled`, replaces the `enableDeveloperMode` method
  - This is a generic settings function to pre-emotively account for an upcoming future change to the native sdks - more settings to be added.
- [NEW] All previous `get*` methods have been removed and replaced with 2 synchronous methods:
  - `getValue(key: string): ConfigValue` - returns a single configuration value `{ value, source }`
  - `getAll(): ConfigValues` - returns all configuration values e.g. `{ some_key: { value, source }, other_key: { value, source } }`

> **Note**: Multi-apps is not yet supported as the Firebase iOS SDK is missing support for it.

---

## Cloud Storage (storage)

<!-- TODO(salakar) change link -->

> **Blog post announcement (NOT LIVE YET)**: [[Firebase Cloud Storage for React Native](https://invertase.io/blog?utm_source=github&utm_medium=changelog)]

- [NEW] Added support for `put` (`Blob` | `ArrayBuffer` | `Uint8Array`)
  - `contentType` mime type is automatically inferred from `Blob`
- [NEW] Added support for `putString` and all StringFormat's (raw, base64, base64url & data_url)
  - `contentType` mime type is automatically inferred from `data_url` strings
- [NEW] Added support multiple buckets, e.g. `firebase.app().storage('gs://my-other-bucket')`
- [NEW] Added support `pause()`, `resume()` & `cancel()` for Upload & Download Storage tasks
- [NEW] Added an `error` property to TaskSnapshot's for `error` state events - this is an instance of `NativeFirebaseError` (with `code` & `message`)
- [NEW] Added support for `StorageReference.list()` & `StorageReference.listAll()`.
- [BREAKING] Removed formerly deprecated `UploadTaskSnapshot.downloadUrl` property, use `StorageReference.getDownloadURL(): Promise<string>` instead
- [BREAKING] `StorageReference.downloadFile()` is now deprecated and will be removed in a later release, please rename usages of this to `writeToFile()` - renamed to match Native SDKs
- [BREAKING] `firebase.storage.Native` has moved to `firebase.utils.Native`
- [BREAKING] `firebase.utils.Native` is now deprecated and will be removed in a later release, please rename usages of this to `firebase.utils.FilePath`
- [BREAKING] `firebase.utils.Native.*` some properties have been renamed and deprecated and will be removed in a later release, follow the in-app console warnings on how to migrate
- [BUGFIX][android] Update/set metadata now correctly supports removing metadata values by passing a null property value in `customMetadata`
- [BUGFIX][android] `contentType` mime type is now correctly determined in all scenarios, there was an edge case where it would just use the default value
- [INTERNAL][android] `downloadFile` no longer uses a `StreamDownloadTask`, replaced with the newer `FileDownloadTask`

---

## ML Kit Natural Language (naturalLanguage) - **[NEW]**

- [NEW] Implemented support for language identification APIs
  - Single Languages: `identifyLanguage()`.
  - Multiple Languages: `identifyPossibleLanguages()`
- [NEW] Implemented support for [Smart Replies](https://firebase.google.com/docs/ml-kit/generate-smart-replies)
  - [Example Video](https://twitter.com/mikediarmid/status/1128837402481635331)

> ML Kit Translate APIs to come in a later release.

---

## ML Kit Vision (vision) - **[NEW]**

- [NEW] Implemented support for [Text Recognition](https://firebase.google.com/docs/ml-kit/recognize-text) Vision APIs;
  - [x] Cloud
  - [x] On Device
- [NEW] Implemented support for [Document Text Recognition](https://firebase.google.com/docs/ml-kit/recognize-text) Vision APIs;
  - [x] Cloud
- [NEW] Implemented support for [Face Detection](https://firebase.google.com/docs/ml-kit/detect-faces) Vision APIs;
  - [x] On Device
- [NEW] Implemented support for [Barcode Detection](https://firebase.google.com/docs/ml-kit/read-barcodes) Vision APIs;
  - [x] On Device
- [NEW] Implemented support for [Image Labelling](https://firebase.google.com/docs/ml-kit/label-images) Vision APIs;
  - [x] Cloud
  - [x] On Device
- [NEW] Implemented support for [Landmark Recognition](https://firebase.google.com/docs/ml-kit/recognize-landmarks) Vision APIs;
  - [x] Cloud

---

## Utils

- [NEW] Added support via `isRunningInTestLab` for checking if an Android application is running inside a Firebase Test Lab environment
- [NEW] Added a new `FilePath` utility that provides common file paths on the device, see `firebase.utils.FilePath` docs for more info, this is the replacement API for `firebase.storage.Native`
