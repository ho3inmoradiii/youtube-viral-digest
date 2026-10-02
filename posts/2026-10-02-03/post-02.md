# ژیمناستیک تایپ

سه هفته روی نوع برگشتی شرطی کار کردم. باگ پروداکشن هنوز `undefined` بود.

کتابخانه کوچک خودمان بود. در ریویو گفتند `any` ممنوع است. رفتم سراغ نوعی که اگر ورودی شخص است رشته برگردد و اگر سایت است URL. ادیتور همان خط `return` را قرمز نگه داشت، چون کامپایلر نوع را تا مقدار واقعی باز نمی‌کرد. یک overload اضافه کردم که فقط CI را سبز کند. کاربر هیچ‌کدام از این رقص را ندید. هفته بعد همان تابع روی داده ناقص API ترکید، چیزی که هیچ ژنریکی جلویش را نمی‌گرفت.

DHH برای Turbo اسمش را گذاشته ژیمناستیک تایپ. Svelte هم سورس فریم‌ورک را از تایپ‌اسکریپت درآورد و IntelliSense را با JSDoc نگه داشت، چون گام کامپایل برای خود کتابخانه کندشان کرده بود. کاربر نهایی هنوز می‌تواند تایپ بنویسد. چیزی که حذف شد، ترجمه اضافه در ریپوی خودشان بود. TypeScript 5.8 هم با `erasableSyntaxOnly` یادآوری می‌کند enum و namespace اصلاً تایپ خالص نیستند؛ کد اجرا می‌سازند.

تایپ برای اپ محصول هنوز به درد می‌خورد. برای سورس کتابخانه، اگر کامپایلر خودش مانع انتشار است، نوع قابل‌پاک‌شدن و کامنت کافی است. خط قرمز را با متغیر الکی ساکت نکن.

آخرین باری که `as any` گذاشتی تا پایپ‌لاین سبز شود، کی بود؟

#تایپ_اسکریپت #TypeScript #ژیمناستیک_تایپ #کدنویسی #فرانت_اند #کیفیت_کد
---
source_videos:
  - title: Big projects are ditching TypeScript… why?
    url: https://www.youtube.com/watch?v=5ChkQKUzDCs
  - title: TypeScript 5.8 Has 2 AWESOME Features
    url: https://www.youtube.com/watch?v=vcVoyLQMCxU
  - title: 4 NEW TypeScript 5.5 Features!
    url: https://www.youtube.com/watch?v=FhT87_CqPug
topic: TypeScript JavaScript new features
generated_at: 2026-10-02T03:40:00+0330
