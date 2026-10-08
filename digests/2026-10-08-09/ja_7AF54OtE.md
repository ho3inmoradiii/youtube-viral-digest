# نیت ذخیره شده، اثر هنوز یک‌بار نیست

- platform: youtube
- url: https://www.youtube.com/watch?v=ja_7AF54OtE
- channel: 0xSero
- title: Pi Durable: Agents That Survive Crashes — Mario Zechner & Armin Ronacher
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 7, 2026` نشان داد. Invidious `published` را `1791331200` داد، که سطل نیمه‌شب است
- views: صفحهٔ watch همین اجرا `11,302 views`. کمی بعد Invidious ۱۱۳۴۷
- likes: عبارت صفحهٔ watch `along with 218 other people`. Invidious هم ۲۱۸
- duration_seconds: ۳۴۶۲ از `/api/v1/videos/ja_7AF54OtE?hl=en`
- metrics_source: HTML صفحهٔ watch و بعد اندپوینت Invidious
- topic: ساندویچ نیت و اجرا، در برابر بازپخش فقط وقتی ابزار `replay: "safe"` است
- text_source: گفتار WebFetch صفحهٔ watch، README خام `packages/durable/README.md` روی `earendil-works/pi` در main، و فرادادهٔ npm و API گیت‌هاب. Whisper نصب نیست

## خلاصه

آرمین روناخر در گفتار، قبل از اجرای کار، یک رکورد ذخیره می‌کند که می‌گوید این ورودی‌ها قرار است اجرا شوند. اگر پروسه بعد از این ذخیره و قبل از اجرا بمیرد، بعد از بالا آمدن همان کار را انجام می‌دهد، چون هنوز اجرا نشده. اگر سیستم بیرونی با یک شناسه بگوید همین کار در حال اجراست، صبر می‌کند. مثالش شناسهٔ یک run در گیت‌هاب است. این را idempotency می‌نامد. بعد از تمام شدن اثر، نتیجه را ذخیره می‌کند. خودش این سه لایه را effect sandwich می‌خواند: نیت، اجرای اثر، ذخیرهٔ نتیجه. می‌گوید بعد از داشتن نتیجه، دیگر لازم نیست به جزئیات وسط ساندویچ برگردد.

README بسته روی https://raw.githubusercontent.com/earendil-works/pi/main/packages/durable/README.md هنوز خط اول بدنه را Experimental می‌گذارد و می‌گوید API بین انتشارها بدون اطلاع عوض می‌شود. هر فراخوانی ابزار وظیفهٔ جداست. نیت قبل از `execute()` کامیت می‌شود. اگر پروسه وسط فراخوانی بمیرد، ابزار فقط وقتی دوباره اجرا می‌شود که `replay: "safe"` اعلام شده باشد. وگرنه مدل نتیجهٔ خطای `interrupted` می‌گیرد، همراه خروجی‌ای که تا همان لحظه کامیت شده. `requestId` تکراری روی `submit` همان submission قبلی را برمی‌گرداند و بار دوم ثبت نمی‌کند. شروع سریع از `MemoryStorage` است. بخش Persist می‌گوید برای ماندن بعد از ری‌استارت SQLite یا JSONL باز شود و `resume()` کار ناتمام را ادامه دهد.

npm همین اجرا: `@earendil-works/pi-durable` نسخهٔ `1.1.0`، زمان انتشار `2026-10-07T22:10:38.752Z`، توضیح بسته «Durable conversation, task, and document runtime for Pi». API گیت‌هاب `earendil-works/pi`: ۱۱۳۲۷۵ ستاره، MIT، push در `2026-10-07T22:23:27Z`.

## نکته‌های کلیدی

- گفتار: ذخیرهٔ نیت قبل از اجرا، و اجرای بعد از کرش فقط اگر اثر هنوز شروع نشده
- گفتار: اگر سیستم بیرونی با همان شناسه بگوید در حال اجراست، صبر کن
- README: وسط `execute()` فقط با `replay: "safe"` دوباره اجرا می‌شود
- `requestId` تکرارِ submission را برمی‌گرداند
- `MemoryStorage` شروع سریع است. دوام ری‌استارت مال SQLite یا JSONL است

## چه وارد پست نشد

- ماجرای کرک نرم‌افزار و بازپخش حمله. به دوام ابزار مربوط نیست
- جملهٔ ماریو دربارهٔ فوریه تا ژوئیه و بی‌اعتمادی به ایجنت برای بستن issue. اندازه‌ای در آن نیست
- جزئیات Chord و نام مدل `gpt-6-sol` در نمونهٔ کد README. این اجرا آن مدل را جدا چک نکرد
