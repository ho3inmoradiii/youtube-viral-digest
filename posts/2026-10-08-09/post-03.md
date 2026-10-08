# توکن آن طرف کوکی ماند

SPA کد مجوز را خودش عوض می‌کند و توکن را در مرورگر می‌گذارد.
در این ارائه، مرورگر دیگر توکن را نمی‌بیند.

سدریک گیومار، معمار IAM در AZQORE، این را در WSO2Con Africa 2026 گفت. ویدیوی WSO2 تاریخ watch را ۷ اکتبر ۲۰۲۶ دارد و همین اجرا ۳ بازدید داشت. گفت access token، و اگر باشد refresh token، در localStorage یا حافظه می‌ماند و جاوااسکریپت به آن می‌رسد. XSS را برداشتن همین توکن و زدن API به‌جای کاربر خواند. «حدود یک ساعت» و «مثلاً هشت ساعت» را با let's say گفت. آن مدت‌ها تنظیم ثبت‌شدهٔ یک سامانه نیست.

BFF را کلاینت OAuth گذاشت. مرورگر فقط با کوکی secure و SameSite و HttpOnly با آن حرف می‌زند. کلیک ورود به BFF می‌رسد. BFF گردش را با Identity Server انجام می‌دهد. وقتی صفحه API می‌خواهد، همان کوکی را می‌فرستد. BFF در session store، که گفت دیتابیس یا Redis، توکن همان کوکی را پیدا می‌کند و در هدر Authorization می‌گذارد. گفت مرورگر access token و refresh token و client secret را نمی‌بیند.

FAPI 2.0 را پروتکل تازه نخواند. گفت پروفایل روی OIDC و OAuth 2 است. چهار تکیه را نام برد: درخواست اول احراز از کانال پشتی، PKCE، کلاینت محرمانه با private key JWT یا mutual TLS، و توکن مقید به سرور. یک عدد نسخه در گفتار نامفهوم بود و این‌جا نیست.

آخرین لاگین فرانت‌تان توکن را به جاوااسکریپت داد، یا فقط یک کوکی HttpOnly؟

#BFF #OAuth #FAPI #میکروفرانت #امنیت #فرانت‌اند

---
source_videos:
  - title: "Securing Modern Applications with the BFF Pattern and WSO2 Identity Server"
    url: https://www.youtube.com/watch?v=DSk808dFVZc
topic: browser sends an HttpOnly cookie; the BFF attaches the access token
generated_at: 2026-10-08T09:55:00+03:30
