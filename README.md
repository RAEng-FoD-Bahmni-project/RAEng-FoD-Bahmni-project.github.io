# Bahmni Arabic RTL — نظام السجلات الطبية الموحد

A fully localized, hospital-grade electronic medical records system. Built with support for Arabic and RTL languages from the ground up. Patient registration, clinical encounters, lab, pharmacy, imaging, and billing. Zero license fees.

نظام سجلات طبية إلكتروني متكامل ومُعرَّب بالكامل، مصمم لدعم اللغة العربية والكتابة من اليمين إلى اليسار. تسجيل المرضى، اللقاءات السريرية، المختبر، الصيدلية، التصوير، والفوترة. بدون رسوم ترخيص.

---

## 📖 Full Installation Guides | أدلة التثبيت الكاملة

- **English Guide:** [Download from Google Drive](https://drive.google.com/file/d/18Z1ruQNfTZCaWEv9QzFcNzpFqYoLeTbf/view?usp=sharing)
- **الدليل بالعربية:** [تحميل من Google Drive](https://drive.google.com/file/d/1tAcgKpV1vUTgCDnOqqdAOi6G0FyURZZW/view?usp=sharing)

---

## Quick Start Guide | دليل البدء السريع

### English

#### Introduction

Bahmni is an open-source hospital information system that has been effectively utilized as a digital medical record since November 2012. It prioritizes supporting hospitals in low-resource environments by utilizing a range of available open-source products.

Bahmni's provision of information greatly aids healthcare workers and providers in enhancing the competence and quality of patient care services, while concurrently minimizing errors in clinics. The open-source digital medical record of Bahmni has been listed within the DPG record associated with the Digital Public Goods Alliance. Presently, Bahmni applications are operational in over 500 hospitals across 50 countries, benefiting millions of patients worldwide.

#### Requirements

- A server with a USB port
- A USB drive with the bootable system image (80 GB)
- Network connectivity (for post-install configuration)

#### Installation Overview

1. **Prepare BIOS settings** — Enter the BIOS on your server and configure it to boot from USB. Press Enter at startup to access the BIOS screen.

2. **Boot from USB** — Insert the USB drive containing the system image and boot the server. The installer will launch automatically.

3. **Install Ubuntu** — The installation process will install the Ubuntu operating system onto one of the server's hard disk drives.

4. **Automatic system deployment** — After Ubuntu is installed, the Unified Medical Records Management System will be installed automatically. The system functions within integrated Docker containers that encompass all necessary libraries and integrations.

5. **Start the system** — Simply execute the system's boot file to start all services. The same straightforward process applies to the system shutdown file.

#### Post-Installation

Once the system is running, access the Bahmni interface via your browser at the server's IP address. All modules — patient registration, clinical encounters, lab, pharmacy, imaging, and billing — are pre-configured and ready to use.

---

### العربية

#### مقدمة

باهمني هو نظام معلومات مستشفيات مفتوح المصدر يُستخدم كسجل طبي رقمي منذ نوفمبر 2012. يهدف إلى تلبية احتياجات المستشفيات في البيئات منخفضة الموارد من خلال الاستفادة من مجموعة من المنتجات مفتوحة المصدر المتوفرة.

توفر المعلومات التي يتيحها باهمني دعماً كبيراً للعاملين في الرعاية الصحية في تحسين كفاءة وجودة خدمات رعاية المرضى، مع تقليل الأخطاء في العيادات. تم إدراج السجل الطبي الرقمي مفتوح المصدر لباهمني ضمن سجل DPG التابع لتحالف السلع العامة الرقمية. حالياً، تعمل تطبيقات باهمني في أكثر من 500 مستشفى في 50 دولة، ويستفيد منها ملايين المرضى حول العالم.

#### المتطلبات

- خادم مزود بمنفذ USB
- ذاكرة USB تحتوي على صورة النظام القابلة للتمهيد (80 جيجابايت)
- اتصال بالشبكة (للإعداد بعد التثبيت)

#### نظرة عامة على التثبيت

1. **تهيئة إعدادات BIOS** — ادخل إلى إعدادات BIOS على الخادم وقم بتهيئته للإقلاع من USB. اضغط على Enter عند بدء التشغيل للوصول إلى شاشة BIOS.

2. **الإقلاع من USB** — أدخل ذاكرة USB التي تحتوي على صورة النظام وشغّل الخادم. سيبدأ برنامج التثبيت تلقائياً.

3. **تثبيت Ubuntu** — ستقوم عملية التثبيت بتنصيب نظام تشغيل Ubuntu على أحد أقراص التخزين الصلبة في الخادم.

4. **نشر النظام تلقائياً** — بعد تثبيت Ubuntu، يتم تنصيب نظام إدارة السجلات الطبية الموحد تلقائياً. يعمل النظام ضمن حاويات Docker متكاملة تحتوي على جميع المكتبات والتكاملات اللازمة.

5. **تشغيل النظام** — ما عليك سوى تشغيل ملف بدء النظام لتفعيل جميع الخدمات. نفس العملية البسيطة تنطبق على ملف إيقاف النظام.

#### بعد التثبيت

بمجرد تشغيل النظام، يمكنك الوصول إلى واجهة باهمني عبر المتصفح باستخدام عنوان IP الخادم. جميع الوحدات — تسجيل المرضى، اللقاءات السريرية، المختبر، الصيدلية، التصوير، والفوترة — مُعدّة مسبقاً وجاهزة للاستخدام.

---

## Architecture | البنية التقنية

The system runs as integrated Docker containers on Ubuntu, encompassing:

| Module | Description |
|--------|-------------|
| **OpenMRS** | Core medical records platform |
| **Bahmni Apps** | Clinical UI (fully RTL) |
| **OpenELIS** | Laboratory information system |
| **Odoo** | Billing & inventory management |
| **Dcm4chee** | Medical imaging (DICOM/PACS) |

## Links

- 🌐 [Landing Page](https://raeng-fod-bahmni-project.github.io)
- 📦 [All Repositories](https://github.com/RAEng-FoD-Bahmni-project)

## License

Components are licensed under their respective open-source licenses. See the [Licensing section](https://raeng-fod-bahmni-project.github.io#licensing) on the landing page for details.
