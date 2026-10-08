# کوکی به BFF می‌رسد، توکن به جاوااسکریپت نه

- platform: youtube
- url: https://www.youtube.com/watch?v=DSk808dFVZc
- channel: WSO2
- title: Securing Modern Applications with the BFF Pattern and WSO2 Identity Server
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 7, 2026` نشان داد. Invidious `published` را `1791331200` داد، که سطل نیمه‌شب است
- views: صفحهٔ watch همین اجرا `3 views`. Invidious هم ۳
- likes: عبارت لایک در HTML صفحهٔ watch دیده نشد. Invidious `likeCount` ۰
- duration_seconds: ۱۳۸۳ از `/api/v1/videos/DSk808dFVZc?hl=en`
- metrics_source: HTML صفحهٔ watch و بعد اندپوینت Invidious
- topic: در الگوی BFF مرورگر توکن را نمی‌بیند و فقط کوکی نشست را به BFF می‌دهد
- text_source: شرح صفحهٔ watch برای نام ارائه‌دهنده، و گفتار WebFetch. Whisper نصب نیست

## خلاصه

شرح ویدیو ارائه‌دهنده را Cedric Guyomard می‌نامد، معمار IAM امنیت در AZQORE، و می‌گوید این مورد در WSO2Con Africa 2026 ارائه شده. موضوع شرح: SPA و میکروفرانت با OAuth معمولی توکن را در مرورگر می‌گذارد.

در گفتار، SPA کاملاً داخل مرورگر است. کد مجوز را خود SPA با سرور هویت عوض می‌کند و access token، و در صورت وجود refresh token، در localStorage یا حافظه می‌ماند. می‌گوید جاوااسکریپت به آن می‌رسد. XSS را دزدیدن همین توکن و مصرف API به‌جای کاربر می‌داند. مدت «access حدود یک ساعت» و «refresh مثلاً هشت ساعت» را با let's say گفت. این مدت پیکربندی ثبت‌شدهٔ سامانه نیست.

FAPI 2.0 را پروتکل تازه نخواند. گفت پروفایل امنیتی روی OIDC و OAuth 2 است و از بانکداری باز و PSD2 آمده. چهار تکیه را نام برد. درخواست اول احراز از جاوااسکریپت رد نشود و از کانال پشتی برود. PKCE تا کد مجوز دزدیده‌شده به‌تنهایی عوض نشود. SPA به‌طور پیش‌فرض کلاینت عمومی است و برای کلاینت محرمانه private key JWT یا mutual TLS را نام برد. توکن را هم به سرور مقید کرد تا دزدیدنش برای مصرف جای دیگر کافی نباشد.

الگوی BFF در گفتار: مرورگر فقط با کوکی secure و SameSite و HttpOnly با BFF حرف می‌زند. BFF کلاینت OAuth است و گردش ورود را با Identity Server انجام می‌دهد. فراخوانی API از مرورگر با کوکی می‌آید. BFF در session store، که گفت می‌تواند دیتابیس یا Redis باشد، توکن متناظر کوکی را پیدا می‌کند، آن را در هدر Authorization می‌گذارد و به API می‌فرستد. گفت مرورگر access token و refresh token و client secret را نمی‌بیند.

یک عدد نسخه در گفتار شبیه «5.2.0» درآمد و با FAPI 2.0 که خودش نام برده بود جور خوانده نشد. در پست نیست.

## نکته‌های کلیدی

- توکن SPA در localStorage یا حافظه، در دسترس جاوااسکریپت
- BFF کلاینت OAuth است و مرورگر فقط کوکی HttpOnly می‌فرستد
- BFF توکن را از نشست برمی‌دارد و در Authorization می‌گذارد
- مدت یک ساعت و هشت ساعت مثال گفتار است
- FAPI 2.0 را پروفایل روی OIDC و OAuth 2 خواند، نه پروتکل تازه

## چه وارد پست نشد

- مدت‌های let's say
- جملهٔ نامفهوم نسخه
- ادعای «هر مقرراتی را از دست می‌دهی» بدون نام سند
