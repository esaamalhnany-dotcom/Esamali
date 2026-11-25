# 🏢 الولاء بزنز — Alwala Business

> **التطبيق المركزي لإدارة الفروع والأقسام — يعمل على جميع الهواتف الذكية (Android + iOS)**

![Flutter](https://img.shields.io/badge/Flutter-Cross%20Platform-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Version](https://img.shields.io/badge/Version-1.0.0-orange)

---

## 📌 ما هو هذا المشروع؟

**الولاء بزنز** هو تطبيق مركزي واحد تستطيع منه:
- إنشاء **فروع** جديدة (إب، صنعاء، تعز، عدن...)
- إنشاء **أقسام عمل متفرعة** تحت كل فرع (مبيعات، مخزن، محاسبة...)
- إدارة كل شيء من **لوحة تحكم واحدة**
- يعمل على **جميع أنواع الهواتف الذكية** من كود واحد بـ Flutter

---

## 🗂️ هيكل المشروع (كل خطوة في ملف مستقل)

```
alwala-business/
│
├── README.md                  ← أنت هنا (نظرة عامة)
├── CHANGELOG.md               ← سجل التحديثات
├── CONTRIBUTING.md            ← كيف تساهم / تعدّل
├── LICENSE                    ← رخصة المشروع
├── .gitignore                 ← ملفات يتجاهلها Git
│
├── docs/                      ← الوثائق
│   ├── 00-Overview.md         ← نظرة عامة على الفكرة
│   ├── 01-Project-Structure.md← شرح هيكل الملفات
│   ├── 02-Roadmap.md          ← خارطة الطريق
│   └── 03-GitHub-Guide.md     ← دليل الرفع على GitHub
│
├── steps/                     ← ⭐ كل خطوة في مجلد مستقل
│   ├── 01-setup/              ← الخطوة 1: تجهيز المشروع
│   ├── 02-central-dashboard/  ← الخطوة 2: لوحة التحكم المركزية
│   ├── 03-branches/           ← الخطوة 3: إدارة الفروع
│   ├── 04-sections/           ← الخطوة 4: إدارة الأقسام
│   ├── 05-company-tree/       ← الخطوة 5: هيكل الشركة
│   ├── 06-database/           ← الخطوة 6: قاعدة البيانات
│   ├── 07-authentication/     ← الخطوة 7: تسجيل الدخول
│   ├── 08-android-build/      ← الخطوة 8: بناء أندرويد
│   ├── 09-ios-build/          ← الخطوة 9: بناء آيفون
│   └── 10-publish/            ← الخطوة 10: النشر
│
├── app/                       ← تطبيق Flutter (Android + iOS)
│   ├── pubspec.yaml
│   └── lib/
│       ├── main.dart
│       ├── core/theme/
│       └── features/
│           ├── dashboard/
│           ├── branches/
│           ├── sections/
│           ├── tree/
│           └── settings/
│
├── web-prototype/             ← النموذج التجريبي (HTML)
│   └── index.html
│
└── .github/workflows/         ← بناء تلقائي على GitHub
    └── flutter.yml
```

---

## 🚀 البدء السريع

### تجربة النموذج التجريبي (بدون تثبيت أي شيء)
افتح ملف `web-prototype/index.html` في المتصفح مباشرة.

### تشغيل تطبيق Flutter
```bash
cd app
flutter pub get
flutter run        # على هاتفك أو المحاكي
flutter build apk --release   # بناء ملف أندرويد
```

---

## 🔄 كيف أعدّل أو أضيف أو أحذف؟

كل خطوة لها ملفها الخاص في `steps/` — عدّل الملف الذي تريده فقط:

| أريد... | أعدّل هذا الملف |
|---|---|
| تغيير لوحة التحكم | `steps/02-central-dashboard/README.md` + `app/lib/features/dashboard/` |
| إضافة فرع جديد | من داخل التطبيق، أو عدّل `app/lib/features/branches/` |
| إضافة قسم جديد | من داخل التطبيق، أو عدّل `app/lib/features/sections/` |
| تغيير الألوان | `app/lib/core/theme/app_theme.dart` |
| إضافة خطوة جديدة | أنشئ مجلداً جديداً `steps/11-.../` وانسخ قالب أي خطوة |

> **قاعدة ذهبية:** كل تعديل = ملف واحد واضح + تحديث `CHANGELOG.md` + حفظ على GitHub.

---

## 📞 الحالة الحالية

- [x] الخطوة 1: تجهيز المشروع والهيكل
- [x] الخطوة 2: لوحة التحكم المركزية (نموذج تجريبي)
- [x] الخطوة 3: إدارة الفروع (نموذج تجريبي)
- [x] الخطوة 4: إدارة الأقسام (نموذج تجريبي)
- [x] الخطوة 5: هيكل الشركة (نموذج تجريبي)
- [ ] الخطوة 6: ربط قاعدة بيانات Firebase
- [ ] الخطوة 7: تسجيل دخول حقيقي
- [ ] الخطوة 8: بناء ملف APK لأندرويد
- [ ] الخطوة 9: بناء نسخة iOS
- [ ] الخطوة 10: النشر على المتاجر

---

## 📄 الرخصة
MIT — انظر ملف `LICENSE`
