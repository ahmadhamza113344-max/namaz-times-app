# اوقاتِ نماز – بنانے کا طریقہ

## 1. کھولیں
Android Studio (تازہ ورژن) میں File → Open → یہ فولڈر منتخب کریں۔ Gradle خود سیٹ اپ ہو جائے گا (انٹرنیٹ چاہیے)۔
اگر Studio اپڈیٹ کا کہے تو "Update" کر دیں۔

## 2. اپنا نام لگائیں
`app/build.gradle.kts` میں `applicationId` بدل کر اپنا منفرد نام رکھیں (مثلاً com.yourname.awqat)۔

## 3. APK (ٹیسٹ کے لیے)
Build → Build Bundle(s)/APK(s) → Build APK(s)

## 4. AAB (Play Store کے لیے)
Build → Generate Signed App Bundle / APK → Android App Bundle → Create new keystore
- keystore فائل اور پاسورڈ کی کئی کاپیاں محفوظ رکھیں۔ کھو گئی تو اپڈیٹ نہیں دے سکیں گے۔
- فائل بنے گی: app/release/app-release.aab

## 5. Play Console
- AAB اپلوڈ کریں
- PRIVACY_POLICY.md کو کسی ویب پیج پر رکھ کر اس کا لنک دیں
- Data safety فارم میں: Approximate location – صرف ڈیوائس پر، شیئر نہیں ہوتا
- Play کی تازہ ضرورت کے مطابق targetSdk چیک کر لیں

## نوٹ
- فی الحال کراچی طریقہ (18°) ہے۔ دوسرا طریقہ چاہیے تو `PrayerCalc.compute` میں زاویے بدلیں۔
- کوئی بھی چیز اپنی مسجد کے اوقات سے ملا لیں۔
