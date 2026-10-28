# دليل الدفع الدولي والبطاقات الافتراضية
# International Payments Guide

دليل تعليمي بالعربية والإنجليزية من **ماجد فتحي — Majd Fatihy**، يجمع شروحات الدفع والشراء أونلاين دوليًا، والبطاقات الافتراضية، وشراء USDT وشحن الرصيد، وحلول مشكلات الدفع.

**الرابط المستهدف بعد تفعيل GitHub Pages:**
https://majdfatihy.github.io/international-payment-guide/

**القناة:** https://www.youtube.com/@MajdFatihy  
**الموقع الأساسي:** https://majdfatihy.com/  
**البريد الرسمي:** info@majdfatihy.com

## محتوى الموقع

- مكتبة من 213 فيديو مختارًا من بيانات القناة، موزعة حسب المهمة والمنصة.
- شروحات Bybit وRedotPay وRizon وOKX وGrey وSpend.net، ومنصات ومحافظ أخرى.
- إصدار البطاقات وتفعيلها، وشراء USDT، وشحن الحسابات والتحويلات.
- الاشتراكات والشراء من المواقع الأجنبية، وحلول رفض البطاقة ومشكلات الدفع.
- روابط إحالة وأكواد مع توضيح شروط المكافآت ومصادرها.
- روابط المشاريع المنشورة ووسائل التواصل والصفحات القانونية.

## المميزات

- واجهة عربية وإنجليزية، مع اختيار اللغة حسب المتصفح وأولوية الاختيار المحفوظ.
- صفحة إنجليزية مستقلة داخل `en/`. تبقى عناوين الفيديوهات بلغتها العربية الأصلية.
- بحث وتصفية حسب المنصة والمهمة ونوع الفيديو، مع عرض Bybit افتراضيًا.
- صور مصغرة تبدأ بأعلى جودة متاحة، ثم تستخدم بدائل عند تعذر التحميل.
- تخطيط متجاوب، واتجاه RTL/LTR، وخط مضمّن، ومسميات للأزرار ودعم تنقل لوحة المفاتيح.
- خلفية متحركة، وأيقونات تواصل، وروابط واتساب وتيليجرام مع رسالة يكتبها الزائر.
- HTML ثابت للمحتوى والروابط، وتحسين تدريجي بالـJavaScript دون مفاتيح API مطلوبة.

## ملفات النشر

| الملف أو المجلد | وظيفته |
| --- | --- |
| `index.html` | الصفحة الرئيسية العربية مع اكتشاف اللغة |
| `en/index.html` | النسخة الإنجليزية |
| `og-image.png` | صورة مشاركة الموقع على منصات التواصل |
| `channel-avatar.jpg` | صورة القناة وأيقونة الموقع |
| `sitemap.xml` | خريطة الموقع للنسختين |
| `.nojekyll` | تعطيل معالجة Jekyll للموقع الثابت؛ ينشئه ملف الرفع إذا لم يوجد |
| `GO-LIVE.md` | تعليمات النشر وملاحظات الإصدار 1.3.0 |
| `source/` | مصادر إعادة توليد الموقع، إذا أُرفقت من حزمة التطوير |
| `upload-to-github.bat` | أداة رفع اختيارية لنظام Windows، تُحمَّل منفصلة |

لا يحتاج تشغيل الموقع إلى تثبيت Node.js أو إعداد خادم خلفي. يحتاج فتح الفيديوهات والصور الخارجية وروابط المنصات إلى اتصال بالإنترنت.

## النشر على GitHub Pages

1. أنشئ المستودع `majdfatihy/international-payment-guide` أو استخدم المستودع الموجود.
2. ارفع ملفات النشر إلى جذر فرع `main` مع الحفاظ على مجلد `en/`.
3. من إعدادات المستودع افتح **Settings → Pages**.
4. اختر **Deploy from a branch**، ثم **main**، ثم **/ (root)** واحفظ.
5. بعد اكتمال النشر، افحص الصفحة الرئيسية والنسخة الإنجليزية وصورة المشاركة.

الرابط الإنجليزي المستهدف:
https://majdfatihy.github.io/international-payment-guide/en/

### الرفع باستخدام ملف BAT

ضع `upload-to-github.bat` بجوار `index.html` بعد فك ضغط الحزمة، ثم شغّله. يستخدم نسخة عمل منفصلة داخل `.github-publish-international-payment-guide`، ويرفع ملفات الموقع العامة المحددة فقط إلى `main` دون استخدام الرفع الإجباري.

قد يطلب Git تسجيل الدخول إلى GitHub أو إدخال اسم وبريد صاحب الـcommit. لا تضع كلمة مرور أو توكن داخل الملفات. لا يحذف الملف ملفات المستودع الأخرى، ولا يرفع مجلد `source/` تلقائيًا.

**لرفع README وملفات التوثيق:** أضف `README.md` إلى جذر المستودع من واجهة GitHub عبر **Add file → Upload files**. أداة BAT الحالية ترفع ملفات الموقع الأساسية فقط، ولا تشمل README أو GO-LIVE ضمن قائمة الرفع.

## التعديل وإعادة البناء

عند استخدام مجلد المصادر المرفق:

1. راجع `source/config.json` لتعديل إعدادات النشر وروابط الإحالة.
2. راجع ملفات المحتوى والتصميم والترجمة داخل `source/` للتعديلات المطلوبة.
3. شغّل من مجلد الحزمة:

