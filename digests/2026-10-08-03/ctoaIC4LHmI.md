# کارخانه مرج نمی‌کند اگر درخت اصلی کثیف باشد

- platform: youtube
- url: https://www.youtube.com/watch?v=ctoaIC4LHmI
- channel: ZazenCodes
- title: Build Your Own AI Software Factory with Claude Code
- published: صفحهٔ watch همین اجرا `Premiered 8 hours ago`. مخزن نمونه `2026-10-07T15:27:09Z` پوش شده بود
- views: صفحهٔ watch همین اجرا `2,011 views`
- likes: عبارت لایک `129`
- duration_seconds: ۱۶۸۲ از `lengthSeconds` نتیجهٔ جست‌وجوی Invidious. اندپوینت ویدیو این اجرا ۵۰۰ داد
- metrics_source: HTML صفحهٔ watch. ستاره و زمان پوش از API گیت‌هاب `zazencodes/zazencodes-season-3`
- topic: حلقهٔ spec و build و review و approve در Claude Code، و گیت مرج که درخت اصلی را تمیز می‌خواهد
- text_source: گفتار WebFetch، شرح (اسپانسر Anthropic)، و فایل‌های https://github.com/zazencodes/zazencodes-season-3/tree/main/src/software-factory-claude-code

## خلاصه

ویدیو اسپانسر Anthropic است. او یک کارخانهٔ کوچک را داخل سایت خودش می‌سازد: مهارت `factory` ارکستر است و خودش کد و spec و بازبینی و تصمیم را نمی‌نویسد. هر عامل فقط فایل خودش را می‌نویسد. حلقه در `SKILL.md` این است: spec-writer، بعد builder روی شاخهٔ `factory/<job-id>`، بعد چهار بازبین security و ux و ui و code، و اگر کسی `CHANGES` بدهد builder از سر گرفته می‌شود. `MAX_RESUMES = 2` یعنی بعد از دور اول، builder حداکثر دو بار از سر گرفته می‌شود و یک اجرا حداکثر سه دور بازبینی دارد. حرف ویدیو «حداکثر دو دور» بود. فایل دقیق‌تر است.

هر کار در worktree جدا است، کنار مخزن، به مسیر `../<name>-factory/<job-id>/`. جلسهٔ ارکستر در checkout اصلی می‌ماند. فقط گام Merge به checkout اصلی دست می‌زند.

در دمو، اولین اجرا شروع نشد چون درخت کاری تمیز نبود و او خودش commit کرد. بعدتر مرج 404 هم ایستاد. گفتار می‌گوید مرج فقط وقتی checkout اصلی تمیز و روی `main` باشد انجام می‌شود، و تغییر backlog مانع شده بود. فایل منتشرشده این استثنا را نوشته است. دستور این است:

`git status --porcelain -- . ':!factory/backlog.md'`

باید خالی باشد و `git branch --show-current` باید `main` چاپ کند. `factory/backlog.md` معاف است، چون هر `/factory next` همان فایل را عوض می‌کند و شاخهٔ کار به آن دست نمی‌زند. اگر شرط برقرار نباشد، stage می‌شود `needs-human`.

`decision.md` کار `001-blog-reading-time` با `ESCALATE` شروع می‌شود. هر چهار بازبین دور اول `PASS` بودند و `git merge-tree` تمیز بود. علت توقف: شاخه `scripts/prerender-blog.js` را عوض کرده و آن را تغییر deploy حساب کرده. تغییر یک خط است و `readingTime.js` را به `RENDERER_DEPENDENCIES` اضافه می‌کند. اثر را این‌طور نوشته: با اولین `./deploy.sh` بعد از مرج، کش prerender وبلاگ عوض می‌شود و هر پست یک بار دوباره رندر می‌شود. تصمیم با انسان است.

`decision.md` کار `002-not-found-page` با `APPROVE` شروع می‌شود و بخش انسان را `N/A` گذاشته. توقفی که در ویدیو برای 404 دیده شد، از کثیف بودن checkout بود، نه از رد شدن بازبینی در همین فایل.

`approver.md` فقط وقتی `APPROVE` می‌دهد که معیارهای پذیرش با شاهد در `build.md` برقرار باشد، هر چهار بازبین دور آخر `PASS` باشند، و `git merge-tree --write-tree main <branch>` تعارض ندهد. جدا از این، اگر تغییر به پول، دسترسی، هویت، deploy یا CI، مهاجرت اسکیما، ایمیل، دادهٔ تولید، یا وابستگی تازه دست بزند، `ESCALATE` است.

README می‌گوید موقع کپی کردن، `/factory/jobs/` را به gitignore اضافه کنید. `SKILL.md` هم پوشهٔ jobs را حالت زمان اجرا و gitignore شده می‌خواند. `.gitignore` ریشهٔ `zazencodes-season-3` پوشهٔ `.claude` را نادیده می‌گیرد و بعد `.claude` همین کارخانه را با `!` برمی‌گرداند. همان فایل `factory/jobs/` را نادیده نمی‌گیرد و دو کار نمونه commit شده‌اند. API این اجرا: ۳۷ ستاره، پوش `2026-10-07T15:27:09Z`. این ستاره مال کل مخزن فصل ۳ است، نه یک مخزن جدا برای کارخانه.

او در دمو bypass permissions را روشن کرد. هزینه را گفت روی پلن Claude بوده و عدد توکن نداد. وارد پست نشد.

## نکته‌های کلیدی

- مرج فقط روی `main` و وقتی porcelain بقیهٔ درخت خالی است. backlog از همین چک معاف است
- `001` با چهار PASS باز هم به‌خاطر یک خط در اسکریپت prerender بالا رفت پیش انسان
- `MAX_RESUMES = 2`، حداکثر سه دور بازبینی
- jobs در متن مهارت gitignore است و در gitignore همین مخزن نیست

## چه وارد پست نشد

- نام ۱۹۶۸ در گفتار واضح نبود
- هزینه و کیفیت. عددی در گفتار یا README نیست
- «حداکثر دو دور» به‌جای متن فایل
