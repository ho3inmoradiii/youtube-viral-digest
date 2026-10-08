# ساندویچ، مجوز پخش دوباره نیست

آرمین می‌گوید قبل از اجرا نیت را بنویس.
اگر پروسه همان‌جا بمیرد و اثر هنوز شروع نشده، بعد از بالا آمدن همان کار را بکن.

این را در گفت‌وگوی ۷ اکتبر ۲۰۲۶ با ماریو زشنر گفت، روی کانال 0xSero. اسم سه‌لایه را effect sandwich گذاشت: نیت، اجرای اثر، ذخیرهٔ نتیجه. مثال بیرونی‌اش شناسهٔ یک run در گیت‌هاب است. اگر همان شناسه را بدهی و سیستم بگوید در حال اجراست، صبر کن. این را idempotency خواند. بعد از ذخیرهٔ نتیجه گفت دیگر لازم نیست جزئیات وسط ساندویچ را نگه داری.

README `@earendil-works/pi-durable` روی main هنوز Experimental است و می‌گوید API بین انتشارها بدون اطلاع عوض می‌شود. npm همین اجرا نسخه را `1.1.0` نشان داد، زمان `2026-10-07T22:10:38.752Z`. نیت قبل از `execute()` کامیت می‌شود. اگر پروسه وسط خود فراخوانی بمیرد، ابزار فقط وقتی دوباره اجرا می‌شود که `replay: "safe"` اعلام شده باشد. وگرنه مدل نتیجهٔ `interrupted` می‌گیرد، با خروجی‌ای که تا همان‌جا مانده. `requestId` تکراری همان submission را برمی‌گرداند. این قفل پذیرش درخواست است. شروع سریع README حافظهٔ پروسه است. ماندن بعد از ری‌استارت را به SQLite یا JSONL و `resume()` سپرده. API گیت‌هاب `earendil-works/pi` همین اجرا: ۱۱۳۲۷۵ ستاره، MIT، push در `2026-10-07T22:23:27Z`. بازدید ویدیو روی صفحهٔ watch ۱۱۳۰۲ بود و کمی بعد Invidious ۱۱۳۴۷. عبارت لایک ۲۱۸ نفر دیگر.

آخرین ابزاری که بعد از کرش دوباره صدا زدی، `replay: "safe"` داشت یا فقط نیتش روی دیسک بود؟

#Pi #durable #idempotency #ایجنت #مهندسی_نرم‌افزار #harness

---
source_videos:
  - title: "Pi Durable: Agents That Survive Crashes — Mario Zechner & Armin Ronacher"
    url: https://www.youtube.com/watch?v=ja_7AF54OtE
  - title: "@earendil-works/pi-durable README"
    url: https://github.com/earendil-works/pi/blob/main/packages/durable/README.md
  - title: "@earendil-works/pi-durable on npm"
    url: https://www.npmjs.com/package/@earendil-works/pi-durable
topic: intent-before-execute versus replay only when the tool says safe
generated_at: 2026-10-08T09:55:00+03:30
