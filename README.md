پرامپت: ساخت پروژه وب‌سایت لندینگ اپ iOS به نام "Mahdigeram"

شرح کلی:
من می‌خوام یک مخزن GitHub کامل و آماده برای انتشار روی GitHub Pages داشته باشم با نام ریپو: `mahdigeram`. این مخزن باید یک سایت معرفی اپ (فارسی، راست‌به‌چپ) برای اپ iOS باشد. سایت باید ساده، واکنش‌گرا و شامل صفحات زیر باشد:
- index.html (صفحهٔ اصلی — لندینگ + دکمهٔ دانلود App Store placeholder)
- privacy.html (سیاست حفظ حریم خصوصی فارسی)
- terms.html (شرایط استفاده فارسی)
- css/style.css (استایل کلی، RTL-friendly)
- js/main.js (اسکریپت کوچک برای مقداردهی سال در فوتر و ثبت service worker)
- manifest.json (برای PWA، با آیکون‌های placeholder)
- sw.js (سرویس‌ورکر ساده برای کش)
- assets/logo.svg (لوگوی ساده SVG)
- README.md (توضیح پروژه + دستورالعمل نشر روی GitHub Pages)
- .gitignore
- LICENSE (MIT)

جزئیات محتوا و الزامات فنی:
1. زبان و جهت: تمام صفحات به فارسی و با `dir="rtl"`. متاتگ مناسب (charset=utf-8, viewport).
2. نام اپ: **Mahdigeram** — این مقدار را دقیق در عنوان‌ها و فوتر استفاده کن.
3. ایمیل پشتیبانی: **ashnam084@gmail.com** — در صفحه تماس/پشتیبانی و صفحات حقوقی قرار بده.
4. صفحه دانلود: دکمهٔ دانلود باید فعلاً به placeholder `https://apps.apple.com` لینک بده (بعداً من لینک واقعی App Store رو قرار میدم).
5. استایل: Modern, dark-ish theme (رنگ اصلی #06b6d4 یا مشابه). فونت وب‌امن (Vazirmatn optional) — اگر استفاده شد fallback به Arial.
6. دسترسی و SEO: اضافه کردن meta description و title مناسب برای هر صفحه. اضافه کردن لینک canonical و favicon (از assets/logo.svg).
7. PWA: manifest.json با name/short_name, theme_color, background_color و آیکون‌های placeholder (assets/logo-192.png, assets/logo-512.png).
8. Service Worker: فایل sw.js با استراتژی cache-first برای فایل‌های استاتیک و fallback به fetch.
9. README.md: توضیح خلاصهٔ پروژه، ساختار فایل‌ها، نحوهٔ انتشار روی GitHub Pages (اینگونه: ساخت repo `mahdigeram`, push کردن فایل‌ها، Settings → Pages → main branch → / (root)). اضافه کن نمونهٔ دستور git برای push مرحله‌ای.
10. LICENSE: از MIT استفاده کن و مؤلف را خالی بگذار یا نام `Mahdigeram` بنویس.
11. Commitها: کدها را در چند commit منطقی قرار بده: `init: add project scaffold`, `feat: add pages and styles`, `chore: add manifest and service worker`, `docs: add README and LICENSE`.
12. Branch: `main` به‌عنوان شاخهٔ پیش‌فرض.

نیازمندی‌های بصری / تولیدی:
- فایل assets/logo.svg باید یک لوگوی ساده و قابل ویرایش SVG تولید کند (مربع با گوشه‌های گرد و یک آیکون پیام/پاکت یا حرف M ساده داخلش).
- hero-phone.svg اختیاری؛ اگر تولید شد میتواند یک شمایل ساده از آیفون با صفحهٔ اپ داخلی باشد.
- تصاویر/آیکون‌ها می‌توانند placeholder باشند (رنگ‌آمیزی همخوان با theme).

خروجی مطلوب:
- یک مخزن آمادهٔ قابل push یا یک آرشیو zip از ساختار بالا.
- README شامل دستورالعمل نشر روی GitHub Pages و نکات لازم برای جایگزینی لینک App Store، و اینکه برای فرم تماس از Formspree یا Netlify Forms استفاده شود.
- همهٔ HTMLها باید در سطح پایه قابل اعتبارسازی باشند (no broken links).

تذکر: لطفاً فایل‌ها را بدون اطلاعات حساس بساز و در متن‌ها از ایمیل پشتیبانی `ashnam084@gmail.com` و نام اپ `Mahdigeram` استفاده کن.

تشکر — وقتی کار تموم شد بگو تا من فایل‌ها رو بررسی و منتشر کنم.
