# حافظه جا ماند؛ کارِ باز اول صف است

صبح ریپو را باز کردم.
ایجنت خاطرهٔ دیروز را خواند و کاری را شروع کرد که شب قبل رها شده بود.

نسخهٔ ۱۳٫۲۹٫۰ Claude Mem، منتشرشده ۳ اکتبر، جلسه را با work state باز می‌کند، نه با حافظه. دو ابزار است: `work_state_write` و `work_state_read`. وضعیت کار یکی از todo و doing و done و dropped است. ردیف‌ها در دیتابیس worker می‌نشیند، نه در گیت، تا merge درگیرشان نشود. همان فهرست در worktreeهای همان checkout دیده می‌شود.

مقدمه تا ۳۰۰۰ نویسه است. اگر کاری باز نباشد، ۸۰۶ نویسه. حافظه باید در باقی‌ماندهٔ سقف ۱۰هزار نویسه‌ای جا شود. خود انتشار می‌گوید SessionStart روی runtime سرور هنوز این جدول را نمی‌خواند. ریل skip_ci همان روز همین شکاف را گفته بود.

حافظهٔ پر، فهرست خالی را جبران نمی‌کند.

اول کارِ باز را بنویس. خاطره هرچه جا ماند.

ایجنتت صبح کدام کارِ رهاشده را از نو شروع کرد؟

#work_state #ClaudeMem #حافظه #ایجنت #MCP #worktree #مهندسی_نرم‌افزار

---
source_videos:
  - title: "Claude Mem Adds Persistent To-Do List"
    url: https://www.instagram.com/reel/DeCkLnREYNS/
  - title: "claude-mem v13.29.0"
    url: https://github.com/thedotmack/claude-mem/releases/tag/v13.29.0
topic: open the session with the open to-do list and fit memory into what remains
generated_at: 2026-10-04T00:50:00+03:30
