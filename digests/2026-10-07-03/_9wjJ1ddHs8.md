# گذار نما، بازنشر آبان ۱۴۰۴

- platform: youtube
- url: https://www.youtube.com/watch?v=_9wjJ1ddHs8
- channel: Chrome for Developers
- title: 95: Updates to View Transitions
- creator: Una Kravets و Bramus Van Damme، CSS Podcast
- published: RSS کانال `2026-10-06T22:36:46+00:00`، برابر `2026-10-07T02:06:46+03:30`. شرح همین فید می‌گوید Originally aired: November 5, 2025
- views: RSS همین اجرا ۹۲. کمی قبل‌تر در جست‌وجوی Invidious ۸۸
- likes: RSS همین اجرا `starRating` با `count` برابر ۱۰ و `average` برابر ۵٫۰۰
- duration_seconds: ۱۰۶۶ از نتیجهٔ جست‌وجوی `invidious.f5.si` که همین شناسه را برگرداند
- metrics_source: فید `feeds/videos.xml` کانال `UCnUYZLuoy1rq1aVMwx4aTzw` برای زمان و بازدید و ستاره. طول از جست‌وجو
- topic: `match-element`، گروه تودرتو در Chrome 140، و گذار محدود به زیردرخت. ادعاهای پشتیبانی مال زمان ضبط‌اند
- text_source: گفتار WebFetch صفحهٔ watch با `hl=en` و شرح RSS. Whisper نصب نیست. کیس‌استادی AI Mode در developer.chrome.com این اجرا باز نشد

## خلاصه

اپیزود ۸۹ را پایه فرض کردند و این قسمت را تغییرات بعد از آن. در زمان ضبط گفتند same-document و cross-document در Chrome و Safari هست. فایرفاکس را روی same-document در نایتلی گفتند، با انتظار رسیدن به پایدار در همان سال برای Interop 2025. گفتند پیاده‌سازی فایرفاکس `view-transition-class` را دارد و types را ندارد.

types را برای مسیرهای مختلف گذاشتند. مثالشان صفحه‌بندی وبلاگ در برابر رفتن به صفحهٔ درباره بود. برای same-document، `document.startViewTransition` می‌تواند شیء بگیرد با `callback` و `types`. برای cross-document، توصیفگر `types` روی قاعدهٔ `@view-transition`. انتخابگر را `:active-view-transition-type()` گفتند، از قبلِ گرفتن اسنپ قدیم تا پایان گذار. AI Mode جست‌وجوی گوگل را مثال استفاده خواندند. آن کیس‌استادی این اجرا باز نشد و عددی از آن نیامد.

`match-element` را مقدار خاص `view-transition-name` خواندند تا مرورگر از روی هویت عنصر اسم یکتا بسازد و لازم نباشد برای صد کارت صد اسم دست‌ساز باشد. گفتند این هویت شمارهٔ داخلی ساخت عنصر است، پس برای cross-document به کار نمی‌آید. اگر فریم‌ورک گره را بسازد و دوباره بسازد، عنصر جدید شمارهٔ دیگر دارد و تطبیق می‌شکند. راهشان `attr()` روی شناسه یا data-attribute، با نوع، و برگشت به `match-none` بود.

گروه تودرتو را مال Chrome 140 خواندند. بدون آن، شبه‌عنصر کارت و آواتارها خواهر می‌شوند و برش، ماسک، فیلتر و تبدیل سه‌بعدی درست نمی‌نشیند. ویژگی `view-transition-group` را `contain` روی والد، یا `nearest` یا یک اسم سفارشی روی فرزند گفتند. فرزندها مستقیم زیر گروه والد نیستند. داخل شبه‌عنصر `view-transition-group-content` جمع می‌شوند و برای برش باید روی همان `overflow: clip` گذاشت.

گذار محدود به زیردرخت را در زمان ضبط فقط Canary با پرچم experimental web platform features گفتند و بازخورد خواستند. به‌جای `document.startViewTransition` روی خود عنصر صدا زده می‌شود. بقیهٔ صفحه تعاملی می‌ماند. دو گذار هم‌زمان را فقط اگر زیردرخت‌ها جدا باشند ممکن خواندند. مسئلهٔ z-index را هم با این کم کردند: شبه‌عنصر گذار بالای سند و حتی top layer نقاشی می‌شد و popover را می‌پوشاند. قبلاً مجبور بودند به popover هم اسم گذار بدهند. ظرفِ scoped خودش با گذار جابه‌جا نمی‌شود، بر خلاف گروه تودرتو. جمع‌بندی خودشان: اول scoped، و اگر کم بود گروه تودرتو.

`document.activeViewTransition` را در زمان ضبط در هیچ مرورگری نگفتند.

## نکته‌های کلیدی

- تاریخ پخش اصلی در شرح: ۵ نوامبر ۲۰۲۵. آپلود RSS این کانال ۶ اکتبر ۲۰۲۶ است
- `match-element` به هویت گره بسته است و بازسازی DOM فریم‌ورک آن را می‌شکند
- Chrome 140 برای گروه تودرتو، در زمان ضبط
- scoped در آن زمان Canary و آزمایشی بود
- پشتیبانی مرورگر این اجرا دوباره چک نشد

## چه وارد پست نشد

- وضعیت ۲۰۲۶ مرورگرها، چون گفتار مال زمان ضبط است
- کیس‌استادی AI Mode، چون صفحهٔ منبع این اجرا باز نشد
