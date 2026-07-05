# 🛠️ Setup Guide

## خطوات التثبيت والإعداد الكامل

### 1. تجهيز Git LFS محلياً

```bash
# تثبيت Git LFS
git lfs install

# تتبع الملفات الكبيرة
git lfs track "*.csv"
git lfs track "*.zip"
git lfs track "*.xlsx"
git lfs track "*.ipynb"

# إضافة ملف .gitattributes
git add .gitattributes
```

### 2. استنساخ المستودع

```bash
git clone https://github.com/tarek-sabry/Olist-Delivery-Performance-SLA-Analysis.git
cd Olist-Delivery-Performance-SLA-Analysis
```

### 3. إنشاء بيئة افتراضية

```bash
# إنشاء
python -m venv venv

# تفعيل (Windows)
venv\Scripts\activate

# تفعيل (macOS/Linux)
source venv/bin/activate
```

### 4. تثبيت المكتبات

```bash
pip install -r requirements.txt
```

### 5. إضافة الملفات الخاصة بك

#### نسخ الملفات إلى المجلدات:

```
# Jupyter Notebooks
cp your_notebooks/*.ipynb notebooks/

# بيانات (CSV, Excel)
cp your_data/*.csv data/

# الصور
cp your_images/*.png images/

# العروض التقديمية
cp your_presentation/*.pdf presentation/
```

### 6. رفع الملفات إلى GitHub

```bash
# إضافة جميع الملفات
git add .

# كتابة رسالة الالتزام
git commit -m "Add initial project files"

# رفع إلى GitHub
git push origin main
```

---

## 📋 قائمة المراجعة

- [ ] تم تثبيت Git LFS
- [ ] تم استنساخ المستودع
- [ ] تم إنشاء البيئة الافتراضية
- [ ] تم تثبيت المكتبات
- [ ] تم نسخ ملفات Notebooks
- [ ] تم نسخ ملفات البيانات
- [ ] تم نسخ الصور والعروض
- [ ] تم رفع الملفات إلى GitHub

---

## 🆘 استكشاف الأخطاء

### المشكلة: Git LFS غير مثبت
```bash
# الحل
git lfs install
```

### المشكلة: خطأ في الرفع (ملف كبير جداً)
```bash
# تحقق من إعدادات LFS
git lfs ls-files
```

### المشكلة: لا يمكن تفعيل البيئة الافتراضية
```bash
# جرب
python -m venv venv
venv\Scripts\python -m pip install --upgrade pip
```

---

تم! ✅ مشروعك جاهز للعمل!