# بدون قفس، دستور نرو

جدول پاس را دیدم و خواستم همان را نصب کنم.
خود ویدیو می‌گوید آن جدول مال قبل از Pi نسخهٔ ۱ است و هنوز دوباره ران نشده.

رقم ۶۶ و ۶۵ را اندازه‌گیری این اجرا حساب نکردم. چیزی که سند گفت این است. ابزار پیش‌فرض Pi چهار تاست: read و bash و edit و write. راهنمای شروع می‌گوید قبل از هر ابزار اجازه نمی‌گیرد، و برای کار نامطمئن باید کانتینر بگذاری. تازه‌ترین انتشاری که API گیت‌هاب این اجرا نشان داد `v1.0.4` بود، مورخ ۵ اکتبر ۲۰۲۶.

DeepSeek Harness اگر روی میزبان بک‌اند سندباکس نباشد، دستور را بدون حصر اجرا نمی‌کند. خطا `SANDBOX_UNAVAILABLE` است و راه فرارش را `danger-full-access` نام می‌برد، نه اجرای بی‌صدا. هر دو ریپو MITاند. ستارهٔ همین اجرا برای Pi برابر ۱۱۲۸۵۵ و برای DeepSeek Harness برابر ۲۴۴۳۳۱ بود.

سالتزر و شرودر به این پیش‌فرض می‌گویند شکستِ امن. ستارهٔ بیشتر جای قفس را نمی‌گیرد.

ایجنت تو وقتی سندباکس نیست می‌ایستد، یا همان دستور را بیرون از قفس اجرا می‌کند؟

#سندباکس #Pi #DeepSeek #هارنس #fail_closed #مهندسی_نرم‌افزار

---
source_videos:
  - title: "DeepSeek Harness vs Pi: Which Free Coding Agent Wins"
    url: https://www.youtube.com/watch?v=gGqi-wcyHc4
  - title: "Pi settings — default tools"
    url: https://pi.dev/docs/latest/settings
  - title: "DeepSeek Harness sandbox contract"
    url: https://github.com/deepseek-ai/deepseek-harness/blob/master/packages/sandbox/sandbox/README.md
topic: stale scoreboard; Pi's four tools versus a fail-closed sandbox
generated_at: 2026-10-06T15:46:00+03:30
