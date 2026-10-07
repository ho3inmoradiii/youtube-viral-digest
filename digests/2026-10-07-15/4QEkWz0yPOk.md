# قفل پل، نه قفل باینری

- platform: youtube
- url: https://www.youtube.com/watch?v=4QEkWz0yPOk
- channel: Alex Hitt
- title: REA GitHub Explained: Local Evidence Graphs for AI Coding Agents
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 7, 2026` نشان داد. Invidious `publishedText` را `12 hours ago` داد و `published` را `1791331200`، سطل نیمه‌شب
- views: صفحهٔ watch `6 views`. کمی بعد Invidious هم ۶ بازدید
- likes: عبارت لایک در HTML دیده نشد. Invidious کمی بعد ۰ لایک
- duration_seconds: ۵۵۳ از `/api/v1/videos/4QEkWz0yPOk?hl=en` روی `invidious.f5.si`
- metrics_source: HTML صفحهٔ watch و بعد اندپوینت Invidious
- topic: مرز امنیتی REA؛ توکن capability روی سوکت محلی، و اجرا با مجوز همان کاربر
- text_source: شرح صفحهٔ watch، `SECURITY.md` و `README.md` شاخهٔ `main` ریپوی `morluto/rea`، و `src/hopper/BridgeLauncher.ts` همان ریپو. گفتار نیامد. WebFetch صفحهٔ watch این اجرا ۴۰۳ داد. زیرنویس Invidious خالی بود. Whisper نصب نیست

## خلاصه

شرح ویدیو ریپو را https://github.com/morluto/rea معرفی می‌کند و می‌گوید REA سندباکس نیست، تحلیل با مجوز کاربر جاری سیستم است، و پل محلی را با توکن capability و سوکت یونیکس mode-0600 محدود می‌کند. همچنین می‌گوید تحلیل ایستای یک پروژهٔ اسباب‌بازی جاوااسکریپت بار را اجرا نمی‌کند و خروجی شواهد، رفتار پویای حل‌نشده را حدس نمی‌زند.

`SECURITY.md` که این اجرا از `main` خوانده شد این مرز را این‌طور می‌نویسد: هر نشست پل ارائه‌دهنده با یک توکن capability تصادفی و یک سوکت یونیکس کاربر جاری احراز می‌شود. توکن از توصیفگر نشست خصوصی رد می‌شود، نه از آرگومان پروسه و نه از متغیر محیط. همان بند می‌گوید این سندباکس نیست و در برابر پروسهٔ مخربی که از قبل با همان کاربر سیستم در حال اجراست محافظتی ندارد. باز کردن باینری نامطمئن، تجزیه و تحلیل را به ارائه‌دهندهٔ محلی با مجوز همان کاربر می‌سپارد.

در `src/hopper/BridgeLauncher.ts` فایل بوت‌استرپ با `mode: 0o600` نوشته می‌شود و بعد `chmod(bootstrapPath, 0o600)` دارد. این mode روی فایل بوت‌استرپ لانچر است. `SECURITY.md` خود سوکت را «current-user Unix socket» می‌نامد و عبارت mode-0600 را برای inode سوکت نمی‌آورد. شرح ویدیو این دو را یکی کرده است.

README در بخش Process Capture می‌گوید پروسه با مجوز کاربر اجرا می‌شود و Process Capture سندباکس امنیتی نیست. در بخش Security model می‌گوید تحلیل جاوااسکریپت ایستا ماژول‌های استخراج‌شده را اجرا نمی‌کند.

API گیت‌هاب همین اجرا برای `morluto/rea`: ۱۱۶۱۳ ستاره، مجوز MIT، `pushed_at` برابر `2026-10-07T12:06:24Z`. توضیح ریپو: «Reverse engineer anything with agents, from app behavior down to native binaries.»

## نکته‌های کلیدی

- سندباکس نبودن را خود `SECURITY.md` می‌گوید، نه فقط شرح ویدیو
- توکن از آرگومان و محیط رد نمی‌شود
- `0o600` در کدی که این اجرا باز شد مال فایل بوت‌استرپ است
- تحلیل ایستای جاوااسکریپت، ماژول استخراج‌شده را اجرا نمی‌کند
- ستاره و زمان push از API همین اجرا است

## چه وارد پست نشد

- ماتریس نسخهٔ Node، هشدار `.asar`، و مسیر WSL. در شرح هست و این اجرا در README خط‌به‌خط باز نشد
- ادعای شرح که سوکت خودش mode-0600 است. کد بازشده این را برای فایل بوت‌استرپ نشان داد
