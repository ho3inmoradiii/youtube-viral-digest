# نمایهٔ اجرا 2026-10-03-03

- تاریخ تهران: 2026-10-03، حدود ساعت ۰۳:۴۰ تا ۰۴:۱۰
- موضوعات از `schedule."2026-10-03"` (۸ مورد): میکروفرانت ۲۰۲۶، Module Federation، روند معماری فرانت، اخبار وب این هفته، CSS مدرن، نکتهٔ ایجنت، گردش‌کار عامل کدنویسی، الگوی RAG و tool calling
- حالت کانال‌ها: `mode: both`، `per_channel_limit: 5`، `max_age_days: 14` (جدیدتر از 2026-09-19)
- شناسهٔ کانال از `rel=canonical` صفحهٔ هندل. اولین `"channelId"` داخل HTML مال کانال دیگری در صفحه است و استفاده نشد
- تاریخ و بازدید کانال‌های فهرست از فید RSS یوتیوب (`feeds/videos.xml?channel_id=`)
- جست‌وجوی موضوع: Invidious `invidious.f5.si` با `sort_by=upload_date`، حدود ۱۰ نتیجه برای هر موضوع
- گفتار کوتاه‌فهرست از متن صفحهٔ watch. `yt-dlp` 2026.08.19 بدون کوکی هنوز به دیوار ربات می‌خورد. بدنهٔ کپشن Invidious خالی برگشت. `youtube-transcript-api` روی این IP مسدود است. Whisper نصب نیست
- پیش‌نویس ساعت ۰۰:۴۰ همین شب (`digests/2026-10-03-00` روی شاخهٔ `cursor/youtube-instagram-digest-posts-bd82`) سهمیهٔ توکن Kimchi، مالیات هارنس، میکروفرانت چومک، و SlopCodeBench را پست کرده. آن چهار زاویه این‌جا تکرار نشد

## اینستاگرام

فقط هندل‌های `config/instagram-accounts.yaml`. اکسپلور اسکرپ نشد. `prefer_reels: true` و سقف هر حساب ۵.

`web_profile_info` برای `captainhoff` قبل از محدودیت جواب داد. دوازده پست عمومی برگشت؛ پنج Reel تازه در جدول پایین است. کپشن‌ها تیتر چندخطی‌اند، نه شرح قابل‌خلاصه. `yt-dlp` روی یکی از همان Reelها همان کپشن را داد و صوت جداگانه پیاده نشد، چون Whisper در محیط نیست. صفحهٔ Reel در واکشی بعدی فقط «۳۹ دقیقه پیش» برگرداند، بدون متن اضافه.

بلافاصله بعد از همان درخواست، دوازده حساب دیگر و تکرار خود `captainhoff` روی `www.instagram.com` و `i.instagram.com` با HTTP 429 جواب دادند. `yt-dlp` روی `/reels/` هم ۴۲۹ شد. برای آن حساب‌ها کپشن و ویو و زمان واقعی نیامد و چیزی ساخته نشد.

| حساب | نتیجه |
|---|---|
| captainhoff | پروفایل عمومی خوانده شد. پنج Reel تازه کپشن کوتاه دارند. خلاصه ساخته نشد |
| daniallqureshi | HTTP 429 |
| youraveragetechbro | HTTP 429 |
| skip_ci | HTTP 429 |
| sicknider_raw | HTTP 429 |
| mattmurphy | HTTP 429 |
| umacodes | HTTP 429 |
| qendresahhoti | HTTP 429 |
| haydenschmitty | HTTP 429 |
| rollins_io | HTTP 429 |
| chase_h_ai | HTTP 429 |
| khashayartalks | HTTP 429 |
| jam_with_ai | HTTP 429 |

پنج Reel تازهٔ `captainhoff`، از همان پاسخ پروفایل. لایک و ویو مال همان پاسخ است.

