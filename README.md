# 📚 Library Management System | نظام إدارة المكتبات واستعارة الكتب

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![Railway](https://img.shields.io/badge/Railway-Deployable-0B0D0E?logo=railway&logoColor=white)](https://railway.app/)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)

---

## 📌 نبذة عامة (Project Overview)

**نظام إدارة المكتبات (Library Management System)** هو نظام شامل لأتمتة فهارس الكتب وإدارة عمليات الإعارة والإرجاع وتتبع المشتركين مع دعم أرقام الإيداع القياسية الدولية (ISBN).

النظام مجهّز بحاويات **Docker** وإعدادات نشر فوري على **Railway** مع تكامل تلقائي لقواعد بيانات MySQL.

---

## 🏗️ الوحدات الوظيفية (Core Modules)

```
library-management-system/
├── books/                 # فهرس الكتب، تصنيفات العناوين، وإدارة المخزون
├── borrowers/             # سجلات المستعيرين (الطلاب، الباحثين، والأعضاء)
├── borrow/                # عمليات الإعارة، تتبع فترات الاستحقاق، وغرامات التأخير
├── includes/              # الترويسات والتذييلات والمكونات المشتركة
├── assets/                # الصور والأيقونات وتنسيقات الواجهة
├── config.php             # إعدادات الاتصال الآمن بقاعدة البيانات
├── Dockerfile             # حاوية التشغيل وبيئة أباتشي/PHP
└── railway.json           # إعدادات النشر السحابي
```

---

## 🌟 الميزات الجوهرية (Key Features)

* **فهرسة وتصنيف الكتب:** إضافة وتعديل وتصنيف الكتب حسب المؤلف، دار النشر، وسنة الإصدار ورقم الـ ISBN.
* **إدارة عمليات الإعارة والاسترجاع:** تسجيل تاريخ الإعارة وتاريخ الاستحقاق والتنبيه عند التأخير.
* **إدارة سجلات المستعيرين:** حفظ بيانات الأعضاء ورقم الهوية وسجل الاستعارات السابقة لكل عضو.
* **بحث وتصفية ذكية:** إمكانية البحث السريع عن أي كتاب بالعنوان أو اسم الكاتب أو الرقم التسلسلي.

---

## 🚀 دليل التشغيل (Getting Started)

### الخيار 1: باستخدام Docker
```bash
docker build -t library-system .
docker run -d -p 8080:80 --name library_app library-system
```

### الخيار 2: عبر الخادم المحلي (XAMPP / LAMP)
1. إنشاء قاعدة بيانات جديدة واستيراد الجداول.
2. ضبط بيانات الاتصال في `config.php`.
3. فتح المشروع عبر المتصفح: `http://localhost/library-management-system`.

---

## 📄 الترخيص (License)
جميع الحقوق محفوظة للمطور © **3hosa**.
