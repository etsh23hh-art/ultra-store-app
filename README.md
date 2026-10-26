# Ultra Store – تطبيق أندرويد

يفتح https://ultrastores.online/ داخل تطبيق (WebView) مع: سحب للتحديث، شريط تحميل، زر رجوع، صفحة "لا يوجد إنترنت"، وفتح روابط واتساب/اتصال/سوشيال/الخرائط في تطبيقاتها.

## بناء ملف APK

### الطريقة 1: GitHub (بدون تثبيت أي شيء)
1. أنشئ مستودعًا جديدًا على GitHub وارفع محتويات هذا المجلد (بما فيها مجلد `.github`).
2. افتح تبويب **Actions** ثم **Build APK** ثم **Run workflow**.
3. بعد دقائق نزّل `UltraStore-apk` من قسم Artifacts، وبداخله `app-debug.apk`.
4. انقله للموبايل وثبّته (فعّل "التثبيت من مصادر غير معروفة").

### الطريقة 2: Android Studio
افتح المجلد، ثم Build ▸ Build APK(s). الملف في `app/build/outputs/apk/debug/`.

## تخصيص
- الرابط: `HOME_URL` في `MainActivity.java`
- الاسم: `res/values/strings.xml`
- الأيقونة: `res/drawable/ic_launcher_foreground.xml`
- لنشر التطبيق على Google Play تحتاج بناء release موقّع (AAB) وحساب مطوّر.
