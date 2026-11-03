# 📱 UZKOMX — Android Native Application (Release v0.2.3)

<p align="center">
  <strong>Markaziy Osiyo va Oʻzbekiston tarixi boʻyicha milliy raqamli komikslar platformasining Android mobil ilovasi.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android%20Native-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Version-v0.2.3-blue?style=for-the-badge" alt="Version" />
  <img src="https://img.shields.io/badge/Min%20SDK-24%20(Android%207.0)-orange?style=for-the-badge" alt="Min SDK" />
  <img src="https://img.shields.io/badge/Target%20SDK-35%20(Android%2015)-green?style=for-the-badge" alt="Target SDK" />
  <img src="https://img.shields.io/badge/Compliance-Google%20Play%20Ready-E53935?style=for-the-badge&logo=googleplay&logoColor=white" alt="Google Play" />
</p>

---

## 📌 Loyiha haqida (Overview)

Ushbu ombor **UZKOMX** mobil platformasining Android native qurilishi (`android` loyihasi) uchun moʻljallangan. Ilova zamonaviy vertikal Webtoon mutolaa dvigateli, oflayn rejim, ikki yozuvli (Lotin va Kirill) matn tizimi hamda Google Play Store talablariga mos xavfsizlik mexanizmlari bilan jihozlangan.

---

## 🏗 Arxitektura va Texnik Koʻrsatkichlar

- **Paket nomi (Package Name):** `com.uzkomx.app`
- **Versiya:** `0.2.3` (VersionCode: `5`)
- **Minimal Android talabi:** Android 7.0 (API Level 24)
- **Maqsadli Android talabi:** Android 15 (API Level 35)
- **Qoʻllab-quvvatlanadigan arxitekturalar:** `armeabi-v7a`, `arm64-v8a`, `x86`, `x86_64`
- **Dizayn va UI:** Edge-to-Edge ekran, Adaptive Launcher Icon, maxsus Splash screen.

---

## 🚀 Qanday qilib quriladi (Build Instructions)

### Talablar:
- **JDK:** Java 17 yoki undan yuqori
- **Android SDK:** API Level 35 va Android Build Tools 35.0.0

### Debug APK yigʻish:
```bash
cd android
./gradlew assembleDebug
```
Yigʻilgan fayl: `android/app/build/outputs/apk/debug/app-debug.apk`

### Production Release APK / AAB yigʻish:
Xavfsizlik maqsadida imzo kaliti (keystore) va parollar omborda saqlanmaydi. Relizni imzolash uchun quyidagi muhit oʻzgaruvchilarini belgilash mumkin:

```bash
export UZKOMX_RELEASE_STORE_PASSWORD="sizning-parolingiz"
export UZKOMX_RELEASE_KEY_ALIAS="uzkomx-key"
export UZKOMX_RELEASE_KEY_PASSWORD="sizning-parolingiz"

cd android
./gradlew assembleRelease
# yoki Google Play App Bundle uchun:
./gradlew bundleRelease
```

---

## 🛡 Xavfsizlik va Maxfiylik (Trust & Safety)

1. **Google Play UGC Talablari:** Ilova ichida nooʻrin kontent ustidan 1-bosishda shikoyat qilish imkoniyati mavjud.
2. **In-App Huquqiy Markaz:** Foydalanish shartlari va Maxfiylik siyosati ilovaning oʻzida toʻliq koʻrinadi.
3. **Kesh va Xotira nazorati:** Foydalanuvchi ilova keshini istalgan vaqt tozalay oladi.

---

## 📄 Litsenziya

© 2026 UZKOMX Ltd. Barcha huquqlar himoyalangan.
