# نمایهٔ اجرا 2026-10-02-12

- تاریخ تهران: 2026-10-02، ساعت اجرا حدود ۱۲
- موضوعات از `schedule."2026-10-02"` (۱۲ مورد): میکروفرانت پروداکشن، فدراسیون در برابر iframe، وضعیت و مسیریابی مشترک، API پلتفرم وب، اخبار DevTools، تایپ‌اسکریپت/جاوااسکریپت، وب وایتال، ارکستراسیون ایجنت، نکتهٔ Claude/Cursor/Copilot، پرامپت ایجنت کدنویسی، دمو ایجنت خودمختار، یکپارچگی MCP
- حالت کانال‌ها: `mode: both` با `per_channel_limit: 5` و `max_age_days: 14` (جدیدتر از 2026-09-18)
- ترنسکریپت یوتیوب از متن صفحهٔ ویدیو. `yt-dlp` متادیتای جست‌وجو و فید را داد؛ دانلود پلیر/زیرنویس با دیوار «Sign in to confirm you’re not a bot» بسته شد. Whisper در محیط نصب نیست.

## اینستاگرام

فقط هندل‌های `config/instagram-accounts.yaml`. اکسپلور اسکرپ نشد. `yt-dlp` روی `/reels/` هر حساب یا به صفحهٔ لاگین خورد یا 429 گرفت. هیچ کپشن، ویو، یا صوت واقعی‌ای برنگشت؛ چیزی ساخته نشد.

| حساب | نتیجه |
|---|---|
| captainhoff | HTTP 429 |
| youraveragetechbro | HTTP 429 |
| mattmurphy | HTTP 429 |
| qendresahhoti | HTTP 429 |
| daniallqureshi | ریدایرکت لاگین |
| skip_ci | ریدایرکت لاگین |
| sicknider_raw | ریدایرکت لاگین |
| umacodes | ریدایرکت لاگین |
| haydenschmitty | ریدایرکت لاگین |
| rollins_io | ریدایرکت لاگین |
| chase_h_ai | ریدایرکت لاگین |
| khashayartalks | ریدایرکت لاگین |
| jam_with_ai | ریدایرکت لاگین |

## اصلاح هندل یوتیوب

سه هندل فایل کانال به سازندهٔ واقعی وصل نبودند و در همین اجرا اصلاح شدند:

- `@MatthewBerman` کانال کوکتیل ۲۰۱۱–۲۰۱۲ بود. هندل AI همان آدم، `@matthew_berman` است.
- `@mckaywrigley` خطای 404 داد. کانال `@realmckaywrigley` است؛ آخرین آپلود فید 2025-07-09، خارج از ۱۴ روز.
- `@ContinuousDelivery` خطای 404 داد. کانال فعلی Modern Software Engineering با هندل `@ModernSoftwareEngineeringYT` است.

## نگه داشته‌شده (متن قابل‌استفاده)

| فایل | کانال | تاریخ | چرا |
|---|---|---|---|
| [I_KVMFrUtPk.md](I_KVMFrUtPk.md) | Fireship | 2026-09-30 | گارد prompt injection بیرون حلقهٔ مدل |
| [No-JPdFvYWU.md](No-JPdFvYWU.md) | Fireship | 2026-10-01 | روایت Dev Day؛ با برچسب تفسیر کانال |
| [_mi3alkqy4s.md](_mi3alkqy4s.md) | AI Engineer / Laurie Voss | 2026-09-30 | گلوگاه ریویو، با عدد |
| [Se8jHLliLXE.md](Se8jHLliLXE.md) | AI Engineer / Justin Reock | 2026-09-30 | سرعت در برابر اعتماد و اندازهٔ PR |
| [UOcHfR3_tys.md](UOcHfR3_tys.md) | AI Engineer / Vlad Luzin | 2026-09-30 | MCP/A2A و حبس انفرادی ایجنت |
| [vukchAoaTdE.md](vukchAoaTdE.md) | Chrome for Developers | 2026-09-30 | DevTools 151–153 و MCP حافظه |
| [kbjHnZOQgkQ.md](kbjHnZOQgkQ.md) | Chrome for Developers | 2026-09-29 | اسکرول‌درایون با و بدون راهنمای پلتفرم |
| [btIOhb6AiOc.md](btIOhb6AiOc.md) | Chrome for Developers | 2026-09-28 | کاروسل CSS بدون جاوااسکریپت |
| [0isk_iLFCdk.md](0isk_iLFCdk.md) | Traversy Media | 2026-09-21 | هایپ مدل روز در برابر کار روی کد موجود |
| [wK5WgbqtI50.md](wK5WgbqtI50.md) | Modern Software Engineering | 2026-09-23 | TDD داخل حلقهٔ ایجنت در برابر کنت بک |
| [iPCa4CODwsU.md](iPCa4CODwsU.md) | Modern Software Engineering | 2026-09-29 | پلتفرم داخلی که مشتری ندارد |
| [JcIN0Alcr_4.md](JcIN0Alcr_4.md) | Dmitriy Zhiganov | 2026-05-30 | بهترین شرح موضوع میکروفرانت امروز؛ قدیمی‌تر از ۱۴ روز |
| [nX44PRZ6Pcc.md](nX44PRZ6Pcc.md) | Awesome | 2025-07-24 | مقایسهٔ کوتاه iframe و فدراسیون؛ قدیمی |

