# Why AI Didn't Actually Make You Ship Faster — Gabriel Spencer-Harper, Meticulous

- platform: youtube
- url: https://www.youtube.com/watch?v=HLTa7Vcs4X0
- channel: AI Engineer
- speaker: Gabriel Spencer-Harper, هم‌بنیان‌گذار و CEO در Meticulous
- published: Oct 2, 2026 (dateText صفحهٔ watch در همین اجرا)
- views: 2,166
- views_source: صفحهٔ watch در همین اجرا
- likes: 4
- likes_source: factoid لایک همان صفحه
- duration: 11:15
- duration_source: نشان مدت روی تب ویدیوهای کانال (`animationActivationTargetId`)
- topic: تأیید فرانت وقتی ایجنت سریع‌تر از ریویو کد می‌نویسد
- text_source: شرح منتشرشده و فهرست فصل‌ها. گفتار کامل گرفته نشد

## خلاصه

گابریل اسپنسر-هارپر می‌گوید AI سریع‌تر از انسان کد می‌نویسد و گلوگاه شده تأیید. تست مبتنی بر assertion را برای کد تولیدشده کافی نمی‌داند، چون فضای رگرسیون ممکن از assertion دست‌نویس بزرگ‌تر است. چیزی که نشان می‌دهد تأیید نزدیک به exhaustive فرانت است، با تلاش نزدیک به صفر برای توسعه‌دهنده: ضبط جریان واقعی کاربر، پخش دوباره روی هر PR، و diff تصویری قبل/بعد.

سه تکنولوژی را نام می‌برد: ترافیک شبکهٔ کاملاً mockشده، مرورگر deterministic برای حذف تست ناپایدار، و انتخاب جریان با راهنمای coverage. می‌گوید coverage وقتی معنی «کد تست‌شده» می‌دهد که از هر قدم اسکرین‌شات داشته باشی.

فصل‌ها یک سؤال دمو دارند: روی این PR دکمهٔ merge را می‌زنی؟ هزینه را باگ، تست ناپایدار، و زمان از دست‌رفته می‌گذارد. محصول Meticulous است و بخش دمو معرفی همان محصول است.

## نکته‌ها

- گلوگاه را از نوشتن به تأیید برده، با مکانیزم record-and-replay تصویری.
- assertion دست‌نویس را به‌خاطر بزرگی فضای رگرسیون کنار می‌گذارد، نه به‌خاطر اینکه تست بی‌فایده است.
- عدد پوشش یا تعداد جریان در شرح نیست.
