# Lessons from Generating 12 Trillion Synthetic Tokens — Bogdan Gaza, DatologyAI

- platform: youtube
- url: https://www.youtube.com/watch?v=FQwTqUmcbRg
- channel: AI Engineer
- speaker: Bogdan Gaza, هم‌بنیان‌گذار و CTO در DatologyAI
- published: Oct 2, 2026 (dateText صفحهٔ watch در همین اجرا)
- views: 739
- views_source: صفحهٔ watch در همین اجرا
- likes: 1
- likes_source: factoid لایک همان صفحه
- duration: 20:32
- duration_source: نشان مدت روی تب ویدیوهای کانال (`animationActivationTargetId`)
- topic: زیرساخت دادهٔ مصنوعی در مقیاس تریلیون توکن
- text_source: شرح منتشرشده و فهرست فصل‌ها. گفتار کامل گرفته نشد

## خلاصه

بوگدان گازا می‌گوید متن قابل‌استفادهٔ وب حدود ۳۰ تریلیون توکن است و پیش‌آموزش مدل مرزی بیشتر می‌خواهد. درس مهندسی را از جاب‌های دادهٔ مصنوعی در مقیاس تریلیون توکن می‌گوید، از جمله یک اجرای اخیر حدود ۱۲ تریلیون توکن روی وب و ریاضی و کد. دستور ساخت را BeyondWeb می‌نامد: بازنویسیِ بذردار، نه خواستن دادهٔ مصنوعی از صفر از مدل. مقاله را در شرح لینک کرده: https://arxiv.org/pdf/2508.10975

از یک چیدمان دوتکهٔ Slurm/Kubernetes رفته‌اند به یک پایپلاین Ray و KubeRay و vLLM روی EKS روی HyperPod. یک گردش کار را curate، synthesize، train، eval می‌نامد.

چهار گلوگاه را نام می‌برد. متادیتای S3: با batch کردن fetch، چیزی که ۹ تا ۱۱ روز طول می‌کشید به حدود ۲ ساعت رسیده. خرابی GPU: پارتیشن اندازه‌مناسب به‌اضافهٔ checkpoint تا شکست قابل‌بازیابی باشد. زمان‌بندی بین کلاستر برای CPU و GPU با هم. تنظیم استنتاج: sweep پرچم‌های vLLM برای حدود ۴۰٪ throughput بیشتر. فصل جمع‌بندی می‌گوید از ۳۰ میلیارد به ۱۲ تریلیون توکن مصنوعی رسیده‌اند.

## نکته‌ها

- عدد ۹–۱۱ روز در برابر حدود ۲ ساعت مال متادیتای S3 است، نه مال خودِ GPU.
- بازنویسیِ بذردار را در برابر ساخت از صفر گذاشته.
- حدود ۴۰٪ مال sweep پرچم vLLM در همین شرح است.
