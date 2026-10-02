# Securing the Agentic Enterprise: Zero-Trust APIs and Sandboxed Micro-Frontends

- platform: youtube
- url: https://www.youtube.com/watch?v=uN2UKIeIiPM
- channel: ConfEngine
- speaker: Shuva Jyoti Kar, Principal Engineer, Palo Alto Networks
- published: 2026-09-28
- views: 28
- likes: 0
- duration_seconds: 1840
- topic: MCP Apps, sandboxed React microfrontends, agent API security
- conference: apidays India 2026 (case study, API security and resiliency)
- text_source: شرح جلسه در صفحهٔ ویدیو. زیرنویس در این اجرا بسته بود. بازدید پایین است و محتوای خلاصه از همان شرح است، نه از حدس.

## خلاصه

شرح، دادن دسترسی مستقیم LLM به ده‌ها هزار ردیف JSON خام تله‌متری را هم اضافه بار شناختی می‌داند و هم شکست تاب‌آوری و امنیت. تکیه بر مدل غیرقطعی برای payloadهای بزرگ را به توهم، باد کردن پنجرهٔ کانتکست، و ورک‌فلوی شکسته وصل می‌کند.

پیشنهاد جلسه: جدا کردن استدلال از رندر، با MCP که آن را «تازه تثبیت‌شده» می‌خواند و افزونهٔ Apps. به‌جای payload خام، API ایجنتی یک میکروفرانت React تعاملی و قطعی برمی‌گرداند. دادهٔ زنده از بک‌اند (مثال شرح: ClickHouse) گرفته و داخل فضای کار ایجنت رندر می‌شود. مکانیک امنیت در شرح: اعتبار دیتابیس روی سرور MCP می‌ماند، iframe سخت سندباکس می‌شود تا به DOM و کوکی دسترسی نباشد، و همگام‌سازی دوطرفهٔ زمینه بین UI و حافظهٔ ایجنت از کانال قابل‌ممیزی JSON-RPC و postMessage رد می‌شود.

## نکته‌ها

- مرز این میکروفرانت، استقلال تیم‌های محصول نیست؛ مرز اعتماد بین مدل و داده است.
- مدل نباید جدول خام را «بفهمد» تا بعد رندر کند. رندر قطعی بیرون حلقهٔ غیرقطعی می‌ماند.
- اعتبار دیتابیس داخل سشن مدل جایی ندارد.
- این خلاصه ادعای شرح جلسه است. دموی زنده جداگانه تأیید نشد چون ترنسکریپت در دسترس نبود.
