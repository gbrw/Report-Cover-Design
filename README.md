# University Report Cover Designer

[العربية](#العربية) | [English](#english)

## العربية

أداة تعمل في المتصفح لإنشاء أغلفة رسمية بحجم A4 للتقارير الجامعية. توفر معاينة مباشرة قابلة للتحرير، ومحتوى بالعربية والإنجليزية، وتخطيطات كلاسيكية متعددة، وشعارات مخصصة، وتصدير ملفات PDF من جانب العميل.

### المزايا

- وضعان للعربية والإنجليزية مع اتجاه الصفحة من اليمين إلى اليسار ومن اليسار إلى اليمين.
- عشرة قوالب أغلفة بحدود وترويسات وأنماط عناوين مختلفة.
- تحرير مباشر لبيانات الجامعة، والكلية، والدراسة، والفصل الدراسي، والسنة الأكاديمية، وعنوان التقرير، والطالب، والمشرف.
- عناصر تحكم لرفع شعاري الترويسة.
- معاينة بحجم A4 تتكيف مع الشاشات الأصغر.
- علامتا تبويب منفصلتان للتحرير والمعاينة على الأجهزة المحمولة.
- إجراء لإعادة ضبط الحقول النصية.
- تصدير ملف PDF باسم `Official_Report_Cover.pdf`.

### التقنيات المستخدمة

- HTML5
- CSS3 وJavaScript خام ضمن صفحة واحدة
- Tailwind CSS محمّل من شبكة CDN
- html2pdf.js محمّلة من شبكة CDN
- أيقونات Font Awesome محمّلة من شبكة CDN
- خطوط Google:‏ Amiri وCairo وNoto Naskh Arabic وLibre Baskerville

### التشغيل محلياً

لا حاجة إلى خطوة بناء أو تثبيت حزم.

1. افتح نافذة أوامر في مجلد المشروع.
2. شغّل خادم ملفات ثابتة:

   ```bash
   python -m http.server 8000
   ```

3. افتح `http://localhost:8000` في المتصفح.

يلزم اتصال بالإنترنت لأن مكتبة التنسيق ومكتبة PDF والأيقونات وخطوط الويب تُحمّل من شبكات CDN خارجية.

### طريقة الاستخدام

1. اختر العربية أو الإنجليزية.
2. اختر واحداً من القوالب العشرة.
3. حرّر بيانات التقرير في اللوحة الجانبية.
4. ارفع شعاراً لأي من جانبي الترويسة اختيارياً.
5. راجع معاينة A4.
6. اختر **Export PDF** على سطح المكتب أو **Save PDF** على الهاتف المحمول لتنزيل الغلاف.

تتم جميع عمليات التحرير وإنشاء ملف PDF داخل المتصفح. لا يرسل هذا المشروع الصور المرفوعة أو البيانات المُدخلة إلى واجهة خلفية.

### بنية المشروع

```text
.
|-- index.html       # بنية التطبيق وأنماطه وJavaScript
`-- images/
    |-- Uni.png      # الشعار الافتراضي في الجانب الأيمن
    |-- Col.png      # الشعار الافتراضي في الجانب الأيسر
    `-- G.md         # ملف عنصر نائب فارغ
```

### الحالة الحالية

يحتوي هذا المستودع على تطبيق وظيفي يعمل من جانب العميل. لا توجد فيه واجهة خلفية أو مساحة لحفظ البيانات أو نظام بناء أو مدير حزم أو اختبارات آلية. يبدأ تحديث الصفحة جلسة تحرير جديدة.

لا يتضمن هذا المستودع ملف ترخيص على مستوى المشروع.

## English

A browser-based tool for creating formal A4 university report covers. It provides an editable live preview, Arabic and English content, multiple classic layouts, custom logos, and client-side PDF export.

### Features

- Arabic and English modes with right-to-left and left-to-right page direction.
- Ten cover templates with different borders, headers, and title styles.
- Live editing for university, college, study, semester, academic year, report title, student, and supervisor details.
- Upload controls for the two header logos.
- A4 preview that scales for smaller screens.
- Separate edit and preview tabs on mobile devices.
- Reset action for text fields.
- PDF export as `Official_Report_Cover.pdf`.

### Tech Stack

- HTML5
- CSS3 and vanilla JavaScript in a single page
- Tailwind CSS loaded from a CDN
- html2pdf.js loaded from a CDN
- Font Awesome icons loaded from a CDN
- Google Fonts: Amiri, Cairo, Noto Naskh Arabic, and Libre Baskerville

### Run Locally

No build step or package installation is required.

1. Open a terminal in the project directory.
2. Start a static file server:

   ```bash
   python -m http.server 8000
   ```

3. Open `http://localhost:8000` in a browser.

An internet connection is required because the styling library, PDF library, icons, and web fonts are loaded from external CDNs.

### How to Use

1. Choose Arabic or English.
2. Select one of the ten templates.
3. Edit the report details in the side panel.
4. Optionally upload a logo for either side of the header.
5. Review the A4 preview.
6. Select **Export PDF** on desktop or **Save PDF** on mobile to download the cover.

All editing and PDF generation happen in the browser. Uploaded images and entered data are not sent to a backend by this project.

### Project Structure

```text
.
|-- index.html       # Application markup, styles, and JavaScript
`-- images/
    |-- Uni.png      # Default right-side logo
    |-- Col.png      # Default left-side logo
    `-- G.md         # Empty placeholder file
```

### Current Status

This repository contains a functional client-side application. It has no backend, saved-data storage, build system, package manager, or automated tests. Reloading the page starts a new editing session.

No project-level license file is included in this repository.
