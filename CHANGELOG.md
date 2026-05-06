## 1.2.2 (6 May 2026)

* feat: persistent console-log session storage — logs are stored across page navigations via a native Android bridge (`window.ErudaAndroid`) and replayed into eruda's console on each page load
* feat: eruda script caching — the eruda CDN script is cached in the app's internal storage with a 7-day TTL and served locally to eliminate repeated network downloads; stale cache is used as a fallback when the network is unavailable

## 1.2.1 (5 May 2026)

* fix: file:/// ERR_ACCESS_DENIED on Android 11+ — added MANAGE_EXTERNAL_STORAGE ("All Files Access") permission
* fix: file:/// ERR_ACCESS_DENIED on Android 10 — serve local files via app process in shouldInterceptRequest
* fix: allow universal file access for JS cross-file references in local pages

## 1.2.0 (21 Dec 2023)

* feat: auto prepend http protocol
* feat: access localhost over http 

## 1.1.0 (30 Mar 2023)

* feat: dark mode
* feat: splashscreen
* fix: unable to login