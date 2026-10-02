# Modern Web Guidance: Scroll-driven entry and exit effects

- platform: youtube
- url: https://www.youtube.com/watch?v=kbjHnZOQgkQ
- channel: Chrome for Developers
- published: 2026-09-29
- views: 10475
- duration_seconds: 132
- topic: scroll-driven animations / agent guidance

## خلاصه

ویدیوی کوتاه کروم دو ایجنت را کنار هم می‌گذارد تا افکت ورود و خروج اسکرول‌محور را پیاده کنند. سمت چپ بدون راهنما است و سمت راست مهارت Modern Web Guidance را در کانتکست دارد.

ایجنت بدون راهنما انیمیشن ورود و خروج را در یک بلوک می‌نویسد، با محاسبهٔ درصد و فرض نسبت ثابت بین ارتفاع کارت و ارتفاع ویوپورت. این با تغییر اندازهٔ کارت یا صفحه می‌شکند. ایجنت راهنما اول راهنمای «scroll entry exit» را پیدا می‌کند. در CSS برای `animation-timeline: view()` و `animation-range` تشخیص قابلیت می‌گذارد، دو کی‌فریم جدا (`slide in` و `slide out`) تعریف می‌کند و هر کدام را به بازهٔ خودش وصل می‌کند. در جاوااسکریپت اگر این APIها نباشند، فال‌بک `IntersectionObserver` است. ظاهر دو خروجی شبیه‌اند؛ نسخهٔ راست با تغییر ابعاد نمی‌شکند.

## نکته‌ها

- تفاوت در ظاهر نهایی نیست؛ در این است که ورود و خروج از هم جدا شده‌اند و نسبت ثابت ارتفاع فرض نشده.
- راهنمای پلتفرم داخل کانتکست ایجنت، جایگزینِ اختراع مجدد درصد و کی‌فریم واحد است.
