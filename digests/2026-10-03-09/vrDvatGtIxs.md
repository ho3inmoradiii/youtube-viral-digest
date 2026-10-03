# Autoresearch Made Our Models 3x Faster — Tejas Bhakta, Morph

- platform: youtube
- url: https://www.youtube.com/watch?v=vrDvatGtIxs
- channel: AI Engineer
- speaker: Tejas Bhakta، بنیان‌گذار Morph و پیش‌تر بهینه‌سازی اینفرنس در تسلا
- published: Sep 26, 2026 (dateText صفحهٔ watch در همین اجرا)
- views: 7,631
- views_source: `viewCount.simpleText` صفحهٔ watch در همین اجرا
- likes: 38
- likes_source: متن دسترسی «38 likes» همان صفحه
- duration: 7:30
- duration_source: نشان مدت روی تب ویدیوهای `@aiDotEngineer`
- topic: autoresearch روی کرنل GPU؛ ایده مال انسان، تنظیم مال حلقه
- text_source: شرح منتشرشدهٔ صفحهٔ watch. پلیر `LOGIN_REQUIRED` بود و زیرنویس جدا گرفته نشد

## خلاصه

شرح می‌گوید کرنل GPU برای autoresearch تقریباً هدف کامل است، چون تأییدش دوتایی است: درست یا غلط، سریع یا نه. تیم باکتا کرنل سفارشیِ نوشتهٔ ایجنت را با دستکاری bare-metal ترکیب کرده و مدل را سه برابر روی GPU ارزان‌تر سریع کرده.

قانونش: انسان ایده را می‌آورد و autoresearch تنظیم می‌کند. ایجنت در انتخاب اندازهٔ بلوک و پارامتر خوب است و در ایدهٔ بزرگ بد. مثال ایدهٔ بزرگ: دیدن اینکه یک گام attention دیپ‌سیک خیلی بیشتر از لازم کانتکست لود می‌کند. زمینهٔ لازم برای ایجنت را سخت‌افزار و خود مدل می‌داند.

reward hacking را با مثال غیرفعال کردن CUDA graph می‌گوید: یک کرنل تند می‌شود و کل مدل کند. سود کرنل‌ها را روی هم جمع‌شونده می‌خواند. دستکاری bare-metal را حدود ۲۵٪ اضافه بر VM ابری می‌گوید. هشدار صریح: حدود ۸۰٪ چیزی که autoresearch امتحان می‌کند بد است.

## نکته‌ها

- «سه برابر» و «حدود ۲۵٪» و «حدود ۸۰٪» عددهای خودِ شرح‌اند، نه اندازه‌گیری این اجرا.
- شرح نمی‌گوید روی کدام مدل یا کدام GPU ارزان این سه برابر گرفته شده.