بازدیدها از yt-dlp یا Invidious در زمان همین اجراست، نه شمارندهٔ زنده.

## داخل پنجرهٔ ۱۴ روز، کوتاه‌فهرست نشد

متن این‌ها گرفته نشد تا اجرا در ویدیوهای تکراری خبر مدل غرق نشود.

- Fireship: `OuNKBjuV7A4` (2026-09-28، DHH)، `c1rPlzxSZ8E` (2026-09-25، Meta Connect)، `ylO0DQeVEBQ` (2026-09-23، وردپرس). بازدید بالا، دور از محور ریویو/پلتفرم/میکروفرانت این اجرا.
- Theo (`@t3dotgg`): `D8PikZ1KhUo` امروز منتشر شده (2026-10-02، حدود ۶۶ دقیقه). بقیهٔ پنج‌تای تازه هم خبر مدل‌اند (`vu8X3YroB-w`، `8WbW_n95wc4`، `IBcBKgYUghU`، `ejjBbaq9RmY`).
- Matthew Berman (`@matthew_berman`): `OODvXcQJyVo` (2026-10-01، Muse)، `Xc6ERvZM1NY` (2026-09-29، حدود ۹۶هزار بازدید)، `T-E7rmD6rh4`، `0NhtHVPQwt8`، `rgO5v8MFtFg`. هم‌پوشان با روایت Dev Day.
- AI Engineer: `apyrzaWj0Z4` (2026-10-02، حافظهٔ Qdrant، بازدید پایین)، `9cJrbj23fOA` (نقش Chief AI Officer).
- Chrome: `BFdsi7mimUI` (2026-10-01، شورت specificity؛ همان موضوع داخل `vukchAoaTdE` هست)، `nwauFPVDVEY` (state queries)، `9U4D5m24mhc` (swipe to remove).
- ByteByteGo: فقط `E5Ef_Kne17U` (2026-09-25، بازسازی یوتیوب، حدود ۴۳ دقیقه) داخل پنجره بود.
- Traversy: فقط `0isk_iLFCdk` داخل پنجره بود و نگه داشته شد.
- Matt Pocock: فقط لایو `MN9dGgmLyso` (2026-09-30) داخل پنجره بود.
- Modern Software Engineering: `LO60O07e2KU`، `T4qP5baf6r8`، `FXgNcAXzZwI`، `h3Ecz_0Zy0g` داخل پنجره‌اند و متن نگرفتند (کوتاه یا خارج از زاویهٔ پست‌ها).

## کانال بدون آپلود تازهٔ ۱۴ روز

- `@ThePrimeagen`: تازه‌ترین فید 2026-08-06
- `@jherr`: تازه‌ترین فید 2026-07-30
- `@WebDevSimplified`: تازه‌ترین فید 2026-09-15
- `@CodeAesthetic`: تازه‌ترین فید 2023-12-23
- `@realmckaywrigley`: تازه‌ترین فید 2025-07-09

## جست‌وجوی موضوع

برای هر ۱۲ موضوع حدود ۵ کاندیدا از `ytsearch` برگشت (سقف پلی‌لیست این اجرا). تقریباً هیچ میکروفرانتِ پرتکراری جدیدتر از ۱۴ روز نبود. `JcIN0Alcr_4` و `nX44PRZ6Pcc` به‌خاطر خود موضوع نگه داشته شدند. بقیهٔ نتایج جست‌وجو (شرح‌های قدیمی MCP، وب‌وایتال کم‌بازدید، خبر فرانت بی‌تاریخ قابل‌اتکا) وارد خلاصه نشدند تا URL و متریک ساختگی ساخته نشود.
