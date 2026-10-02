# What's New: Chrome DevTools 151–153

- **عنوان:** What's New: Chrome DevTools 151–153
- **لینک:** https://www.youtube.com/watch?v=vukchAoaTdE
- **کانال:** Chrome for Developers
- **بازدید:** ۷٬۰۸۴ (طبق متادیتای جستجوی yt-dlp)
- **مدت:** حدود ۶ دقیقه
- **موضوع:** Chrome DevTools frontend news

## خلاصه

این قسمت اخبار DevTools برای کروم ۱۵۰ تا ۱۵۳ است و با یک تغییر انتشار شروع می‌شود: از کروم ۱۵۳ چرخه انتشار دسکتاپ و اندروید و iOS دو هفته‌ای شده تا قابلیت پلتفرم و رفع باگ زودتر برسد.

در پنل Network، بازپخش قدیمی XMLHttpRequest جایش را به fetch داده. روی هر درخواست: Resend همان را دوباره می‌فرستد، و Edit and resend as fetch یک دستور fetch آماده را در Console می‌ریزد تا هدر و پارامتر را قبل از Enter دستکاری کنی. کپی به‌صورت curl و PowerShell و fetch سر جایش است. ستون Preloaded نشان می‌دهد منبع preload شده یا نه، و Copy as preload element تگ link آماده را در کلیپ‌بورد می‌گذارد. تب payload برای WebSocket و قالب باینری، بیننده Base64 و hex و UTF-8 دارد.

در Styles، هاور روی سلکتور وزن specificity به شکل A,B,C را نشان می‌دهد تا `!important` از روی عادت ننویسی. هاور روی سلکتور والد در CSS nesting همان عنصر را روی صفحه روشن می‌کند. رابطه‌هایی مثل `popovertarget` به گره هدف وصل می‌شوند.

برای عامل‌ها، سرور MCP DevTools به دیباگ حافظه رسیده: heap snapshot و نشت از رشته‌های تکراری. آزمایشی هم هست که به‌جای JSON از یک کدگذاری فشرده‌تر برای حجم زیاد داده استفاده کند. در Performance، ناوبری نرم (soft navigation) جدا از ریلود کامل سنجیده می‌شود؛ الگوی پیش‌فرض SPAهایی مثل Next.js. در Console، خروجی `console.table` را می‌شود به‌صورت Markdown یا CSV کپی کرد.

## نکات کلیدی

- از کروم ۱۵۳ ریتم انتشار دو هفته است، روی دسکتاپ و موبایل.
- Resend و Edit-as-fetch بازپخش شبکه را به شکل fetch مدرن درآورده.
- Preload را هم می‌بینی هم به‌صورت تگ link کپی می‌کنی.
- payload باینری داخل خود DevTools خوانده می‌شود.
- tooltip specificity جایگزین حدس زدن و `!important` شانسی است.
- soft navigation در پنل Performance برای SPA اندازه‌گیری می‌شود، نه فقط full reload.
- MCP DevTools به حافظه و heap هم رسیده، علاوه بر DOM و شبکه.

## برش کوتاه

> `!important` معمولاً راه‌حل نیست؛ سلکتور است. از این به بعد وزن specificity را با هاور می‌بینی. و اگر SPA داری، پنل Performance دیگر هر جابه‌جایی URL را ریلود کامل فرض نمی‌کند.
