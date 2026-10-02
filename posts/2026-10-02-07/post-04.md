# سیصد کیلوبایت برای یک تولتیپ

تولتیپ ما حدود شصت خط جاوااسکریپت داشت. مرورگر همان کار را با Popover API و حدود ده خط HTML می‌کند. ما هنوز پکیج نصب می‌کردیم.

اسپرینت پرفورمنس بود. LCP لندینگ حدود ۳٫۸ ثانیه، INP موبایل بالای ۵۰۰ میلی‌ثانیه. پیشنهاد این بود یک لایبرری انیمیشن اسکرول اضافه کنیم. در DevTools تسک‌های بلند روی main thread را دیدم: هر فریم اسکرول، همان تردی که باید به کلیک جواب بدهد مشغول حساب کتاب بود. نسخهٔ CSS که کار را به کامپوزیتور می‌سپارد همان حرکت را می‌دهد، بدون این‌که INP را گروگان بگیرد. خوب بودن INP یعنی زیر ۲۰۰ میلی‌ثانیه، نه اسلاید «بهینه‌سازی شد».

همان الگو برای مودال هم بود. Radix داشتیم تا فوکوس و Escape را مدیریت کند، در حالی که `dialog` بومی همان را دارد. یک کیس در همین بحث، پروژهٔ HTMX، با تکیه بر پلتفرم حدود ۹۶٪ وابستگی را کم کرده. جهت مه ۲۰۲۶ هم همین است: حالت باز dialog با CSS، ویدیو تا دیده نشد بار نشود، container query اگر فقط نام دارد یعنی محدودهٔ استایل نه اندازه. ما بودجه را با پکیج تازه پر کردیم.

اصل کمترین قدرت لازم ضد جاوااسکریپت نیست. می‌گوید ساده‌ترین ابزار مقاوم را بردار. قبل از `npm install` بپرسید مرورگر این کار را همین الان بلد است یا نه.

آخرین پکیجی که از پروژه حذف کردید کدام بود، و چند کیلوبایت واقعی برگشت؟

#وب_پلتفرم #CoreWebVitals #INP #CSS #فرانت_اند #کارایی #جاوااسکریپت

---
source_videos:
  - title: Browser APIs Just Killed Off Your JavaScript Dependencies
    url: https://www.youtube.com/watch?v=jHRHV1MNR5s
  - title: Core Web Vitals 2025 Explained: INP, LCP, CLS & How to Boost Your Site Speed!
    url: https://www.youtube.com/watch?v=m_yWVuf8ZkE
  - title: Web Platform Changes in May 2026: What Actually Matters
    url: https://www.youtube.com/watch?v=6EH2AC2vsXw
topic: web platform APIs and Core Web Vitals
generated_at: 2026-10-02T07:36:00+0330
