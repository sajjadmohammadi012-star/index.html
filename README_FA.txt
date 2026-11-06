OurJournal Daylight — بستهٔ نصب وب‌اپ (PWA)

این بسته نسخهٔ نهایی OurJournal_day_light.html را با همان آیکون‌های قبلی به PWA متصل می‌کند.

ساختار فایل‌ها را دقیقاً با همین نام‌ها در ریشهٔ سایت یا پوشهٔ اصلی پروژهٔ GitHub Pages قرار دهید:

- index.html  ← نسخهٔ Daylight با متادیتای آیکون و ثبت Service Worker
- manifest.webmanifest
- sw.js
- icons/
  - apple-touch-icon.png
  - favicon.svg
  - icon-192.png
  - icon-512.png
  - icon-maskable-512.png

نکته‌های مهم:
1) فقط آپلود کردن HTML کافی نیست؛ همهٔ فایل‌ها و پوشهٔ icons باید کنار آن و با همین مسیرها منتشر شوند.
2) سایت باید از طریق HTTPS باز شود (GitHub Pages به‌صورت پیش‌فرض HTTPS دارد). باز کردن فایل به‌صورت file:// نصب وب‌اپ را فعال نمی‌کند.
3) پس از انتشار، سایت را یک بار در مرورگر باز کنید تا فایل manifest و Service Worker بارگذاری شوند.

نصب روی Android:
Chrome → منوی سه‌نقطه → Install app یا Add to Home screen.

نصب روی iPhone:
صفحه را در Safari باز کنید → Share → Add to Home Screen.
آیکون iPhone از apple-touch-icon.png خوانده می‌شود.

اگر قبلاً نسخهٔ قدیمی را نصب کرده‌اید، آیکون/میانبر قبلی را حذف کنید، سایت را دوباره در مرورگر باز کنید و سپس دوباره Add to Home Screen را انجام دهید.
