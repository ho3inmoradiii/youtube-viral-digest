# نقش، با وصل شدن سرور عوض نمی‌شود

- platform: youtube
- url: https://www.youtube.com/watch?v=N1CPzwb2210
- channel: Matthias Falland -The Trusted Advisor- Fabric & AI
- title: Fabric Core MCP Server: What an AI Agent Can Do in Your Tenant
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 7, 2026` نشان داد. Invidious `published` را `1791331200` داد، که سطل نیمه‌شب است
- views: صفحهٔ watch همین اجرا `233 views`. Invidious همان عدد
- likes: عبارت صفحهٔ watch `along with 203 other people`. Invidious `likeCount` ۲۰۳
- duration_seconds: ۲۶۲ از `/api/v1/videos/N1CPzwb2210?hl=en` روی `invidious.f5.si`
- metrics_source: HTML صفحهٔ watch و بعد اندپوینت Invidious
- topic: سرور GA است و ایجنت با نقش همان هویت واردشده کار می‌کند
- text_source: گفتار صفحهٔ watch از WebFetch، به‌اضافهٔ صفحه‌های Learn که همین اجرا باز شد. Whisper نصب نیست

## خلاصه

ویدیو می‌گوید Fabric Core MCP Server در What’s new سپتامبر ۲۰۲۶ عموماً در دسترس است. جدول GA در https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new همان ردیف را دارد: `September 2026 | Fabric Core MCP Server (Generally Available)` و می‌گوید ایجنت‌های سازگار دسترسی احرازشده و حسابرسی‌شده به ورک‌اسپیس، آیتم، مجوز، جست‌وجو، و ظرفیت می‌گیرند.

همان صفحه، بالاتر، زیر «Features currently in preview» این ردیف را دارد: `OneLake Catalog search API, MCP, and CLI tools (Preview)`. متن ردیف می‌گوید همین قابلیت به‌عنوان ابزار داخلی Fabric Core MCP server هم هست.

نمای کلی https://learn.microsoft.com/en-us/rest/api/fabric/articles/mcp-servers/core-remote/overview-core-mcp-server اندپوینت را `https://api.fabric.microsoft.com/v1/mcp/core` می‌گذارد. ورود، OAuth در مرورگر با Entra ID است. ایجنت ابزار را انتخاب می‌کند و سرور API فابریک را با مجوز هویت احرازشده صدا می‌زند. عملیات پشتیبانی‌شده در لاگ حسابرسی با همان هویت ثبت می‌شود. ابزارهای مدیریت منبع برای کوئری یا تغییر دادهٔ جدول lakehouse نیستند.

صفحهٔ مقایسه https://learn.microsoft.com/en-us/rest/api/fabric/articles/mcp-servers/what-is-fabric-mcp-server می‌گوید وصل کردن سرور MCP خودش مجوز فابریک اضافه نمی‌کند. عملیات زنده با مجوز هویت احرازشده است و این هویت می‌تواند با کسی که پای کلاینت نشسته فرق داشته باشد. همان صفحه: فابریک عملیات پشتیبانی‌شدهٔ Core را با هویت اجراکننده ثبت می‌کند. سرور محلی خودش لاگ حسابرسی فابریک نمی‌نویسد. لاگ تشخیصی و تله‌متری‌اش جای رد حسابرسی نیست. عملیات زنده از سرور محلی ممکن است سمت سرویس زیرین ثبت شود. جملهٔ صریح صفحه: فرض نکن هر فراخوانی ابزار MCP در لاگ حسابرسی فابریک می‌آید.

ملاحظات همان نمای کلی: کلاینت خودمختار یا بدپیکربندی ممکن است کار مخرب انجام دهد. پرچمی که کار مخرب را ببندد در مشخصات MCP استاندارد نیست و هر کلاینت آن را ندارد. شروع سریع می‌گوید بعضی مثال‌ها منبع می‌سازند یا دسترسی را عوض می‌کنند و قبل از اجازه باید فراخوانی ابزار و تنظیم تأیید کلاینت دیده شود. یکی از مثال‌ها ساخت ورک‌اسپیس است و یکی افزودن Contributor.

ویدیو همین مرزها را می‌گوید: وصل شدن مجوز اضافه نمی‌دهد، Admin ماندن یعنی ایجنت هم Admin است، و Core دادهٔ جدول lakehouse را عوض نمی‌کند. قیمت جدا در Learn ندید و عددی نداد. این اجرا هم قیمتی در این صفحه‌ها ندید.

## نکته‌های کلیدی

- ردیف GA سپتامبر ۲۰۲۶ برای Fabric Core MCP Server روی صفحهٔ What’s New هست
- ردیف جست‌وجوی کاتالوگ OneLake هنوز زیر پیش‌نمایش است و می‌گوید ابزار داخلی همین سرور است
- وصل کردن سرور مجوز تازه نمی‌دهد. عملیات با نقش هویت واردشده است
- حسابرسی برای عملیات پشتیبانی‌شده است. صفحه می‌گوید هر فراخوانی ابزار را فرض نکن
- سرور محلی خودش لاگ حسابرسی فابریک نمی‌نویسد

## چه وارد پست نشد

- قیمت. نه ویدیو عدد داد، نه این صفحه‌ها
- ادعای Solv یا Atlan دربارهٔ «هر عملیات» در لاگ. صفحهٔ Learn خودش این تعمیم را نمی‌دهد
