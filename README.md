# Prebuilt APKs

This is a collection of FOSS APKs, coupled with the respective Android.mk for an
easy integration in the Android build system.
These are just the official unmodified prebuilt binaries, signed by the
corresponding developers, except for:
 * com.google.android.maps, as the JAR and the XML have been extracted from the ZIP on the [microG's GitHub release page](https://github.com/microg/android_frameworks_mapsv1/releases)
 * additional_repos.xml, as it is just the microG FDroid repository XML file, plus additional repos

To include them in your build just add their name in CUSTOM_PACKAGES (for
example in vendor/lineage/config/common.mk).

The included APKs are:
 * FDroid packages (binaries sourced from [here](https://f-droid.org/packages/org.fdroid.fdroid/) and [here](https://f-droid.org/packages/org.fdroid.fdroid.privileged/))
   * ClassyShark3xodus: checks apps for code signatures of known trackers (provided by Exodus)
   * DejaVuNlpBackend: UnifiedNlp backend that uses locally acquired WLAN/Wi-Fi AP and mobile/cellular tower data to resolve user location
   * FDroid: a catalogue of FOSS (Free and Open Source Software) applications for the Android platform
   * FDroid Privileged Extension: a FDroid extension to ease the installation/removal of apps
   * NewPipe: a lightweight YouTube frontend without proprietary APIs or Google Play Services
   * NominatimNlpBackend: UnifiedNlp (no GAPPS) backend that uses MapQuest's Nominatim service (based on OpenStreetMap) for geocoding
   * additional_repos.xmly: a simple package to include the [microG FDroid repository](https://microg.org/fdroid.html) in the ROM (requires FDroid >= 1.5)
 * microG packages (binaries sourced from [here](https://microg.org/download.html) and [here](https://github.com/microg/android_frameworks_mapsv1))
   * GmsCore: the main component of microG, a FOSS reimplementation of the Google Play Services (requires GsfProxy and FakeStore for full functionality)
   * GsfProxy: a GmsCore proxy for legacy GCM compatibility
   * FakeStore: an empty package that mocks the existence of the Google Play Store
   * com.google.android.maps: legacy microG's mapsv1 reimplementation
 * Bromite packages (binaries sourced from [here](https://github.com/bromite/bromite/releases)) 
   * Bromite: Chromium plus ad blocking and other privacy-related features
 * EdXposed packages (binaries sourced from [here](https://github.com/ElderDrivers/EdXposedManager/releases))
   * EdXposedManager: companion Android application for EdXposed
 * LineageOS packages (binaries sourced from [here](https://download.lineageos.org/extras))
   * OpenWeatherProvider: "Open Weather Map" provider for the LineageOS v16 weather service

