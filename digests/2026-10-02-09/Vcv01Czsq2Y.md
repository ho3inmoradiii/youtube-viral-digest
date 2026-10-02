# هفت قابلیت CSS که جای جاوااسکریپت UI را تنگ می‌کند

- **عنوان:** 7 CSS Features Coming in 2026 That KILL JavaScript
- **لینک:** https://www.youtube.com/watch?v=Vcv01Czsq2Y
- **کانال:** camelCase
- **بازدید:** 55648
- **موضوع:** web platform APIs latest 2026

## خلاصه

ویدیو هفت قابلیت را از «همین حالا baseline» تا «فقط در بعضی مرورگرها» جدا می‌کند. Anchor positioning با popover تول‌تیپ و منو را به عنصر هدف می‌چسباند، حتی اگر در DOM کنار هم نباشند. position-try-fallbacks مثل flip-block و flip-inline، اگر جا نبود خودش جهت را عوض می‌کند و لازم نیست به scroll و resize گوش بدهید و مختصات حساب کنید. مشکل stacking context تول‌تیپ مطلق داخل کامپوننت هم با این مدل کمتر می‌شود.

`@scope` محدودهٔ قانون را بدون سلکتور صلب و specificity بالا می‌سازد. scope دوناتی یعنی قانون از یک نقطه شروع شود و قبل از یک زیرشاخه (مثلاً آواتار) قطع شود. برخلاف `.posts .post img`، قانون scoped آن‌قدر خاص نیست که برای دارک‌مود مجبور به `!important` شوید. این قابلیت چند هفته است baseline شده.

Scroll-driven animation با `animation-timeline: scroll` و `view` نوار پیشرفت و fade-in ورود به viewport را بدون GSAP انجام می‌دهد. پوشش فعلی Chrome و Edge و Safari حدود ۹۵ درصد کاربران است و فایرفاکس هنوز کامل نیست. `sibling-index()` و `sibling-count()` تأخیر پلکانی و اندازهٔ داینامیک را بدون nth-child دستی حساب می‌کنند؛ در Chrome و Safari هستند.

کاروسل CSS با `::scroll-button` و `::scroll-marker` اسلایدر و ویزارد را بدون JS می‌سازد ولی فعلاً عمدتاً Chrome است. Masonry بعد از سال‌ها بحث، مسیر `display: grid-lanes` را گرفته و اول در Safari پیاده شده. Interest Invoker API هاور واقعی تول‌تیپ را با interest-delay پوشش می‌دهد تا حرکت ماوس از تریگر به خود تول‌تیپ تول‌تیپ را نبندد. بخش میانی ویدیو معرفی پلتفرم هاست است و به قابلیت‌ها مربوط نیست.

## نکات کلیدی

- Anchor positioning و `@scope` همین حالا در مرورگرهای اصلی قابل‌اتکا هستند.
- `@scope` سلکتور ضعیف ولی مکانی می‌دهد تا جنگ specificity و `!important` کمتر شود.
- انیمیشن مبتنی بر اسکرول، listenerهای جاوااسکریپت layout را برای خیلی از افکت‌ها حذف می‌کند.
- کاروسل CSS و Interest Invoker هنوز همه‌جا نیستند؛ استفادهٔ تولیدی باید با baseline چک شود.
- حذف JS وقتی برد است که رفتار را خود مرورگر تضمین کند، نه وقتی فقط دموی کنفرانس است.

## برش کوتاه

> هر بار `!important` می‌نویسید، در خیلی از موارد میان‌بر زده‌اید. `@scope` قانون را مکانی محدود می‌کند بدون اینکه specificity را آن‌قدر بالا ببرد که دیگر نشود بازنویسی‌اش کرد.
