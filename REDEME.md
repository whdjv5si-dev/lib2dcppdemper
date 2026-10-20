```markdown
# 🛠️ lib2dcppdemper

**أداة تحليل مكتبات C++ (Cocos2d-x / Unity / Unreal) على Android**

---

## 👨‍💻 المطور
**ADEM**

## 🏢 المختبر
**DZ Security Lab**

---

## 📖 عن الأداة

**lib2dcppdemper** هي أداة احترافية مخصصة لتحليل واستخراج الدوال من مكتبات C++ (`.so`) على نظام Android.

### 🎯 تدعم:
- ✅ **Cocos2d-x** (`libcocos2dcpp.so`)
و يعمل بكفائمة على محرك Cocos2d
- ✅ **أي محرك C++**

---

## ✨ الميزات

| الميزة | الوصف |
|---|---|
| 🎯 **استخراج الدوال** | يستخرج جميع الدوال مع عناوينها |
| 🔍 **تفكيك ARM64** | يفك كامل التعليمات (Disassembly) |
| 📍 **دالة محددة** | يفك دالة واحدة بعنوانها |
| ⚡ **وضع سريع** | استخراج سريع خلال 1-2 دقائق |
| 🐢 **وضع دقيق** | مع فك أسماء C++ (c++filt) |
| 📁 **ملفات كبيرة** | يدعم ملفات حتى 100 ميجابايت |

---

## 📁 مكان وضع المكتبة

ضع ملف المكتبة (`.so`) في المسار التالي:

غير اسم ملف
lib2dcppdemper.so
إلى 
lib2dcppdemper
احذف .so 
```

/storage/emulated/0/Download/

```

**أمثلة:**
```

/storage/emulated/0/Download/libcocos2dcpp.so
/storage/emulated/0/Download/libil2cpp.so
/storage/emulated/0/Download/libgame.so

```

---

## 📦 ملف المشغل

```

mod.py

```

---

## 🚀 طريقة التشغيل

### 1️⃣ التوجه لمجلد التحميلات
```bash
cd /sdcard/Download/
```

2️⃣ تشغيل المثبت

```bash
python mod.py
```

3️⃣ استخدام الأداة

```bash
cd ~
./lib2dcppdemper [الأمر]
```

---

📋 الأوامر

الأمر الوظيفة
./lib2dcppdemper /2 استخراج الدوال (وضع سريع)
./lib2dcppdemper /1 استخراج الدوال (وضع دقيق)
./lib2dcppdemper /3 تفكيك المكتبة كاملة
./lib2dcppdemper -d 0xADDR تفكيك دالة محددة
./lib2dcppdemper -h عرض المساعدة

خيارات إضافية

الخيار الوصف
-f /path/lib.so تحديد مكتبة مختلفة
-o output.cs تحديد اسم الملف الناتج

---

📁 الملفات الناتجة

الأمر اسم الملف الموقع
/2 أو /1 libcocos2dcpp_offsets.cs /storage/emulated/0/Download/
/3 libcocos2dcpp_disasm.cs /storage/emulated/0/Download/
-d 0xADDR libcocos2dcpp_0xADDR.cs /storage/emulated/0/Download/

---

💡 أمثلة عملية

📌 استخراج الدوال (سريع)

```bash
./lib2dcppdemper /2
```

📌 استخراج الدوال (دقيق)

```bash
./lib2dcppdemper /1
```

📌 تفكيك المكتبة كاملة

```bash
./lib2dcppdemper /3
```

📌 تفكيك دالة محددة

```bash
./lib2dcppdemper -d 0x5ca2cc
```

📌 استخدام مكتبة Unity

```bash
./lib2dcppdemper -f /storage/emulated/0/Download/libil2cpp.so /2
```

📌 استخدام مكتبة مخصصة

```bash
./lib2dcppdemper -f /storage/emulated/0/Download/libgame.so /2
```

📌 تغيير اسم الملف الناتج

```bash
./lib2dcppdemper -o my_offsets.cs /2
```

---

🛠️ المتطلبات

mod.py يقوم بتثبيتها تلقائياً:

الأداة الحزمة الوظيفة
gcc gcc مترجم C
make make أداة بناء
readelf binutils قراءة ELF
objdump binutils تفكيك ARM64
c++filt binutils فك أسماء C++

---

📊 مقارنة الأوضاع

الوضع السرعة الدقة الاستخدام
/2 ⚡ سريع جيد استخراج سريع
/1 🐢 بطيء دقيق جداً تحليل متقدم
/3 🐢 بطيء تفكيك كامل تحليل عميق
-d ⚡ سريع دالة واحدة تفكيك محدد

---

💾 دعم الملفات الكبيرة

الميزة الدعم
ملفات حتى 100 ميجابايت ✅
آلاف الدوال ✅
تفكيك سريع ✅
معالجة ذكية ✅

---

⚠️ ملاحظات مهمة

· ✅ يدعم ARM64 فقط
· ✅ يعمل على Termux
· ✅ تلقائي بالكامل
· ✅ آمن للاستخدام
· ✅ مفتوح المصدر

---

📞 الدعم

· المطور: ADEM
· المختبر: DZ Security Lab

---

🏆 الخلاصة

الأداة المثالية لتحليل مكتبات C++ و Cocos2d-x على Android. مثالية للمطورين والباحثين في مجال الأمن السيبراني والهندسة العكسية.

---

```
▀▄ DZ Security Lab ▄▀
```