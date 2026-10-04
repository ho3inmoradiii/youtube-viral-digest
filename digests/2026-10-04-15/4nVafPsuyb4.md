# AGENTS.md فرمان است، جملهٔ مهربان نیست

- platform: youtube
- url: https://www.youtube.com/watch?v=4nVafPsuyb4
- channel: Carl Lindberg
- title: If You Don't Understand AGENTS.md, You Don't Understand Coding Agents
- published: صفحهٔ watch، `dateText` برابر Oct 4, 2026
- views: 76
- likes: 7
- duration_seconds: 1632
- metrics_source: بازدید و لایک از HTML صفحهٔ watch با کوکی `SOCS=CAI` در همین اجرا. مدت از `lengthSeconds` جست‌وجوی Invidious `invidious.f5.si` در همین اجرا. اندپوینت `/api/v1/videos/4nVafPsuyb4` همان اینستنس ۵۰۰ داد
- topic: دستور مبهم را ایجنت هر بار جور دیگری معنی می‌کند، و CLAUDE.md می‌تواند AGENTS.md را از زمینه حذف کند
- text_source: گفتار صفحهٔ watch از WebFetch در همین اجرا. ادعای «بیش از ۶۰هزار پروژه» و «۸۸ فایل در ریپوی اصلی OpenAI» با متن https://agents.md/ در همین اجرا جور شد
- convention: https://agents.md/

## خلاصه

لیندبرگ مشاور ابر و Microsoft MVP است و Terraform پروداکشن Azure را با ایجنت می‌نویسد. ویدیو AGENTS.md را README برای ایجنت می‌داند، نه قالب تازه. فیلد اجباری ندارد. README برای آدم است: نصب، اسکرین‌شات، لایسنس. AGENTS.md فرمان ساخت و تست، سبک کد، قاعدهٔ PR، و معیار تمام‌شدن را برای ایجنت همان ریپو می‌گذارد. می‌گوید پرامپت صریح چت از فایل جلو می‌زند و اگر تناقض را بگویی، ایجنت فایل را کنار می‌گذارد. پس فایل قانون نیست.

دمو یک ریپوی Terraform است با resource group و virtual network و subnet، روی dev و prod. بدون AGENTS.md از Claude می‌خواهد subnet به نام app اضافه شود. مدل `terraform validate` را می‌زند. تست را این بار زد، چون پوشهٔ تست را دید. می‌گوید سیستم تصادفی است و بار بعد ممکن است تست را نزند.

آناتومی پیشنهادی‌اش: نمای پروژه، فرمان دقیق setup، سبک، تست، راز و مسیر ممنوع، قاعدهٔ کامیت و PR، و مسیر dev به prod. نمونهٔ ضعیف فقط می‌گوید «کد معتبر و تست‌شده باشد و با پروداکشن مراقب باش». نمونهٔ بهتر فرمان را می‌نویسد: init، فرمت، validate، تست، سبک AzAPI، و «اعمال نکن». معیار تمام‌شدن این است که format و validate و test سبز باشند. در دمو با فایل بهتر، تست نام‌گذاری subnet را lowercase می‌خواهد و app می‌شود net-app. برای dev و prod هر دو plan می‌زند و خلاصه را گزارش می‌کند: یک افزودن، صفر تغییر، صفر حذف. apply نمی‌زند. یک خط امضا («درخت کریسمس، چک‌شده با AGENTS.md») فقط نشانگر این است که فایل خوانده شده.

قرارداد تو در تو را هم نشان می‌دهد. نزدیک‌ترین AGENTS.md به محل کار مقدم است. در پوشهٔ تست یک فایل دوم می‌گذارد که قاعدهٔ ریشه را نگه می‌دارد و فرمان plan را برای تست مشخص می‌کند. می‌گوید سایت قرارداد مثال زده که ریپوی اصلی OpenAI در زمان نوشتن ۸۸ فایل AGENTS.md داشته. این جمله در https://agents.md/ هست، بخش monorepo.

اگر CLAUDE.md با همان محتوا باشد و فقط خط امضا را نداشته باشد، Claude Code در دموی او AGENTS.md را نمی‌خواند. دستور context فقط CLAUDE.md و CLAUDE.md سراسری را فهرست می‌کند. راه‌حل دمو این است که CLAUDE.md به AGENTS.md اشاره کند تا فایل دوم هم وارد زمینه شود. در پایان یک بخش deploy اضافه می‌کند: اعمال فقط روی dev و فقط وقتی خود تسک بخواهد، با plan و apply روی `dev.tfvars`. Copilot CLI همان AGENTS.md را بومی می‌خواند. با Sonnet و allow-all از آن می‌خواهد subnet را اضافه و روی dev مستقر کند. پورتال Azure بعد از refresh subnet سوم را نشان می‌دهد.

## نکته‌ها

- «بیش از ۶۰هزار پروژهٔ متن‌باز» و «۸۸ فایل در ریپوی اصلی OpenAI» را خود https://agents.md/ در همین اجرا نوشته. شمارش جداگانهٔ ریپوی OpenAI انجام نشد.
- درخت کریسمس نشانگر دمو است، نه توصیهٔ سبک.
- خط قرمز apply و نام دقیق فلگ‌ها از گفتار دمو آمده، نه از یک AGENTS.md عمومی که این اجرا جدا خوانده باشد.
