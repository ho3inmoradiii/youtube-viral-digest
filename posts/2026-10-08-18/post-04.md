# یک آواتار، صفحهٔ استاتیک را داینامیک می‌کند

نکست ۱۶٫۴، که ۶ اکتبر منتشر شد، می‌گوید Cache Components در نکست ۱۷ پیش‌فرض می‌شود. از همین نسخه آن را برای هر اپ توصیه می‌کند. اپ تازهٔ `create-next-app` همین حالا با این مدل بالا می‌آید.

`'use cache'` را مثل هدر Cache-Control برای یک کامپوننت توصیف کرده‌اند. خوشامد کاربر جاری هر درخواست رندر می‌شود. لیست پروژه‌ها می‌تواند کش شود. انعطاف همین است. هزینه هم همین‌جا قایم می‌شود. یک کامپوننت داینامیک می‌تواند صفحه‌ای را که باید استاتیک بماند ببرد سمت رندر زمان درخواست.

`ensureStatic = 'navigation'` یعنی اگر آن تکه، مثلاً آواتار کاربر، وارد صفحه شود، بیلد می‌شکند. می‌شود آن را روی لی‌اوت ریشه گذاشت. برای اینباکس، prefetch هر لینک کل ترد را از قبل می‌کشد، حتی پیامی که باز نمی‌شود. `await navigation()` همان ترد را تا ناوبری واقعی عقب می‌اندازد. `prefetch()` جداست و محتوا را تا یک prefetch صریح از پوستهٔ اولیه بیرون می‌گذارد.

ویدیوی امروز این دو را در رونویسی قاطی کرد و «await prefetch» گفت. دستور ارتقا را هم جویده. شکل پست رسمی این است: `npx next@canary upgrade --agent=latest`.

بازخورد ایجنت برای اپ تازهٔ create-next-app روشن است. اپ موجود باید خودش `experimental.agentFeedback` را روشن کند. پیش‌نویس در مرورگر باز می‌شود. کد و لاگ و راز نباید داخلش باشد. تا Send را نزنی چیزی نمی‌رود. در CI اجرا نمی‌شود و تله‌متری می‌خواهد.

اگر یک آواتار داینامیک بیلد سایت بازاریابی را قرمز کند، کامپوننت را درمی‌آوری یا گارد را؟

#Nextjs #CacheComponents #فرانت‌اند #ایجنت #بیلد #پری‌فچ

---
source_videos:
  - title: "Next.js 17 Is Coming: Learn Cache Components Now (16.4 Update)"
    url: https://www.youtube.com/watch?v=paQbukUXE8w
  - title: "Next.js 16.4"
    url: https://nextjs.org/blog/next-16-4
topic: ensureStatic fails the build when a dynamic piece enters a static route; agent feedback is a draft until Send
generated_at: 2026-10-08T19:10:00+03:30
