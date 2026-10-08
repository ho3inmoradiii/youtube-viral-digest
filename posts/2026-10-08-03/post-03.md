# دفتر کارخانه، درِ مرج را بست

کارخانه فیچر را ساخت، چهار بازبین را پاس کرد، و بعد ایستاد.
مقصر کد نبود. فایلی بود که خود کارخانه هر بار خطش می‌زند.

در دمو، اولین اجرا اصلاً شروع نشد چون درخت کاری تمیز نبود. او اول commit کرد. کمی بعد مرج صفحهٔ ۴۰۴ هم ایستاد، چون checkout اصلی کثیف بود. مهارت منتشرشده حالا این را صریح نوشته. مرج فقط در checkout اصلی است، فقط وقتی شاخهٔ جاری `main` باشد، و فقط وقتی این دستور هیچ چاپی ندهد:

`git status --porcelain -- . ':!factory/backlog.md'`

`factory/backlog.md` عمداً بیرون است. هر `/factory next` همان فایل را عوض می‌کند و شاخهٔ کار به آن دست نمی‌زند، پس کثیف بودنش با مرج تعارض ندارد. بقیهٔ درخت اگر کثیف باشد، stage می‌شود `needs-human`.

یک توقف دیگر در فایل تصمیم مانده، نه در حرف دمو. کار `001-blog-reading-time` هر چهار بازبین دور اول را `PASS` گرفته و merge بدون تعارض بوده. approver باز هم `ESCALATE` نوشته، فقط چون شاخه یک خط در `scripts/prerender-blog.js` عوض کرده: `readingTime.js` را به `RENDERER_DEPENDENCIES` اضافه کرده. اثر را خودش این‌طور جمع کرده که با اولین deploy بعد از مرج، کش prerender وبلاگ می‌شکند و هر پست یک بار دوباره رندر می‌شود. تصمیم با انسان است.

`MAX_RESUMES = 2` است. یعنی builder بعد از دور اول حداکثر دو بار برمی‌گردد و یک کار حداکثر سه دور بازبینی دارد. حرف ویدیو «دو دور» بود. فایل این است.

README موقع کپی می‌گوید `factory/jobs/` را gitignore کنید. متن مهارت هم همان پوشه را حالت زمان اجرا می‌خواند. gitignore ریشهٔ مخزن فصل ۳ پوشهٔ jobs را نادیده نمی‌گیرد و دو کار نمونه commit شده‌اند. API این اجرا برای کل `zazencodes/zazencodes-season-3` سی و هفت ستاره دید، نه برای یک مخزن جدا.

گیت اتوماتیکی که فایل وضعیت خودش را «کثیف» حساب کند، یا باید همان یک فایل را معاف کند یا هر اجرای سالم را پیش انسان بفرستد. معاف کردن همهٔ درخت، آن گیت را نمایشی می‌کند.

در گیت اتوماتیک شما، فایلی که خود سیستم هر بار می‌نویسد هنوز جلوی مرج را می‌گیرد؟

#claude_code #git #اتوماسیون #بازبینی #کارخانه_نرم‌افزار #مهندسی_نرم‌افزار

---
source_videos:
  - title: "Build Your Own AI Software Factory with Claude Code"
    url: https://www.youtube.com/watch?v=ctoaIC4LHmI
  - title: "factory/SKILL.md"
    url: https://github.com/zazencodes/zazencodes-season-3/blob/main/src/software-factory-claude-code/.claude/skills/factory/SKILL.md
  - title: "001-blog-reading-time/decision.md"
    url: https://github.com/zazencodes/zazencodes-season-3/blob/main/src/software-factory-claude-code/factory/jobs/001-blog-reading-time/decision.md
topic: merge requires a clean main checkout except the backlog file; a prerender one-liner still escalates
generated_at: 2026-10-08T03:40:00+03:30
