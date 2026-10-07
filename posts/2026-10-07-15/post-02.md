# قفل روی پل است

توکن capability و سوکت کاربر جاری، باینری را سندباکس نمی‌کند.

`SECURITY.md` ریپوی `morluto/rea` همین جمله را دارد. هر نشست پل با یک توکن تصادفی و یک سوکت یونیکس کاربر جاری احراز می‌شود. توکن از توصیفگر نشست خصوصی رد می‌شود. از آرگومان پروسه رد نمی‌شود. از متغیر محیط هم رد نمی‌شود. همان بند می‌گوید این در برابر پروسهٔ مخربی که از قبل با همان کاربر سیستم بالا است محافظتی ندارد. باز کردن باینری نامطمئن، تجزیه را به ابزار محلی همان کاربر می‌سپارد.

در `BridgeLauncher.ts` فایل بوت‌استرپ لانچر با `mode: 0o600` نوشته می‌شود و همان mode رویش `chmod` می‌شود. شرح ویدیو سوکت را mode-0600 خوانده. فایلی که این اجرا خط mode را در آن دید، بوت‌استرپ است. `SECURITY.md` خود سوکت را سوکت یونیکس کاربر جاری می‌نامد.

README هم Process Capture را جدا می‌گوید. پروسه با مجوز کاربر اجرا می‌شود، و این ضبط سندباکس امنیتی نیست. تحلیل ایستای جاوااسکریپت هم ماژول استخراج‌شده را اجرا نمی‌کند. API گیت‌هاب همین اجرا: ۱۱۶۱۳ ستاره، MIT، و push در `2026-10-07T12:06:24Z`.

اگر این پل را به ایجنت دادی، کدام پروسه هنوز با کاربر خودت بالا می‌آید؟

#امنیت #MCP #سندباکس #ایجنت #مهندسی_نرم‌افزار #REA

---
source_videos:
  - title: "REA GitHub Explained: Local Evidence Graphs for AI Coding Agents"
    url: https://www.youtube.com/watch?v=4QEkWz0yPOk
  - title: "morluto/rea SECURITY.md"
    url: https://github.com/morluto/rea/blob/main/SECURITY.md
  - title: "morluto/rea BridgeLauncher.ts"
    url: https://github.com/morluto/rea/blob/main/src/hopper/BridgeLauncher.ts
topic: capability token on the bridge, analysis still runs as the user
generated_at: 2026-10-07T15:40:00+03:30