```bash
python3 source/finalize.py
```

على Windows، يمكن استخدام:

```bat
py source\finalize.py
```

4. استخدم ملفات النشر الناتجة داخل `source/dist/`، وانسخها إلى جذر المستودع مع مجلد `en/`.

لا تعدّل النسخة العربية وحدها إذا كان التغيير يجب أن يظهر في النسخة الإنجليزية أيضًا. راجع ملفات الترجمة وإعدادات البناء قبل إعادة التوليد.

## السيو والفهرسة

الإعدادات الحالية مخصصة لعنوان:
`https://majdfatihy.github.io/international-payment-guide/`

تتضمن الصفحات عناوين وأوصافًا، وcanonical منفصلة لكل لغة، وhreflang، وOpen Graph، وصورة مشاركة، وبيانات منظمة وخريطة موقع.

إذا غيّرت اسم المستودع أو استخدمت نطاقًا مخصصًا، عدّل `baseUrl` داخل إعدادات المصادر ثم أعد البناء قبل النشر. لا تترك canonical أو روابط الصور على العنوان القديم.

بعد النشر:

- تحقق من نجاح تحميل الصفحتين وصورة `og-image.png` عبر HTTPS.
- افحص الرابطين في Google Search Console.
- أرسل خريطة الموقع: https://majdfatihy.github.io/international-payment-guide/sitemap.xml
- لا تنشئ `robots.txt` داخل مستودع فرعي وتتوقع أن يحل محل ملف `robots.txt` الموجود في جذر النطاق.

الالتزام بالإعدادات الفنية وإرسال خريطة الموقع لا يضمن الفهرسة أو ترتيبًا محددًا في نتائج البحث.

## دقة المعلومات والإحالات

الموقع دليل مستقل وليس موقعًا رسميًا للمنصات المذكورة. قد يحصل صاحب الموقع على عمولة أو مكافأة عند استخدام بعض روابط الإحالة، وتُوسم هذه الروابط بـ`rel="sponsored"`.

- الرسوم والهدايا والحدود وإتاحة الخدمات تختلف حسب البلد والحساب والحملة ووقت الاستخدام.
- تحقق من الشروط الظاهرة في حسابك قبل التسجيل أو الإيداع أو الدفع.
- العروض والأسعار في عناوين الفيديوهات القديمة ليست وعودًا بأنها ما زالت سارية.
- إجمالي 20 USDT في شرح Bybit مشروط بمهمتين منفصلتين وأهليتك لكل عرض؛ ليس مكافأة بطاقة تلقائية.
- مبلغ 200 دولار شهريًا المذكور في دليل الأرباح هدف تخطيطي للزائر وليس دخلًا موثقًا أو مضمونًا.
- رابط Grey مُدرج كما قدّمه صاحب القناة؛ إذا فتح الصفحة الرئيسية فقط، فتحقق من تسجيل كود الإحالة. احتساب الإحالة لم يُؤكَّد باختبار تسجيل فعلي.

## الخصوصية والتواصل

لا تتضمن الصفحة نموذجًا لجمع بيانات البطاقات أو كلمات المرور أو معالجة المدفوعات. يُحفظ اختيار اللغة محليًا عندما يتيح المتصفح ذلك. فتح الروابط والصور الخارجية يخضع لسياسات الجهات المقدمة لها.

نافذة التواصل تفتح واتساب أو تيليجرام مع نص السؤال؛ على الزائر تأكيد الإرسال داخل التطبيق.

- [من نحن](https://majdfatihy.github.io/about.html)
- [اتصل بنا](https://majdfatihy.github.io/contact.html)
- [سياسة الخصوصية](https://majdfatihy.github.io/privacy.html)
- [شروط الاستخدام](https://majdfatihy.github.io/terms.html)
- [إخلاء المسؤولية](https://majdfatihy.github.io/disclaimer.html)
- [واتساب](https://wa.me/201066732514)
- [تيليجرام](https://t.me/majdfatihy)

## English overview

A bilingual educational directory by Majd Fatihy covering international payments, virtual cards, USDT funding, payment troubleshooting and conditional referral rewards. It includes 213 curated channel videos, search and category filters, Arabic/English interface switching, and social/contact links. Original video titles remain in Arabic.

Deploy the public files to the `main` branch root and enable GitHub Pages. The current canonical URLs target `https://majdfatihy.github.io/international-payment-guide/` and its `en/` page. Update the source configuration and rebuild before changing the hosting URL.

No card acceptance, referral reward, monthly income or search ranking is guaranteed. Confirm current eligibility and terms with each provider.

## المصادر الرسمية

- [GitHub Pages — إعداد مصدر النشر](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Google Search — متطلبات الفهرسة الفنية](https://developers.google.com/search/docs/essentials/technical)
- [Google Search — خرائط الموقع](https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview)
- [Google Search — الروابط المدفوعة والإحالات](https://developers.google.com/search/docs/crawling-indexing/qualify-outbound-links)
- [Bybit Card — شروط برنامج الإحالة](https://www.bybit.com/en/help-center/article/FAQ-Bybit-Card-Referral-Program)
- [Bybit — شروط برنامج الإحالة العام](https://www.bybit.com/en/help-center/article/Bybit-Referral-Program-General-FAQ)

آخر تحديث للتوثيق: **28 أكتوبر 2026**. إصدار الموقع الموصوف: **1.3.0**.
