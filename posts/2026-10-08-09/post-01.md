# نقش را سرور عوض نمی‌کند

جدول GA فابریک برای سپتامبر ۲۰۲۶ می‌گوید Core MCP دسترسی حسابرسی‌شده می‌دهد.
همان صفحه، جست‌وجوی کاتالوگ OneLake را هنوز پیش‌نمایش خوانده و گفته همین قابلیت ابزار داخلی همان سرور است.

ردیف را این اجرا از https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new خواند: `Fabric Core MCP Server (Generally Available)`. جملهٔ ردیف: دسترسی احرازشده و حسابرسی‌شده به ورک‌اسپیس، آیتم، مجوز، جست‌وجو، و ظرفیت. چند ردیف بالاتر، هنوز زیر جدول پیش‌نمایش: `OneLake Catalog search API, MCP, and CLI tools (Preview)`. متنش می‌گوید این قابلیت ابزار داخلی Fabric Core MCP server هم هست.

ویدیوی ماتیاس فالاند، ۷ اکتبر ۲۰۲۶، همان GA را می‌گوید. نمای کلی Learn اندپوینت را `https://api.fabric.microsoft.com/v1/mcp/core` گذاشته. ورود با Entra ID در مرورگر است. سرور API را با مجوز هویت واردشده صدا می‌زند. صفحهٔ مقایسه می‌گوید وصل کردن سرور MCP خودش مجوز تازه نمی‌دهد، و هویت اجرا می‌تواند با کسی که پای کلاینت نشسته فرق کند. اگر در ورک‌اسپیس Admin هستی، ایجنت با همان نقش Admin است. ابزارهای مدیریت منبع برای کوئری جدول lakehouse نیستند.

حسابرسی را همان مقاله باریک کرده. عملیات پشتیبانی‌شدهٔ Core با هویت اجراکننده ثبت می‌شود. جملهٔ بعدی: فرض نکن هر فراخوانی ابزار MCP در لاگ حسابرسی فابریک می‌آید. سرور محلی خودش این لاگ را نمی‌نویسد. عملیات زنده‌اش ممکن است سمت سرویس زیرین بماند. ملاحظات Core: کلاینت خودمختار یا بدپیکربندی ممکن است کار مخرب کند. پرچم بستن کار مخرب در مشخصات MCP استاندارد نیست. شروع سریع، قبل از مثال «یک ورک‌اسپیس بساز» و «این آدرس را Contributor کن»، می‌گوید فراخوانی ابزار و تنظیم تأیید کلاینت را ببین. بازدید ویدیو ۲۳۳ بود و عبارت لایک ۲۰۳ نفر دیگر.

آخرین ایجنتی که به فابریک وصل کردی، با حساب Admin بود یا با حسابی که فقط می‌بیند؟

#فابریک #MCP #حسابرسی #RBAC #ایجنت #مهندسی_نرم‌افزار

---
source_videos:
  - title: "Fabric Core MCP Server: What an AI Agent Can Do in Your Tenant"
    url: https://www.youtube.com/watch?v=N1CPzwb2210
  - title: "What's new in Microsoft Fabric"
    url: https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new
  - title: "Fabric Core MCP Server overview"
    url: https://learn.microsoft.com/en-us/rest/api/fabric/articles/mcp-servers/core-remote/overview-core-mcp-server
  - title: "Fabric MCP Servers overview"
    url: https://learn.microsoft.com/en-us/rest/api/fabric/articles/mcp-servers/what-is-fabric-mcp-server
topic: GA row and preview catalog-search row, agent keeps the signed-in role
generated_at: 2026-10-08T09:55:00+03:30
