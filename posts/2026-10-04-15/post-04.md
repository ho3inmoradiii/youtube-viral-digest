# OnPush را هنوز دستی می‌نویسد

OnPush را دستی نوشت.
از Angular ۲۲ آن حالت پیش‌فرض است.

فایل best-practices روی angular.dev به مدل می‌گوید `standalone: true` را داخل دکوراتور ننویس، چون از نسخهٔ ۲۰ پیش‌فرض است. `OnPush` را هم صریح نگذار، چون از نسخهٔ ۲۲ پیش‌فرض است. فرم تازه را Signal Forms می‌خواهد و می‌گوید در ۲۲ پایدار است. برای سرویس تک‌نسخه، دکوراتور `@Service` را به `@Injectable({providedIn: 'root'})` ترجیح می‌دهد. کنترل جریان را `@if` می‌خواهد، نه ستارهٔ ساختاری قدیمی.

تگ پایدار `v22.2.1` روی گیت‌هاب تاریخ `2026-09-30` دارد. ویدیوی سوم اکتبر از Fable می‌پرسد Angular ۲۲ را دیده یا نه. جواب به قطع آموزش حوالی انتشار ۲۲ برمی‌گردد. MCP آزمایشی CLI سند زنده را برای همین گفتگو می‌آورد. خود گوینده گفت این بازیابی، دانش پایه را عوض نمی‌کند. فقط جواب همین نوبت را.

سند زنده وزن مدل نیست. جلسهٔ بعد، اگر همان فایل دوباره داخل زمینه نباشد، OnPush اضافه برمی‌گردد.

تا دستور نسخهٔ جاری داخل زمینه باشد، ایجنت Angular دیروز را روان‌تر می‌نویسد.

آخرین کامپوننتی که ایجنتت ساخت، OnPush را هنوز دستی نوشته بود؟

#Angular #OnPush #MCP #ایجنت #RAG #فرانت_اند #مهندسی_نرم‌افزار

---
source_videos:
  - title: "How Angular Uses MCP AI Agents to Keep Code Up to Date (Setup & Workaround)"
    url: https://www.youtube.com/watch?v=qpgNRJgu8FM
  - title: "LLM prompts and AI IDE setup"
    url: https://angular.dev/ai/develop-with-ai
  - title: "angular/angular release v22.2.1"
    url: https://github.com/angular/angular/releases/tag/v22.2.1
topic: current Angular defaults are in the docs, not in the model's weights
generated_at: 2026-10-04T15:50:00+03:30
