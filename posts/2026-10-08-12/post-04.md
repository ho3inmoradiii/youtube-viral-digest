# ۰٫۸۵۱ فقط خانهٔ توسعه است

ریل می‌گوید Kev-27B دقت ۰٫۸۵۱ دارد و تا یک صدم به Jev با ۰٫۸۵۷ نزدیک است.

جدول README روی main چیز دیگری است. هر خانه development / test است. دقت Kev-27B روی منبع تازه ۰٫۸۵۱ / ۰٫۸۸۹ است. Jev فقط ۰٫۸۵۷ روی development دارد و خانهٔ test خالی است. جملهٔ خود README این است که روی منبع تازه تا یک صدم نزدیک است، و چون نمی‌دانیم Jev روی چه چیزی آموزش دیده، این مقایسهٔ کنترل‌شدهٔ دو معماری نیست. Jev را فقط روی مجموعهٔ development همین سوئیت‌ها اجرا کرده‌اند.

شاخص تصحیح‌شدهٔ شانس روی breadth-v1 برای Kev-27B برابر ۵۲٫۳ است و برای Jev برابر ۵۴٫۰. Brier منبع تازه روی development برای Kev برابر ۰٫۲۲۵ است و برای Jev برابر ۰٫۲۱۱. پایین‌تر بهتر است. کپشن این دو را نگفت.

شروع را README روی Kev-4B گذاشته، نه برچسب default. آموزش همان ۴B روی H100 را «حدود ۱ دلار» نوشته. Kev-27B به GPU هشتاد گیگابایت نیاز دارد و ۵۱ گیگابایت وزن bf16 است. API را با System One یکی کرده تا SDK پایتون TypeSafe به سرور محلی اشاره کند. ستارهٔ همین اجرا ۸۶۹۴ بود، Apache-2.0، و push در ۶ اکتبر.

اگر این ۰٫۸۵۱ را بدون ستون test و بدون جملهٔ «مقایسه کنترل‌شده نیست» به مدیر ببری، کدام خانهٔ جدول را نشانش می‌دهی؟

#Kev #Jev #ارزیابی #مدل #مهندسی_نرم‌افزار #OpenSource

---
source_videos:
  - title: "Kev: Open-Source Clone of Jev Scores 0.851 Accuracy"
    url: https://www.instagram.com/reel/DeNfj1SESmL/
  - title: jaredpalmer/kev README
    url: https://github.com/jaredpalmer/kev
topic: caption flattens a development/test cell and skips the uncontrolled-comparison sentence
generated_at: 2026-10-08T13:05:00+03:30
