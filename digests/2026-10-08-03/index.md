# نمایهٔ اجرا 2026-10-08-03

- تاریخ تهران: 2026-10-08، حدود ساعت ۰۳:۳۰. تریگر کرون `2026-10-08T00:00:55Z` در تهران ۰۳:۳۰ است و `RUN_ID` از همان ساعت است
- برای `2026-10-08` کلیدی در `schedule` نیست. موضوعات از `default` آمد (۱۲ مورد): میکروفرانت ۲۰۲۶، فدراسیون ماژول، معماری میکروفرانت ری‌اکت، Single-SPA، خبر توسعهٔ وب ۲۰۲۶، روند فرانت ۲۰۲۶، قابلیت تازهٔ CSS و HTML و جاوااسکریپت، به‌روزرسانی Next.js و React، نکتهٔ ایجنت، گردش کار Cursor، ترفند RAG و ابزار، رویهٔ ایجنت کدنویسی
- حالت کانال‌ها: `mode: both`، `per_channel_limit: 5`، `max_age_days: 14`
- فید RSS `feeds/videos.xml` برای هر ۱۴ کانال ۲۰۰ داد
- زاویه‌های اجرای `2026-10-08-00` دوباره پست نشد: کد بدون تست، تابلوی توکن، انسان-روتر، و ۵۷۳٫۸۶ دلار در برابر Astra/Soul
- Whisper نصب نیست. `yt-dlp` روی PATH نبود. گفتار چهار ویدیوی کوتاه‌فهرست از WebFetch صفحهٔ watch آمد. `/api/v1/videos/ID` برای همین شناسه‌ها ۵۰۰ داد. طول از `lengthSeconds` جست‌وجوی Invidious است

## اینستاگرام

فقط هندل‌های `config/instagram-accounts.yaml`. اکسپلور اسکرپ نشد. `prefer_reels` روشن بود.

صفحهٔ اصلی `www.instagram.com` کد ۲۰۰ داد و دو کوکی گذاشت. حدود ۸ ثانیه بعد، `web_profile_info` برای `khashayartalks` روی `i.instagram.com` با `X-IG-App-ID: 936619743392459` کد ۴۲۹ داد و بدنه خالی بود. دوازده حساب دیگر زده نشد. بعد از ۴۲۹ پخش بقیه سقف را بدتر می‌کند.

هیچ کپشن، لایک، یا کوتاه‌کدی این اجرا از اینستاگرام خوانده نشد. چیزی ساخته نشد.

## نگه داشته‌شده

| فایل | منبع | زمان | چرا |
|---|---|---|---|
| [VOMtCIcWq-s.md](VOMtCIcWq-s.md) | The Augmented Expert | watch `Oct 3, 2026` | وبلاگ ۲۰۲۴ vLLM شتاب QPS پایین و کندی QPS بالا را جدا نوشته. PR 49620 هنوز باز است. پست شد |
| [ctoaIC4LHmI.md](ctoaIC4LHmI.md) | ZazenCodes | premiere حدود ۸ ساعت قبل از خواندن watch | گیت مرج، backlog را معاف کرده و اسکریپت prerender را بالا برده پیش انسان. پست شد |
| [f3o0-9Dlw3E.md](f3o0-9Dlw3E.md) | AI Engineer | RSS `2026-10-07T21:30:34Z` | قاضی باید اکسپلویت را نشان بدهد. درصدهای گفتار پست نشد |
| [BsNHg6cNjZE.md](BsNHg6cNjZE.md) | Matthew Berman | RSS `2026-10-07T23:08:41Z` | پاک‌سازی دیسک چیزی پاک نکرد و پیش‌نویس Beehive منتظر کلیک ماند. پست نشد |

## پست‌ها

