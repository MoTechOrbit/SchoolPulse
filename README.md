<div align="center">

<img src="icon.png" alt="SchoolPulse Logo" width="120" height="120">

# SchoolPulse

### 🎓 مساعدك المدرسي الذكي

**نظّم جدولك، اضبط منبهاتك، واستقبل تنبيهاتك اليومية — بدون إنترنت.**

[![Flutter](https://img.shields.io/badge/Flutter-3.47+-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.13+-0175C2?logo=dart&logoColor=white)](https://dart.dev)
[![Android](https://img.shields.io/badge/Android-7.0+-3DDC84?logo=android&logoColor=white)](https://www.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-2.3+-7F52FF?logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](#-الترخيص)

[المميزات](#-المميزات) • [التثبيت](#-التثبيت) • [لقطات الشاشة](#-لقطات-الشاشة) • [المطور](#-المطور)

</div>

---

## 📱 نظرة عامة

**SchoolPulse** هو تطبيق مساعد مدرسي مصمم للطلاب، يعمل **بدون إنترنت** بالكامل، ويساعدهم على:

- تنظيم جدول المدرسة الأسبوعي.
- ضبط منبهات يومية حقيقية تعمل حتى عند إغلاق التطبيق.
- استقبال إشعارات ذكية تحتوي على **جدول اليوم كاملًا** عند عمل المنبه.

كل البيانات تُحفظ **محليًا على الجهاز** — بدون حساب، بدون خادم، وبدون Firebase.

---

## ✨ المميزات

### 📅 جدول مرن
- عدد الحصص **قابل للتخصيص** (من 1 إلى 10).
- دعم **7 أيام** مع إمكانية تفعيل/تعطيل أي يوم.
- لكل حصة: المادة، المدرس، الفصل، والملاحظات.

### ⏰ منبهات حقيقية
- تعمل حتى عند:
  - إغلاق التطبيق.
  - إخراجه من Recent Apps.
  - قفل الهاتف.
- إعادة جدولة تلقائية بعد:
  - إعادة تشغيل الهاتف.
  - تغيير الوقت أو المنطقة الزمنية.
  - تحديث التطبيق.

### 🔔 ربط المنبه بالجدول (الميزة الأبرز)
- عند إنشاء منبه، يمكنك تفعيل خيار: **"عرض جدول المدرسة مع الإشعار"**.
- عندما يعمل المنبه، يقرأ التطبيق **جدول اليوم** من التخزين المحلي.
- يظهر الإشعار بمحتوى ذكي:

```
SchoolPulse
صباح الخير يا محمد!
المدرسة ستبدأ قريبًا.
جدول اليوم:
1. رياضيات
2. عربي
3. إنجليزي
4. علوم
5. تاريخ
6. ألعاب
```

### 🎵 أصوات مخصصة
- اختر من بين عدة نغمات مدمجة.
- عاين أي صوت قبل الحفظ.
- صوت تشغيل متكرر حتى يوقفه المستخدم.

### 📢 إشعارات محلية متقدمة
- تعمل في كل الحالات: التطبيق مفتوح، في الخلفية، مغلق، أو الهاتف مقفل.
- إدارة كاملة لصلاحيات Android 13+ و14+.
- قنوات إشعارات منفصلة (Channels).

### 🌙 واجهة حديثة
- **Material 3** بالكامل.
- وضعان: **فاتح** و**داكن** (أو حسب الجهاز).
- تصميم متجاوب لكل أحجام الشاشات.
- Animations بسيطة واحترافية.

### 🔒 خصوصية كاملة
- ✅ بدون تسجيل دخول.
- ✅ بدون حساب مستخدم.
- ✅ بدون خادم أو Backend.
- ✅ بدون Firebase.
- ✅ بدون أي طلب شبكة.
- ✅ كل البيانات محفوظة محليًا على الجهاز.

---

## 🖼️ لقطات الشاشة

<div align="center">

| الرئيسية | الجدول | المنبهات | الإعدادات |
|:--------:|:------:|:--------:|:---------:|
| ![Home](screenshots/home.png) | ![Timetable](screenshots/timetable.png) | ![Alarms](screenshots/alarms.png) | ![Settings](screenshots/settings.png) |

| Setup Wizard | شاشة الرنين | الوضع الداكن | About Developer |
|:------------:|:-----------:|:------------:|:---------------:|
| ![Setup](screenshots/setup.png) | ![Ringing](screenshots/ringing.png) | ![Dark](screenshots/dark.png) | ![About](screenshots/about.png) |

</div>

---

## 🛠️ التقنيات المستخدمة

### Framework
- **Flutter 3.47+** مع **Dart 3.13+**
- **Material 3** للتصميم

### State Management
- **Provider** — نظام واحد فقط.

### Local Storage
- **SharedPreferences** — تخزين البيانات كـ JSON.
- **path_provider** — لحفظ صور الطالب.

### الإشعارات والمنبهات
- **flutter_local_notifications** — إشعارات محلية.
- **android_alarm_manager_plus** — جدولة على مستوى النظام.
- **timezone** + **flutter_timezone** — معالجة صحيحة للمناطق الزمنية.
- **Kotlin + ForegroundService** — تشغيل الصوت المتكرر.
- **MediaPlayer** مع `AudioAttributes.USAGE_ALARM` — لتشغيل الصوت كمنبه حقيقي.

### أدوات إضافية
- **image_picker** — اختيار صورة الطالب.
- **permission_handler** — إدارة الصلاحيات.
- **url_launcher** — فتح تطبيق الاتصال.
- **intl** — تنسيق التواريخ.
- **uuid** — توليد معرفات المنبهات.

---

## 🏗️ البنية المعمارية

المشروع يتبع **Clean Architecture** مع فصل واضح للمسؤوليات:

```
lib/
├── main.dart                          # نقطة الدخول
├── app.dart                           # إعداد Providers
│
├── core/                              # الأنظمة المشتركة
│   ├── constants/                     # الثوابت
│   ├── theme/                         # الثيمات
│   ├── utils/                         # أدوات مساعدة
│   └── services/                      # خدمات النظام
│       ├── notification_service.dart
│       ├── alarm_service.dart
│       └── alarm_native_channel.dart
│
├── models/                            # نماذج البيانات
│   ├── student_model.dart
│   ├── timetable_model.dart
│   └── alarm_model.dart
│
├── data/                              # طبقة البيانات
│   ├── local/                         # التخزين المحلي
│   └── repositories/                  # المستودعات
│
├── features/                          # الصفحات
│   ├── home/
│   ├── setup/
│   ├── timetable/
│   ├── alarms/
│   └── settings/
│
└── widgets/                           # مكونات مشتركة

android/app/src/main/kotlin/com/example/school_pulse/
├── MainActivity.kt                    # نقطة دخول Android
├── AlarmMethodChannel.kt              # جسر Flutter ↔ Android
├── AlarmService.kt                    # خدمة الصوت (ForegroundService)
├── AlarmReceiver.kt                   # مستقبل المنبهات
├── AlarmScheduler.kt                  # مجدول AlarmManager
├── AlarmOverlayController.kt          # شاشة فوق التطبيقات
└── AlarmPreviewPlayer.kt              # معاينة الصوت
```

---

## 🚀 التثبيت

### المتطلبات
- Flutter SDK 3.47+
- Android SDK 24+
- JDK 17+

### خطوات التشغيل

```bash
# 1. استنسخ المستودع
git clone https://github.com/username/school-pulse.git
cd school-pulse

# 2. جلب الحزم
flutter pub get

# 3. التحقق من البيئة
flutter doctor

# 4. التشغيل
flutter run
```

### بناء APK

```bash
# Debug
flutter build apk --debug

# Release (شامل)
flutter build apk --release

# Release (لكل معمارية)
flutter build apk --release --split-per-abi
```

**الناتج**: `build/app/outputs/flutter-apk/`

### بناء AAB (لـ Google Play)

```bash
flutter build appbundle --release
```

**الناتج**: `build/app/outputs/bundle/release/app-release.aab`

---

## 🔐 إعداد التوقيع (للإصدار)

### 1. أنشئ مفتاح التوقيع

```bash
keytool -genkey -v -keystore my-release-key.jks \
  -keyalg RSA -keysize 2048 -validity 10000 \
  -alias my-key-alias
```

### 2. أنشئ `android/key.properties`

```properties
storePassword=كلمة_المرور
keyPassword=كلمة_المرور
keyAlias=my-key-alias
storeFile=C:/path/to/my-release-key.jks
```

### 3. اربط التوقيع في `android/app/build.gradle.kts`

```kotlin
signingConfigs {
    create("release") {
        keyAlias = keystoreProperties["keyAlias"] as String?
        keyPassword = keystoreProperties["keyPassword"] as String?
        storeFile = keystoreProperties["storeFile"]?.let { file(it) }
        storePassword = keystoreProperties["storePassword"] as String?
    }
}
```

### 4. ابنِ الإصدار

```bash
flutter build appbundle --release
```

> ⚠️ **لا ترفع `key.properties` أو `my-release-key.jks` إلى GitHub أبدًا.**

---

## 🎵 إضافة صوت مخصص

1. ضع ملف `.mp3` في:
   ```
   android/app/src/main/res/raw/alarm_mySound.mp3
   ```

2. أضف اسمًا عربيًا في `lib/features/alarms/widgets/alarm_form_sheet.dart`:
   ```dart
   static const Map<String, String> _soundLabels = {
     'alarm_default': 'افتراضي',
     'alarm_school': 'منبه المدرسة',
     'alarm_mySound': 'اسمي الخاص',  // ← أضف هنا
   };
   ```

3. أعد البناء:
   ```bash
   flutter clean
   flutter pub get
   flutter build apk --release
   ```

---

## 🔒 صلاحيات Android المطلوبة

| الصلاحية | الاستخدام |
|---------|-----------|
| `POST_NOTIFICATIONS` | إرسال الإشعارات (Android 13+) |
| `SCHEDULE_EXACT_ALARM` | جدولة المنبهات بدقة |
| `RECEIVE_BOOT_COMPLETED` | إعادة الجدولة بعد إعادة التشغيل |
| `WAKE_LOCK` | إيقاظ الجهاز لعرض الإشعار |
| `VIBRATE` | الاهتزاز |
| `FOREGROUND_SERVICE` | خدمة الصوت |
| `SYSTEM_ALERT_WINDOW` | عرض الشاشة فوق التطبيقات (اختياري) |

---

## ⚠️ قيود معروفة

- **Android 12+**: يتطلب إذن `SCHEDULE_EXACT_ALARM` يدويًا من المستخدم.
- **Android 14+**: يتطلب `FOREGROUND_SERVICE_SPECIAL_USE`.
- **بعض المصنّعين** (Xiaomi, Huawei, Oppo, Vivo): قد يوقفون التطبيق في الخلفية — يُنصح بإضافة التطبيق إلى "قائمة الحماية".
- **`flutter_timezone`**: لا يزال يستخدم KGP القديم. قد يظهر تحذير أثناء البناء.

---

## 🗺️ خريطة الطريق

- [x] جدول مرن
- [x] منبهات حقيقية
- [x] ربط المنبه بالجدول
- [x] أصوات مخصصة
- [x] وضعان فاتح وداكن
- [x] دعم اللغة العربية
- [ ] دعم iOS
- [ ] Localization (عربي/إنجليزي)
- [ ] إحصائيات الحضور
- [ ] مزامنة اختيارية

---

## 🤝 المساهمة

المشروع حاليًا **مغلق للمساهمات**. لأي استفسار أو اقتراح:

- 📞 **Phone**: 01553308975 / 01553308947
- 💬 **Issues**: [GitHub Issues](https://github.com/username/school-pulse/issues)

---

## 📄 الترخيص

```
© 2026 Mohamed Hany. All rights reserved.
```

هذا المشروع **خاص** ولا يُسمح بنسخه أو توزيعه أو تعديله بدون إذن كتابي من المطور.

---

## 👨‍💻 المطور

<div align="center">

**Mohamed Hany**

مطوّر تطبيقات Flutter

📞 01553308975 | 01553308947

© 2026 Mohamed Hany. All rights reserved.

</div>

---

<div align="center">

**⭐ إذا أعجبك المشروع، لا تنسَ إضافة نجمة!**

</div>
