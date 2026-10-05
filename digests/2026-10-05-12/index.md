# نمایهٔ اجرا 2026-10-05-12

- تاریخ تهران: 2026-10-05، حدود ساعت ۱۲:۴۶. تریگر کرون `2026-10-05T09:04:40Z` در تهران ۱۲:۳۴ است و `RUN_ID` از همان ساعت است
- برای `2026-10-05` کلیدی در `schedule` نیست. موضوعات از `default` آمد: میکروفرانت ۲۰۲۶، فدراسیون ماژول، معماری میکروفرانت ری‌اکت، Single-SPA، خبر وب ۲۰۲۶، روند فرانت ۲۰۲۶، CSS و HTML و جاوااسکریپت، Next.js و React، نکتهٔ ایجنت، گردش کار Cursor، ترفند RAG، رویهٔ ایجنت کدنویسی
- حالت کانال‌ها: `mode: both`، `per_channel_limit: 5`، `max_age_days: 14` (جدیدتر از حدود `2026-09-21T09:06:21Z`)
- فهرست کانال و جست‌وجو از `invidious.f5.si`. بدنهٔ زیرنویس همان منبع خالی بود. اندپوینت `/api/v1/videos/:id` برای کوتاه‌فهرست ۵۰۰ داد، پس لایک جدا نیامد. بازدیدها مال فهرست کانال یا نتیجهٔ جست‌وجو است و بعضی‌ها گرد شده‌اند
- `published` این منبع برای چند ویدیوی «2 weeks ago» یک سطل نزدیک مرز ۱۴ روز است. داخل نگه داشته شدند چون هم متن «2 weeks ago» بود هم عدد سطل از cutoff رد می‌شد. ساعت دقیق‌تر در دست نبود
- Whisper نصب نیست. `youtube-transcript-api` از این IP بلاک شد. گفتار کوتاه‌فهرست از WebFetch صفحهٔ watch آمد
- زاویه‌های اجرای ۰۹ همین تاریخ (اول عدد، نوار استخدام، تست بدون مدل، پوشهٔ اسکیل) تکرار نشد

## اینستاگرام

فقط هندل‌های `config/instagram-accounts.yaml`. اکسپلور اسکرپ نشد. `prefer_reels` روشن بود.

`web_profile_info` روی `www.instagram.com` اول برای `captainhoff` کد ۲۰۰ داد. تلاش بعدی برای بقیهٔ حساب‌ها ۴۲۹ شد. بعد از جمع کردن یوتیوب، هم `www` و هم `i.instagram.com` برای `qendresahhoti` کد ۴۰۰ دادند (پیام حذف شدن یک asset داخلی). آینهٔ imginn برای سه حساب ۴۰۳ و صفحهٔ چالش بود. WebFetch خود پروفایل `youraveragetechbro` دیوار لاگین بود. گفتار ریل گرفته نشد.

| حساب | نتیجه |
|---|---|
| captainhoff | ۲۰۰، قبل از سقف. دوازده آیتم تایم‌لاین. پنج ریل تازه پایین |
| daniallqureshi | ۴۲۹ |
| youraveragetechbro | ۴۲۹، و WebFetch پروفایل دیوار لاگین |
| skip_ci | ۴۲۹ |
| sicknider_raw | ۴۲۹ |
| mattmurphy | ۴۲۹ |
| umacodes | ۴۲۹ |
| qendresahhoti | ۴۲۹، بعد ۴۰۰ |
| haydenschmitty | ۴۲۹ |
| rollins_io | ۴۲۹ |
| chase_h_ai | ۴۲۹ |
| khashayartalks | ۴۲۹ |
| jam_with_ai | ۴۲۹ |

پنج ریل تازهٔ `captainhoff`، مرتب بر `taken_at_timestamp`. هر پنج تا `product_type=clips`. کپشن‌ها سؤال کوتاه‌اند، نه ادعای قابل‌چک. خلاصهٔ جدا نوشته نشد تا از روی سؤال، حرف ویدیو ساخته نشود.

| شورت‌کد | زمان تهران | لایک | بازدید | کپشن |
|---|---|---|---|---|
| DeArKRXAC2r | 2026-10-03T03:04:37+03:30 | ۲۰ | ۲۷۹ | Become the Director of AI. کار را خودت نکن، کارگردان ایجنت‌ها شو |
| Dd-OoneAaKl | 2026-10-02T04:17:18+03:30 | ۱۲۰ | ۱۹۸۱ | How to Become AI Native |
| Dd7p2k6DYSM | 2026-10-01T04:17:22+03:30 | ۱۷ | ۴۱۱ | The Key to AI Leadership |
| Dd5E_TViTYW | 2026-09-30T04:16:17+03:30 | ۸۰ | ۱۳۸۲ | Build an AI-Native Business |
| Dd2d3BEjhF7 | 2026-09-29T03:56:20+03:30 | ۲۰۲ | ۳۵۰۲ | Which AI Model is the Best? هزینه و سرعت و هوش |

