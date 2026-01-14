# Prumysl Website - Project Information

## 📋 نظرة عامة | Overview

موقع إلكتروني احترافي لبيع كاميرات المراقبة الشمسية في المغرب.

## 🗂️ هيكل المشروع | Project Structure

```
prumysl-solar-main/
│
├── 📄 HTML Pages (12 pages)
│   ├── index.html              → / (Homepage)
│   ├── moka.html               → /moka
│   ├── dio-moka.html           → /dio-moka
│   ├── assas.html              → /assas
│   ├── garde-corps.html        → /garde-corps
│   ├── saqr.html               → /saqr
│   ├── about.html              → /about
│   ├── contact.html            → /contact
│   ├── faq.html                → /faq
│   ├── return-policy.html      → /return-policy
│   ├── terms.html              → /terms
│   └── thank-you.html          → /thank-you
│
├── 📁 css/
│   └── style.css               # Main stylesheet (907 lines)
│
├── 📁 js/                      # JavaScript files (ready for future use)
│
├── 📁 assets/                  # Additional assets
│
├── 📁 img/                     # All images organized by product
│   ├── logo.png
│   ├── Desktop-hero.jpg
│   ├── Mobile-hero.jpg
│   ├── product-1.jpg
│   ├── product-2.jpg
│   └── [Product folders]/
│
├── 📄 Configuration Files
│   ├── CNAME                   # Custom domain
│   ├── .htaccess               # Apache URL rewriting
│   ├── _redirects              # Netlify redirects
│   └── .gitignore              # Git ignore rules
│
└── 📄 Documentation
    ├── README.md               # Main documentation
    ├── STRUCTURE.md            # Structure details
    └── PROJECT-INFO.md         # This file
```

## ✨ المميزات | Features

### 🎨 التصميم
- ✅ تصميم متجاوب 100% (Responsive Design)
- ✅ محسّن للأجهزة المحمولة
- ✅ دعم RTL للغة العربية
- ✅ واجهة مستخدم عصرية وجذابة

### ⚡ الأداء
- ✅ Lazy Loading للصور
- ✅ Preload للموارد الحرجة
- ✅ تحسينات CSS
- ✅ تحميل سريع

### 📱 تجربة المحمول
- ✅ رأس ثابت عند التمرير
- ✅ زر واتساب عائم
- ✅ أزرار كبيرة للمس
- ✅ جداول قابلة للتمرير
- ✅ تباعد محسّن

### 🔗 SEO & URLs
- ✅ روابط نظيفة بدون .html
- ✅ دعم Apache & Netlify
- ✅ Facebook Pixel
- ✅ Meta tags جاهزة

## 🚀 الاستضافة | Hosting

### GitHub Pages
- استخدم ملف `_redirects` أو `.htaccess`
- رفع الملفات كما هي

### Netlify
- استخدم ملف `_redirects`
- النشر التلقائي من Git

### Apache Server
- استخدم ملف `.htaccess`
- تأكد من تفعيل mod_rewrite

## 📝 ملاحظات مهمة | Important Notes

1. **الروابط**: جميع الروابط بدون `.html` (مثل `/moka` بدلاً من `/moka.html`)
2. **الصور**: جميع الصور في مجلد `img/` مع تنظيم حسب المنتج
3. **CSS**: ملف التنسيقات في `css/style.css`
4. **JavaScript**: الكود الحالي مضمن في HTML، مجلد `js/` جاهز للمستقبل

## 🔧 الصيانة | Maintenance

- تحديث المنتجات: عدّل ملفات HTML في المجلد الرئيسي
- تحديث التصميم: عدّل `css/style.css`
- إضافة صور: ضعها في `img/` مع التنظيم المناسب
