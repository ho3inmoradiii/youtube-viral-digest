# What's New: Chrome DevTools 151-153

- platform: youtube
- url: https://www.youtube.com/watch?v=vukchAoaTdE
- channel: Chrome for Developers
- published: 2026-09-30
- views: 7137
- duration_seconds: 370
- topic: Chrome DevTools / web platform

## خلاصه

ویدیو تازه‌های DevTools حول کروم ۱۵۰ تا ۱۵۳ را مرور می‌کند (عنوان روی ۱۵۱ تا ۱۵۳ است). از کروم ۱۵۳ چرخهٔ انتشار دسکتاپ و اندروید و iOS دو هفته‌ای شده تا فیچر پلتفرم زودتر برسد.

در پنل Network، به‌جای replay قدیمی: Resend همان درخواست را دوباره می‌فرستد، و Edit and resend as fetch یک دستور `fetch` پر شده را در کنسول می‌گذارد. کپی همچنان curl و PowerShell و fetch را دارد. ستون Preloaded نشان می‌دهد منبع preload شده یا نه، و Copy as preload element تگ `link` آماده می‌دهد. برای WebSocket و قالب باینری، تب payload بینندهٔ Base64 و hex و UTF-8 دارد.

در Styles، هاور روی سلکتور tooltip ویژگی‌پذیری (specificity) با تفکیک وزن را نشان می‌دهد. هاور روی سلکتور والد داخل قانون تودرتو، عنصر منطبق را روی صفحه هایلایت می‌کند. ویژگی‌هایی مثل `popovertarget` به گرهٔ هدف وصل می‌شوند.

برای ایجنت‌ها، سرور MCP دوآپس گسترش یافته: دیباگ حافظه، هیپ‌اسنپ‌شات، و نشت از تکرار رشته. آزمایشی هم هست که به‌جای JSON از encoding فشرده برای حجم زیاد استفاده کند. در پنل Performance متریک soft navigation آمده؛ ناوبری SPA که URL عوض می‌شود ولی JS و استایل زنده می‌مانند، با برچسب soft nav از ریلود کامل جدا می‌شود. در کنسول، `console.table` را می‌شود به‌صورت مارک‌داون یا CSV کپی کرد.

## نکته‌ها

- specificity و preload و replay درخواست از حدس ایجنت به ابزار قابل‌مشاهده منتقل شده‌اند.
- soft navigation متریک جدا از ریلود کامل است؛ برای نکست و SPA لازم است.
- MCP دوآپس دیگر فقط DOM نیست؛ هیپ هم به ایجنت رسیده، همراه با هشدار ضمنی حجم داده.