سه ریل پین قدیمی‌تر هم در همان پاسخ بود (`Dc4lMf-Fcwb` پنجم سپتامبر، `DbJ-66TAFu1` و `Dal9sb8jxwe` در تیر) و جزو پنج تای تازه حساب نشدند.

## نگه داشته‌شده

| فایل | منبع | چرا |
|---|---|---|
| [B6B9LOLpoKY.md](B6B9LOLpoKY.md) | Modern Software Engineering | دویست نفر و کامپایل نشدن. پست شد |
| [jojMVmRZABw.md](jojMVmRZABw.md) | Web Dev Simplified | ۸۶۰۰ توکن و اسم اسکیل در هر پرامپت. پست شد |
| [aAFn0rRqeJ8.md](aAFn0rRqeJ8.md) | Traversy Media | یک هوک، ده میزبان. پست شد |
| [df2H7reofa8.md](df2H7reofa8.md) | CodeHead، از جست‌وجوی موضوع | لیسنر به‌جای API مرورگر. پست شد |

## پست‌ها

1. نفر اضافه، یادگیری را کند می‌کند
2. مالیات AGENTS.md
3. هوک سفر کرد، رندرر نه
4. راه‌حلی که مرورگر داشت

## گفتار گرفته شد، خلاصه نشد

- `T-E7rmD6rh4` (Matthew Berman، اقیانوس کد با Sonnet 5.5، ۱۱۱۰۰۰ بازدید، ۱۰۲۰ ثانیه): دموی بازی و لگو و شهر. قیمتی که می‌گوید نصف Opus است و چند بنچمارک نزدیک هم‌اند. زاویهٔ مدل تازه، کنار پست‌های همین هفته تکراری بود
- `jGD_UR4wMJc` (Matthew Berman، هشت کاربرد Jev، ۲۲۹۰۰۰ بازدید، ۶۳۸ ثانیه): تصمیم‌گیر، نه مولد. Jev در اجرای ۲۱ مهر پست شده بود
- `nwauFPVDVEY` (Chrome for Developers، عنوان «93: State queries in 2025»، ۴۴۹ بازدید، ۱۰۷۳ ثانیه): کوئری scroll-state در Chrome 133 و anchored در Canary. عنوان خودش را ۲۰۲۵ می‌داند و بازدید پایین است

## داخل پنجره، باز نشد

میکروفرانت و فدراسیون و Single-SPA نتیجهٔ تازهٔ پربازدید نداد. `litIF9DM6t0` و `GT_hkkcLKHc` قبلاً خلاصه شده‌اند. `YXOO6vZW2f8` هشت بازدید. `HFAkIgRzPMY` ده بازدید. `Bee4ysrtyOs` ۱۳۳۱ بازدید بود و گفتارش این اجرا گرفته نشد.

خبر وب این هفته بیشتر DevDay بود. `Fls_onRviPM` و `GjN3xLDuc8o` و `uXspbC2srEQ` باز نشدند. `vu8X3YroB-w` و `8WbW_n95wc4` و `IBcBKgYUghU` از تئو هم باز نشدند تا اجرا در خبر OpenAI غرق نشود. `FsDUOUV9Vs8` صبح همین روز پست شده بود.

`7r4ikZHm9AI` و `LoLYw--s-5w` از Fireship داخل پنجره‌اند و بازدید میلیونی دارند. این اجرا باز نشدند. `c1rPlzxSZ8E` و `ylO0DQeVEBQ` را اجرای ۰۹ دیده و به‌خاطر لحن گزارش طنز کنار گذاشته بود.

`E5Ef_Kne17U` از ByteByteGo (۴۹۰۰۰ بازدید) باز نشد. `U8lGbSaCCYI` و `CtTtWuch4Yk` و `-Z11mZaJU0w` هنوز «0 seconds ago» و صفر بازدید بودند.

بیرون پنجره: `@ThePrimeagen` حدود یک ماه، `@jherr` حدود دو ماه، `@mattpocockuk` حدود یک ماه، `@realmckaywrigley` حدود یک سال، `@CodeAesthetic` چند سال. `jojMVmRZABw` را اجرای ۰۹ با سطل قدیمی‌تر بیرون پنجره دیده بود. سطل این اجرا داخل پنجره بود و نگه داشته شد.
