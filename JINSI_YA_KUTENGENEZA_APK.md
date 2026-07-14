# Jinsi ya kutengeneza APK kutoka mradi huu

Mradi huu ni programu kamili ya Android Studio. Faili lako la HTML
(`ProX__1-5-1-2-8.html`) tayari limewekwa ndani kama
`app/src/main/assets/index.html`, na `MainActivity.kt` imewekwa
kuunganisha WebView na "daraja" la kuchagua faili
(`onShowFileChooser`) — ndilo lililokuwa halipo kwenye App Creator 24.

## Njia ya haraka zaidi (bila kompyuta): GitHub + GitHub Actions
1. Fungua akaunti ya bure ya GitHub (github.com) kwenye simu au kompyuta.
2. Tengeneza "New repository" tupu.
3. Pakia (upload) folda hii yote ya mradi ndani ya hilo repository
   (GitHub inaruhusu "Upload files" moja kwa moja kwenye kivinjari).
4. Niambie ukishafika hapo — nitakutengenezea faili la
   `.github/workflows/build.yml` litakalojenga APK kiotomatiki kila
   ukipakia mabadiliko, na kukupa link ya kupakua APK bila
   kuhitaji Android Studio au kompyuta yenye nguvu.

## Njia ya kawaida: Android Studio (kwenye kompyuta)
1. Pakua na sakinisha **Android Studio** (bure): developer.android.com/studio
2. Fungua Android Studio → "Open" → chagua folda hii
   (`ManukuuPapoHapoApp`).
3. Subiri "Gradle Sync" ikamilike (inahitaji intaneti mara ya kwanza
   kupakua zana za ujenzi).
4. Kwenye menyu: **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. APK yako itapatikana kwenye:
   `app/build/outputs/apk/debug/app-debug.apk`
6. Hamishia hiyo faili kwenye simu na uifungue kuisakinisha
   (huenda ukahitaji kuruhusu "Install from unknown sources").

## Baada ya kusakinisha
Jaribu kubonyeza "Chagua hifadhi/folda" kwenye tab ya Sauti au Video —
sasa kidirisha halisi cha kuchagua faili cha Android kitafunguka,
kwa sababu `onShowFileChooser` imewekwa ndani ya `MainActivity.kt`.

## Ukitaka kubadilisha jina la programu au ikoni
- Jina: badilisha `app_name` kwenye
  `app/src/main/res/values/strings.xml`
- Ikoni: ongeza faili za `ic_launcher.png` kwenye folda za
  `res/mipmap-*` (Android Studio ina kifaa cha "Image Asset" cha
  kukusaidia kutengeneza hizo kiotomatiki: bonyeza-kulia `res` →
  New → Image Asset).
