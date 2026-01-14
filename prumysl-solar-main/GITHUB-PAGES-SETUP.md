# GitHub Pages Setup Guide

## المشكلة | Problem
GitHub Pages لا يدعم ملفات `.htaccess` أو `_redirects` - هذه خاصة بـ Apache و Netlify.

## الحل | Solution

### 1. ملف `.nojekyll`
تم إنشاء ملف `.nojekyll` لتعطيل معالجة Jekyll (غير ضروري للموقع الثابت).

### 2. ملف `404.html`
تم إنشاء صفحة `404.html` التي تعيد توجيه الروابط بدون `.html` تلقائياً.

### 3. إعدادات GitHub Pages

#### في إعدادات المستودع:
1. اذهب إلى **Settings** → **Pages**
2. **Source**: اختر **Deploy from a branch**
3. **Branch**: اختر `main` (أو `master`)
4. **Folder**: اختر `/ (root)`
5. اضغط **Save**

### 4. الروابط

**مهم**: في GitHub Pages، يجب استخدام `.html` في الروابط أو الاعتماد على `404.html` لإعادة التوجيه.

#### الخيار 1: استخدام `.html` في الروابط (الأسهل)
```html
<a href="/moka.html">موكا</a>
<a href="/index.html">الرئيسية</a>
```

#### الخيار 2: استخدام روابط بدون `.html` (سيتم إعادة التوجيه تلقائياً)
```html
<a href="/moka">موكا</a>
<a href="/">الرئيسية</a>
```

### 5. التحقق من النشر

بعد الرفع:
1. انتظر 1-2 دقيقة
2. افتح `https://[username].github.io/[repository-name]/`
3. أو `https://prumysl.cc` إذا كان CNAME مضبوط

## ملاحظات مهمة

- ✅ ملف `.nojekyll` موجود - يعطل Jekyll
- ✅ ملف `404.html` موجود - يعيد توجيه الروابط
- ✅ ملف `CNAME` موجود - للنطاق المخصص
- ⚠️ `.htaccess` لا يعمل على GitHub Pages
- ⚠️ `_redirects` لا يعمل على GitHub Pages (خاص بـ Netlify)

## حلول بديلة

### إذا أردت روابط نظيفة تماماً:

1. **استخدم Netlify** بدلاً من GitHub Pages
   - Netlify يدعم ملف `_redirects`
   - رفع الملفات كما هي

2. **استخدم Vercel**
   - Vercel يدعم `vercel.json` للروابط
   - رفع الملفات كما هي

3. **استخدم Apache Server**
   - Apache يدعم `.htaccess`
   - رفع الملفات كما هي

## التحقق من الملفات المطلوبة

تأكد من وجود هذه الملفات في الجذر:
- ✅ `index.html`
- ✅ `404.html`
- ✅ `.nojekyll`
- ✅ `CNAME` (إذا كان لديك نطاق مخصص)
- ✅ `css/style.css`
- ✅ `img/` (مجلد الصور)
