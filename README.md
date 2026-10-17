# Proxy SDK Maven repository

Static Maven repository for the in-app network inspector SDK of [Proxy](https://github.com/bharath914/proxy), an open-source HTTP/HTTPS debugging proxy. Built from `sdk/android` in that repository; do not edit by hand.

```kotlin
// settings.gradle.kts
pluginManagement { repositories { maven("https://bharath914.github.io/proxy-sdk-maven/"); google(); mavenCentral(); gradlePluginPortal() } }
dependencyResolutionManagement { repositories { maven("https://bharath914.github.io/proxy-sdk-maven/"); google(); mavenCentral() } }

// app/build.gradle.kts
plugins { id("com.android.application"); id("dev.proxy.inspector") version "0.1.0" }
```

Debug builds only: release builds get a no-op library. See the [quick start](https://github.com/bharath914/proxy/blob/main/docs/sdk-quickstart.md).

Versions: 0.1.0. Licensed under MIT OR Apache-2.0.