| زمان UTC | shortcode | لایک | ویو | درازا کپشن | چرا خلاصه نشد |
|---|---|---|---|---|---|
| 2026-10-02 23:34 | [DeArKRXAC2r](https://www.instagram.com/reel/DeArKRXAC2r/) | 1 | 15 | ۱۷۲ | تیتر «Become the Director of AI» و هشتگ. گفتار نیست |
| 2026-10-02 00:47 | [Dd-OoneAaKl](https://www.instagram.com/reel/Dd-OoneAaKl/) | 81 | 1486 | ۱۵۲ | تیتر «How to Become AI Native» |
| 2026-10-01 00:47 | [Dd7p2k6DYSM](https://www.instagram.com/reel/Dd7p2k6DYSM/) | 14 | 331 | ۱۲۷ | تیتر «The Key to AI Leadership» |
| 2026-09-30 00:46 | [Dd5E_TViTYW](https://www.instagram.com/reel/Dd5E_TViTYW/) | 79 | 1288 | ۱۴۸ | تیتر «Build an AI-Native Business» |
| 2026-09-29 00:26 | [Dd2d3BEjhF7](https://www.instagram.com/reel/Dd2d3BEjhF7/) | 186 | 3260 | ۱۷۳ | تیتر «Which AI Model is the Best?» |

## نگه داشته‌شده

هر چهار تا گفتار دارند. زاویه‌شان با پیش‌نویس ۰۰:۴۰ و با پست‌های ۱۲ و ۲۱ دیروز یکی نیست.

| فایل | منبع | تاریخ | چرا |
|---|---|---|---|
| [5xi_S1f9sDU.md](5xi_S1f9sDU.md) | AI Engineer / Derek Meegan | 2026-10-02T21:30:15Z | بعد از اجرای ۰۰:۴۰ به فید آمده. ۹۹٪ در هر قدم |
| [HLTa7Vcs4X0.md](HLTa7Vcs4X0.md) | AI Engineer / Gabriel Spencer-Harper | 2026-10-02T21:30:22Z | همان پنجره. تأیید فرانت، نه ریویوی دیروز |
| [y-OVWZD4j6U.md](y-OVWZD4j6U.md) | AI Engineer / Eric Schwartz | 2026-10-02T23:30:30Z | تازه‌ترین صحبت کانال در این فید. بازدید RSS پایین، متن کامل |
| [qwnJJMNGwgY.md](qwnJJMNGwgY.md) | Cole Medin | 2026-09-30 | Jev داخل هوک و ساندویچ مدل. از طبقه‌بند فایِرشیپِ اجرای ۲۱ جداست |

بازدید سه ویدیوی AI Engineer از RSS همین اجراست. برای `5xi_S1f9sDU` صفحهٔ watch کمی بعد ۴۶۰ نشان داد. بازدید کول مدین از همان صفحهٔ watch است، نه RSS، چون کانال فهرست ما نیست.

## کانال‌ها

پنج آپلود تازهٔ `@aiDotEngineer` در این فید، همهٔ ۲۰۲۶-۱۰-۰۲:

- `y-OVWZD4j6U`، `FQwTqUmcbRg`، `HLTa7Vcs4X0`، `5xi_S1f9sDU` نگه داشته یا رد شدند، پایین‌تر.
- `48YUYDjwfYY` (Kimchi، ۲۰:۰۰ UTC، حدود ۲۰۴۳ بازدید RSS) در پیش‌نویس ۰۰:۴۰ خلاصه و پست شده. این‌جا تکرار نشد.

`FQwTqUmcbRg` («Lessons from Generating 12 Trillion Synthetic Tokens»، ۲۰۲۶-۱۰-۰۲T۲۳:۳۰:۲۷Z، ۲۳ بازدید RSS) شرحش خط لولهٔ دادهٔ مصنوعی است: S3، GPU، Ray، vLLM. به حرف ایجنت کدنویسی و فرانت این اجرا نچسبید و گفتارش جدا گرفته نشد.

بقیهٔ کانال‌ها آپلود تازه‌تر از نمایهٔ ۲۱ و پیش‌نویس ۰۰ نداشتند، یا همان پنجرهٔ قبلی است.

بدون آپلود تازهٔ ۱۴ روز:

- `@ThePrimeagen`: تازه‌ترین فید 2026-08-06
- `@jherr`: تازه‌ترین فید 2026-07-30
- `@WebDevSimplified`: تازه‌ترین فید 2026-09-15
- `@CodeAesthetic`: تازه‌ترین فید 2023-12-23
- `@realmckaywrigley`: تازه‌ترین فید 2025-07-09

داخل پنجره و کوتاه‌فهرست نشد، چون اجرای ۱۲، ۲۱، یا پیش‌نویس ۰۰ خلاصه شده، یا شرحش برای حرف تازه کافی نبود: Fireship (`No-JPdFvYWU`، `I_KVMFrUtPk` و سه ویدیوی قبلی)، Theo (`D8PikZ1KhUo` و خبر مدل)، Matthew Berman (`OODvXcQJyVo` اسپانسر Muse و روایت مدل)، Chrome (`BFdsi7mimUI`، `vukchAoaTdE`، `kbjHnZOQgkQ`، `btIOhb6AiOc`)، Modern Software Engineering (`LO60O07e2KU` و بقیه)، ByteByteGo فقط `E5Ef_Kne17U` (تبلیغ دوره)، Matt Pocock فقط لایو `MN9dGgmLyso` با شرح یک‌خطی، Traversy `0isk_iLFCdk`.

## جست‌وجوی موضوع

تقریباً هیچ Module Federation یا RAG تازه‌ای داخل چهارده روز، با بازدید قابل‌اتکا، در صفحهٔ مرتب‌شده بر اساس آپلود نبود. `litIF9DM6t0` (میکروفرانت، dotJS، ۲۸ سپتامبر، ۱۹۶ بازدید در صفحهٔ watch) در پیش‌نویس ۰۰ خلاصه شده و این‌جا تکرار نشد.

| ویدیو | موضوع | چرا نه |
|---|---|---|
| `b8duTFBvH0o` | CSS anchor، ۲۸ سپتامبر، ۲۹۳۴ بازدید، ۲۳۲ ثانیه | شرح، فهرست ویژگی است: `anchor-name`، `position-anchor`، `position-try`. پلتفرم در اجرای ۲۱ آمده. گفتار جدا گرفته نشد |
| `3u72wGo7nbU` | CSS | Invidious تاریخ انتشار را 2026-09-15 گذاشت، بیرون پنجرهٔ ۱۴ روز |
| `knOhSmOkqMM` | ایجنت | آموزش Agent Builder کوپایلت، ۲۸ سپتامبر، ۴۱۶۰۶ بازدید. شرحش قدم‌های محصول و لایسنس M365 است |
| `qwnJJMNGwgY` | گردش‌کار ایجنت | نگه داشته شد |
| `ILn2GX8s1FM` | tool calling | حدود یک هفته، سخنرانی بلند Spring AI. متن این اجرا گرفته نشد؛ چهار گفتار کوتاه‌فهرست جا را پر کرده بود |
| `SbpcbShc8uE` | میکروفرانت انگولار | حدود دو هفته، آموزش چندساعته، نه کیس |
| `uN2UKIeIiPM` | میکروفرانت | عنوان امنیت enterprise، بازدید پایین |

بقیهٔ نتایج `ytsearch` تاریخ قابل‌اتکا نداشتند و اگر کهنه یا بی‌ربط بودند وارد خلاصه نشدند تا URL و متریک ساختگی ساخته نشود.
