# وسط پنجره می‌افتد

پنجره را که بزرگ‌تر کنی، وسطش همان جایی است که گم می‌شود.

الیزابت فوئنتس لئونه در AWS ایجنتی را مثال زد که باید لاگ اپلیکیشن را بخواند. هر بازیابی، همان لاگ را می‌ریزد داخل پنجره. جلسهٔ بعد، جلسهٔ قبل را هم با خودش می‌آورد، چون ایجنت همین‌طور یادش می‌ماند. گفت حدود یک سال پیش حرف این بود که توکن بیشتر درستش می‌کند. امروز نه. اگر داده خیلی بزرگ باشد، مدل اول و آخر را نگه می‌دارد و وسط را فراموش می‌کند. درصدی از مقاله نداد.

روی اسلاید، در Strands، نسبت خلاصه را در همان مثال ۵۰ درصد گذاشت و چهار پیام آخر را نگه داشت. سند فعلی `SummarizingConversationManager` پیش‌فرضش این نیست. `summary_ratio` پیش‌فرض ۰٫۳ است: موقع سرریز، حدود ۳۰ درصد از پیام‌های قدیمی خلاصه می‌شود، و مقدار بین ۰٫۱ و ۰٫۸ می‌ماند. `preserve_recent_messages` پیش‌فرض ۱۰ است، نه ۴.

خودش ضدالگو را هم نام برد. خلاصهٔ ساده‌لوحانه همان تکه‌ای را می‌اندازد که مدل برای جواب لازم داشت. برای لاگ، الگویی که نشان داد این بود که متن لاگ داخل پنجره نماند. ذخیره شود، یک شناسه در state ایجنت بماند، و فقط اگر واقعاً لازم شد با همان شناسه برگردد. بین ایجنت‌های یک swarm هم همان شناسه رد شود، نه کل پنجره.

سقف سه بار برای یک ابزار، مثال اسلاید بود. عدد بهینه نبود.

مهندسی کانتکست، به تعریف خودش: به مدل همان اطلاعاتی را بده که لازم دارد، همان وقت که لازم دارد.

آخرین باری که به‌جای بیرون بردن خروجی ابزار، پنجره را بزرگ کردی، وسطش چه چیزی افتاد؟

#کانتکست #ایجنت #Strands #لاگ #مهندسی_نرم‌افزار #lost_in_the_middle

---
source_videos:
  - title: "Why Bigger Context Windows Won't Save Your Agent — Elizabeth Fuentes Leone, AWS"
    url: https://www.youtube.com/watch?v=DrfyORO8RqA
  - title: "SummarizingConversationManager"
    url: https://strandsagents.com/docs/api/python/strands.agent.conversation_manager.summarizing_conversation_manager/
  - title: "Conversation Management"
    url: https://strandsagents.com/docs/user-guide/sdk/agents/conversation-management/
topic: context engineering, memory pointer instead of a bigger window
generated_at: 2026-10-08T06:54:00+03:30