1. ۱٫۵ و ۲٫۸ برابر در یک پرس‌وجو بر ثانیه، و ۱٫۴ و ۱٫۸ برابر کندتر وقتی QPS بالا است
2. PR باز ۴۹۶۲۰: خروجی speculative بعد از preemption کهنه است
3. مرج کارخانه فقط روی درخت تمیز، به‌جز `factory/backlog.md`؛ یک خط prerender باز هم escalate شد
4. اسکنر پرچم می‌زند. قاضی باید نشان بدهد کاربر A واقعاً به دادهٔ کاربر B می‌رسد

## داخل پنجره، خلاصه نشد

- `o4-29oLHU8E` (Theo، I finally did it.، RSS `2026-10-07T21:03:15Z`، RSS ۶۰۳۱ بازدید و ۱۷۶ ستاره). صفحهٔ watch نوشت `Started streaming` و شرح فقط `Sup nerds we got things to discuss.` بود. WebFetch همان یک خط را داد
- `jlEMo6Dsh9E` (AI LABS، watch `Oct 7, 2026`، ۵۴۳۴ بازدید و ۱۲۴ لایک). دور هشت ابزار Jev است، با اسپانسر. امتیازهای دمو با مخزن چک نشد
- `KcuS-_f4X24` (AI Coding Daily، watch `Oct 5, 2026`، ۱۷۳۳۶ بازدید و ۳۳۵ لایک). شرح قابل‌استفاده نداشت و گفتار گرفته نشد
- جست‌وجوی موضوع روی Invidious `invidious.f5.si` با `sort_by=upload_date` و برای چند پرسش `date=week` یا `date=today`. بیشتر نتیجه‌ها یا قدیمی بودند یا در اجراهای ۷ اکتبر پست شده بودند: `kQ4BRmFr9eI`، `NLioZJBb52U`، `OcvTMCkVvTo`، `HFAkIgRzPMY`، `uccBE9Tun6M`، `RknGPBeA6AQ`، `h9SsHkRSHxo`، `3bLrrkA1nlQ`
- `WrCjAAl9okA` هنوز تازه‌ترین Fireship است و در اجرای ۰۰ بدون گفتار ماند. این اجرا دوباره گرفته نشد

## کانال‌ها

تازه‌ترین RSS این اجرا. پنج‌تای اول هر کانال دیده شد. بازدید و ستاره مال همان فید است.

- `@matthew_berman` تازه‌ترین `BsNHg6cNjZE`، `2026-10-07T23:08:41Z`، ۱۰۰۴ بازدید و ۵۱ ستاره
- `@aiDotEngineer` تازه‌ترین `f3o0-9Dlw3E`، `2026-10-07T21:30:34Z`، ۳۴۷ بازدید و ۷ ستاره
- `@t3dotgg` تازه‌ترین `o4-29oLHU8E`، `2026-10-07T21:03:15Z`، ۶۰۳۱ بازدید و ۱۷۶ ستاره
- `@Fireship` تازه‌ترین `WrCjAAl9okA`، `2026-10-07T20:24:27Z`
- `@ModernSoftwareEngineeringYT` تازه‌ترین `jScItKhruN0`، `2026-10-07T18:00:16Z`
- `@ChromeDevs` تازه‌ترین `_9wjJ1ddHs8`، `2026-10-06T22:36:46Z`
- `@traversymedia` تازه‌ترین `B7GM6F3BP6A`، `2026-10-05T16:12:09Z`
- `@mattpocockuk` تازه‌ترین `BsJGo1wFTvQ`، `2026-10-05T10:50:24Z`
- `@ByteByteGo` تازه‌ترین داخل پنجره `E5Ef_Kne17U`، `2026-09-25`
- `@WebDevSimplified` تازه‌ترین `jojMVmRZABw`، `2026-09-15`، بیرون پنجرهٔ ۱۴ روز
- بیرون پنجره: `@ThePrimeagen` تازه‌ترین `2026-08-06`، `@jherr` `2026-07-30`، `@realmckaywrigley` `2025-07-09`، `@CodeAesthetic` `2023-12-23`
