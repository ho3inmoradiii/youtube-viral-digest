# ایجنت کاروسل را از نو نوشت؛ مرورگر از قبل داشت

ده خط CSS که مرورگر حالتش را بلد است، بهتر از چهارصد خط جاوااسکریپتی است که ایجنت با درصد ارتفاع ساخته.

دیروز از ایجنت یک کاروسل محصول خواستم. خروجی یک بلوک کی‌فریم بود که ارتفاع کارت را نسبتی ثابت از ویوپورت فرض کرده بود. روی دسکتاپ قشنگ بود. روی موبایل کارت کوتاه‌تر شد و ورود و خروج به هم گره خورد. همان مقایسهٔ کروم در راهنمای اسکرول‌درایون: ایجنت بدون راهنما درصد می‌نویسد و با تغییر اندازه می‌شکند. نسخهٔ راهنما ورود و خروج را جدا می‌کند، `animation-timeline` و `animation-range` را چک می‌کند، و اگر نباشند می‌افتد روی `IntersectionObserver`.

بدتر این است که از کروم ۱۳۵ خود کاروسل هم بدون جاوااسکریپت درآمده. `overflow` و `scroll-snap`، بعد `::scroll-button` و `::scroll-marker`، و `:target-current` برای نقطهٔ فعال. در کروم ۱۴۰ با `scroll-target-group: auto` اسکرول‌اسپای فهرست هم دو خط CSS است. مرورگر دکمهٔ انتهای لیست را خودش disable می‌کند. من هنوز از ایجنت ماشین state می‌خواستم.

DevTools نسخهٔ ۱۵۱ تا ۱۵۳ هم ابزار را داده دست ایجنت، نه فقط دست ما. specificity روی هاور سلکتور، soft navigation در پنل پرفورمنس، و MCP برای هیپ‌اسنپ‌شات. از کروم ۱۵۳ چرخهٔ رلیز دو هفته‌ای شده. اگر ایجنتت پلتفرم این ماه را در کانتکست ندارد، فیچر ۲۰۱۹ را با اعتمادبه‌نفس ۲۰۲۶ می‌نویسد.

آخرین بار ایجنتت کدام API مرورگر را از نو اختراع کرد، فقط چون در کانتکستش نبود؟

#CSS #ChromeDevTools #WebPlatform #کاروسل #ScrollDriven #فرانت_اند #AIAgents

---
source_videos:
  - title: "Modern Web Guidance: Scroll-driven entry and exit effects"
    url: https://www.youtube.com/watch?v=kbjHnZOQgkQ
  - title: "94: CSS carousels (and scroll)"
    url: https://www.youtube.com/watch?v=btIOhb6AiOc
  - title: "What's New: Chrome DevTools 151-153"
    url: https://www.youtube.com/watch?v=vukchAoaTdE
topic: web platform APIs vs agent-reinvented UI
generated_at: 2026-10-02T12:40:00+03:30
