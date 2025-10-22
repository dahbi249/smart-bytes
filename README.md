# نادي Smart Bytes العلمي - موقع النادي الإلكتروني

## نظرة عامة / Overview

موقع إلكتروني احترافي لنادي Smart Bytes العلمي في كلية العلوم والتكنولوجيا بجامعة تمنراست. الموقع مصمم باللغة العربية مع دعم كامل للاتجاه من اليمين إلى اليسار (RTL) ومتجاوب مع جميع الأجهزة.

A professional website for Smart Bytes scientific club at the Faculty of Science and Technology, University of Tamanrasset. The website is designed in Arabic with full RTL support and responsive design for all devices.

## الملفات المطلوبة / Required Files

- `index.html` - الصفحة الرئيسية مع المحتوى العربي
- `styles.css` - ملف التنسيقات مع دعم RTL
- `README.md` - دليل التخصيص (هذا الملف)

## كيفية التخصيص / Customization Guide

### 1. تغيير الألوان / Changing Colors

في ملف `styles.css`، يمكنك تعديل المتغيرات في بداية الملف:

```css
:root {
    --primary-color: #0B5FFF;    /* اللون الأساسي */
    --primary-light: #1E88E5;    /* اللون الأساسي الفاتح */
    --accent-color: #00C2A8;     /* لون التمييز */
    --light-bg: #F7F9FC;         /* خلفية فاتحة */
    --dark-text: #0F1724;        /* نص داكن */
}
```

### 2. تغيير الخطوط / Changing Fonts

لتغيير الخط العربي، عدّل المتغير في `styles.css`:

```css
:root {
    --font-family: 'Cairo', 'Arial', sans-serif;
}
```

أو استخدم خطوط أخرى من Google Fonts مثل:
- 'Noto Naskh Arabic'
- 'Amiri'
- 'Scheherazade New'

### 3. تحديث معلومات الحدث / Updating Event Information

في ملف `index.html`، ابحث عن قسم "برنامج الافتتاح" وعدّل:

```html
<div class="info-item">
    <span class="info-label">التاريخ:</span>
    <span class="info-value">الأحد 26 أكتوبر 2025</span>
</div>
<div class="info-item">
    <span class="info-label">الوقت:</span>
    <span class="info-value">10:00 صباحًا</span>
</div>
<div class="info-item">
    <span class="info-label">المكان:</span>
    <span class="info-value">قاعة السمعي البصري – كلية العلوم والتكنولوجيا</span>
</div>
```

### 4. تحديث معلومات الفريق / Updating Team Information

استبدل الأسماء في قسم "فريقنا":

```html
<h3 class="team-name">[اسم الرئيس]</h3>
<p class="team-role">رئيس النادي</p>
```

### 5. استبدال الصور / Replacing Images

#### شعار النادي / Club Logo
استبدل الصورة في `index.html`:

```html
<img src="data:image/svg+xml;base64,..." alt="شعار نادي Smart Bytes" class="logo">
```

#### صور أعضاء الفريق / Team Photos
استبدل الصور في قسم الفريق:

```html
<img src="data:image/svg+xml;base64,..." alt="صورة رئيس النادي" class="photo">
```

**ملاحظة:** جميع الصور الحالية هي placeholders باستخدام data URIs. استبدلها بصور حقيقية.

### 6. ربط نموذج الاتصال / Connecting Contact Form

في ملف `index.html`، ابحث عن:

```html
<form class="contact-form" action="#" method="POST">
```

استبدل `action="#"` بأحد الخيارات التالية:

#### أ) استخدام Formspree (مجاني)
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

#### ب) استخدام Netlify Forms
```html
<form class="contact-form" action="#" method="POST" data-netlify="true">
```

#### ج) ربط بخادم مخصص
```html
<form class="contact-form" action="https://your-server.com/contact" method="POST">
```

### 7. تحديث معلومات التواصل / Updating Contact Information

عدّل المعلومات في قسم "تواصل معنا":

```html
<div class="contact-item">
    <span class="contact-label">البريد الإلكتروني:</span>
    <span class="contact-value">smartbytes.univ.tmr@gmail.com</span>
</div>
```

### 8. إضافة روابط وسائل التواصل الاجتماعي / Adding Social Media Links

في قسم "تواصل معنا"، استبدل الروابط:

```html
<a href="#" class="social-link" aria-label="فيسبوك">
<a href="#" class="social-link" aria-label="إنستغرام">
```

### 9. تخصيص المحتوى / Content Customization

#### النص الرئيسي / Main Text
عدّل النصوص في الأقسام المختلفة:

- **Hero Section:** العنوان والعنوان الفرعي
- **About Section:** وصف النادي
- **Activities Section:** قائمة الأنشطة

#### إضافة أقسام جديدة / Adding New Sections
يمكنك إضافة أقسام جديدة باتباع نفس النمط:

```html
<section class="new-section" id="new-section">
    <div class="container">
        <h2 class="section-title">عنوان القسم الجديد</h2>
        <!-- محتوى القسم -->
    </div>
</section>
```

## الميزات المتقدمة / Advanced Features

### 1. دعم الطباعة / Print Support
الموقع يدعم الطباعة مع تنسيقات مخصصة للطباعة.

### 2. إمكانية الوصول / Accessibility
- دعم التنقل بالكيبورد
- نصوص بديلة للصور
- تباين ألوان مناسب
- دعم قارئات الشاشة

### 3. تحسين الأداء / Performance
- تحميل الخطوط المحسن
- صور مضغوطة
- CSS و JavaScript محسن

### 4. دعم RTL كامل / Full RTL Support
- تخطيط مرآة للاتجاه العربي
- تنسيقات مخصصة للنص العربي
- دعم الخطوط العربية

## استكشاف الأخطاء / Troubleshooting

### مشاكل شائعة / Common Issues

1. **الخطوط لا تظهر بشكل صحيح**
   - تأكد من اتصال الإنترنت لتحميل Google Fonts
   - تحقق من صحة رابط الخط في HTML

2. **التخطيط لا يعمل على الهاتف**
   - تأكد من وجود viewport meta tag
   - تحقق من CSS media queries

3. **نموذج الاتصال لا يعمل**
   - تأكد من صحة action URL
   - تحقق من إعدادات الخادم

## الدعم / Support

للمساعدة في التخصيص أو حل المشاكل، يمكنك:

1. مراجعة التعليقات في الكود
2. التحقق من console المتصفح للأخطاء
3. اختبار الموقع على أجهزة مختلفة

## الترخيص / License

هذا المشروع مفتوح المصدر ويمكن استخدامه وتعديله بحرية.

---

**ملاحظة مهمة:** تذكر استبدال جميع النصوص بين الأقواس المربعة `[مثل هذا]` بالمعلومات الفعلية قبل النشر.

**Important Note:** Remember to replace all text in square brackets `[like this]` with actual information before publishing.
