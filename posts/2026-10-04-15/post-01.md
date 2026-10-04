# فرمان را ننویسی، ایجنت حدس می‌زند

فایل دستور را نوشتی.
ایجنت هنوز هر بار یک جور دیگر فرمان را انتخاب می‌کند.

کارل لیندبرگ پای یک ریپوی Terraform نشسته بود. دو محیط، dev و prod. از Claude خواست یک subnet به نام app اضافه کند و AGENTS.md نداشت. مدل `terraform validate` را بلد بود. تست را این بار زد، چون پوشهٔ تست را دید. بار بعد هیچ تضمینی نیست. خودش می‌گوید ورودی یکی است و خروجی یکی نیست.

فایل را از «مراقب پروداکشن باش» برد به فرمان. init. فرمت. validate. تست. plan هر دو محیط. تمام‌شدن یعنی هر چهار تا سبز باشند و plan فقط همان تغییری را نشان بدهد که خواستی. این بار خلاصهٔ هر دو plan آمد و apply نزد.

پیچش جای فرمان نبود. یک CLAUDE.md با همان متن گذاشت، منهای یک خط امضا. فهرست context فقط CLAUDE.md را نشان داد. AGENTS.md اصلاً وارد زمینه نشده بود. سایت خود قرارداد، agents.md، نزدیک‌ترین فایل به محل ویرایش را مقدم می‌داند و می‌گوید پرامپت صریح چت از فایل جلو می‌زند. در دموی Claude Code، وجود CLAUDE.md همان قرارداد را از زمینه حذف کرد.

تا فرمان را عیناً ننویسی، «درست تست کن» برای ایجنت یک جملهٔ مهربان است.

آخرین باری که ایجنت فرمان غلط زد، فایل دستور را باز کردی یا فقط پرامپت را بلندتر نوشتی؟

#AGENTS_md #ClaudeCode #Terraform #ایجنت #هارنس #مهندسی_نرم‌افزار #Cursor

---
source_videos:
  - title: "If You Don't Understand AGENTS.md, You Don't Understand Coding Agents"
    url: https://www.youtube.com/watch?v=4nVafPsuyb4
  - title: "AGENTS.md"
    url: https://agents.md/
topic: vague agent instructions stay guesses, and CLAUDE.md can hide AGENTS.md
generated_at: 2026-10-04T15:50:00+03:30
