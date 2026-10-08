# تأیید محلی هست و چک نسخه خاموش نمی‌شود

- platform: youtube
- url: https://www.youtube.com/watch?v=My0KTjLEX4M
- channel: Alex Hitt
- title: Plannotator GitHub Overview: Review AI Plans and Diffs Locally
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 7, 2026` نشان داد. Invidious `published` را `1791331200` داد. جست‌وجو `publishedText` را `8 hours ago` داد
- views: صفحهٔ watch همین اجرا `32 views`. Invidious هم ۳۲
- likes: عبارت صفحهٔ watch `along with 2 other people`. Invidious هم ۲
- duration_seconds: ۵۱۰ از `/api/v1/videos/My0KTjLEX4M?hl=en`
- metrics_source: HTML صفحهٔ watch و اندپوینت Invidious
- topic: قلاب ExitPlanMode برنامه را در مرورگر محلی نگه می‌دارد و چک نسخهٔ گیت‌هاب opt-out ندارد
- text_source: گفتار WebFetch صفحهٔ watch و README خام `backnotprop/plannotator` روی main. Whisper نصب نیست

## خلاصه

گفتار ابزار را یک سرور محلی زودگذر می‌خواند که نخ ایجنت را قبل از نوشتن کد نگه می‌دارد، پورت تصادفی می‌گیرد، با xdg-open مرورگر را باز می‌کند، و سه دکمه دارد: approve و annotate و dismiss. می‌گوید چک نسخهٔ گیت‌هاب موقع لود اجباری است و خاموش نمی‌شود، ولی `git ls-remote` را می‌شود خاموش کرد. تلهٔ هدلس را هم می‌گوید: اگر xdg-open پروسهٔ شبح بسازد، جلسه منتظر مرورگری می‌ماند که نمی‌آید مگر تایم‌اوت دستی. این جزئیات پورت و iframe و هدلس در بخش خوانده‌شدهٔ README نبود.

README جریان را این‌طور می‌نویسد: ایجنت ExitPlanMode را صدا می‌زند، قلاب PermissionRequest آتش می‌گیرد، سرور محلی برنامه را از ورودی قلاب می‌خواند، مرورگر باز می‌شود، انسان حاشیه می‌نویسد و approve یا deny می‌کند. approve یعنی ایجنت ادامه دهد. deny بازخورد ساخت‌یافته می‌فرستد و ایجنت اصلاح می‌کند. بازبینی کد با `/plannotator-review` از git diff یا URL یک PR است و approve فقط رشتهٔ `LGTM` را می‌فرستد.

حریم خصوصی README: تله‌متری مصرف جمع نمی‌کند. برنامه و diff و حاشیه به‌طور پیش‌فرض محلی می‌مانند. هر سطح plan review و annotate و archive و share-portal و code-review موقع لود آخرین نسخه را از گیت‌هاب می‌پرسد. محتوا نمی‌فرستد و تنظیم opt-out ندارد. `git ls-remote` را می‌شود با `plannotator review --no-git-remote-check` یا `PLANNOTATOR_GIT_REMOTE_CHECK=0` یا `gitRemoteCheck: false` خاموش کرد. محتوا وقتی بیرون می‌رود که خودت اشتراک، بازبینی گیت‌هاب یا گیت‌لب، Ask AI، یا Workspaces را روشن کرده باشی. لینک رمزشده متن رمز را به سرویس paste می‌فرستد. Workspaces محصول میزبانی جداست.

API گیت‌هاب همین اجرا: ۹۲۱۰ ستاره، Apache-2.0، push در `2026-10-08T09:11:18Z`.

## نکته‌های کلیدی

- README: قلاب، سرور محلی، approve یا deny، بعد ادامه یا بازخورد
- چک نسخهٔ گیت‌هاب opt-out ندارد و محتوا نمی‌فرستد
- چک ریموت گیت opt-out دارد
- پورت تصادفی و گیر کردن هدلس را README این خواندن نگفت
- اشتراک و Workspaces پیش‌فرض «همه‌چیز محلی» را سوراخ می‌کنند اگر روشن شوند

## چه وارد پست نشد

- این ویدیو پست نشد. زاویه‌های اندازه‌گیری و شرح ابزار در همین اجرا مشخص‌تر بودند
- ادعای iframe و تایم‌اوت هدلس، چون در README خوانده‌شده نبود
