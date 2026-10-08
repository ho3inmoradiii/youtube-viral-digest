# حدس روی سرور خلوت، کندی روی سرور شلوغ

- platform: youtube
- url: https://www.youtube.com/watch?v=VOMtCIcWq-s
- channel: The Augmented Expert
- title: GPT 6.1 Sol Got Cheaper. Why Speculative Decoding Can Slow Your vLLM Server
- published: صفحهٔ watch همین اجرا `dateText` را `Oct 3, 2026` نشان داد. Invidious جست‌وجو `publishedText` را `4 days ago` داد. فیلد `published` جست‌وجو در اجراهای قبلی به زمان fetch می‌چسبید و این‌جا زمان دقیق حساب نشد
- views: صفحهٔ watch همین اجرا `381 views`
- likes: عبارت `like this video along with N other people` در HTML دیده نشد
- duration_seconds: ۶۴۷ از `lengthSeconds` نتیجهٔ جست‌وجوی Invidious. `/api/v1/videos/VOMtCIcWq-s?hl=en` این اجرا ۵۰۰ داد
- metrics_source: HTML صفحهٔ watch و نتیجهٔ جست‌وجوی `invidious.f5.si`
- topic: speculative decoding در vLLM؛ شتاب در QPS پایین و کندی در QPS بالا، به‌علاوهٔ PR باز برای خروجی کهنه بعد از preemption
- text_source: گفتار WebFetch صفحهٔ watch، شرح همان صفحه، وبلاگ https://vllm.ai/blog/2024-10-17-spec-decode به تاریخ ۱۷ اکتبر ۲۰۲۴، سند فعلی https://docs.vllm.ai/en/latest/features/speculative_decoding/ ، و بدنهٔ https://github.com/vllm-project/vllm/pull/49620

## خلاصه

ویدیو قیمت GPT 6.1 Sol را زمینه می‌گذارد و می‌گوید کارت سیستم OpenAI نمی‌گوید مدل چطور سرو می‌شود، پس هیچ جمله‌ای از این قسمت ادعایی دربارهٔ سرور OpenAI نیست. این اجرا کارت سیستم و صفحهٔ Artificial Analysis باز نشد. برچسب ۲ و ۱۰ دلار برای هر میلیون توکن قبلاً در اجرای `2026-10-08-00` از روی حرف Theo آمده بود. پست این اجرا از همان برچسب شروع نمی‌کند.

عددهایی که با وبلاگ vLLM جور شد از ۱۷ اکتبر ۲۰۲۴ است، نه یک اندازه‌گیری ۲۰۲۶. روی Llama 3 70B و چهار H100، در یک پرس‌وجو بر ثانیه: مدل پیش‌نویس (`turboderp/Qwama-0.5B-Instruct`) تا ۱٫۵ برابر روی ShareGPT، و n-gram تا ۲٫۸ برابر روی خلاصهٔ CNN/DailyMail. همان صفحه برای QPS بالا می‌گوید ۱٫۴ برابر کندتر روی ShareGPT و ۱٫۸ برابر کندتر روی CNN/DailyMail. مقدار عددی آن QPS بالا در متن وبلاگ نیست. مثال وبلاگ برای یک قدم: پیش‌نویس پنج توکن `I like cooking and traveling` می‌دهد، هدف `playing` می‌خواهد، و همان قدم `I like playing` را بیرون می‌دهد.

سند فعلی، همین قابلیت را برای کم کردن تأخیر بین توکن‌ها در QPS متوسط تا پایین و بار حافظه‌محور معرفی می‌کند. جدول کیفی همان صفحه برای n-gram در QPS بالا «بهرهٔ متوسط» نوشته است، نه کندی ۱٫۸ برابر. این دو منبع یکی نیستند.

ویدیو یک مثال حسابی با سه توکن پیش‌نویس می‌دهد: ۳۲ درخواست همزمان ۹۶ جایگاه، و ۲۵۶ درخواست ۷۶۸ جایگاه. خودش می‌گوید این بنچمارک نیست. وارد پست نشد.

PR شمارهٔ ۴۹۶۲۰ هنوز باز است و merge نشده. بدنه می‌گوید با زمان‌بندی async، درخواست می‌تواند بعد از ارسال یک فریم speculative و قبل از برگشتن خروجی‌اش preempt شود. preemption وضعیت KV را آزاد می‌کند و خروجی دیررس کهنه است. PR خروجی کهنه را بعد از هر preemption دور می‌ریزد. بودجه را با واحد توکن جای‌نگهدار حساب می‌کند: یک فریم speculative به‌جای یک فریم، `1 + num_scheduled_spec` مصرف می‌کند، نه تعداد توکن پذیرفته‌شده. همان بودجه بین preemptionهای پشت‌سرهم می‌ماند. هم preemption معمولی زیر فشار KV را می‌پوشاند و هم `reset_prefix_cache(reset_running_requests=True)`.

کلید `num_speculative_tokens_per_batch_size` و مثال ۱ تا ۶۴ و ۶۵ تا ۱۲۸ و ۱۲۹ تا ۵۱۲ در HTML سند فعلی که این اجرا خواند نبود. آن آستانه وارد پست نشد. جملهٔ ویدیو دربارهٔ lookahead slot و پیش‌فرض recompute در نسخهٔ ۱ هم این اجرا در سند جدا چک نشد.

## نکته‌های کلیدی

- وبلاگ ۱۷ اکتبر ۲۰۲۴: تا ۱٫۵ برابر و تا ۲٫۸ برابر در یک پرس‌وجو بر ثانیه، و ۱٫۴ و ۱٫۸ برابر کندتر در QPS بالا، Llama 3 70B روی چهار H100
- سند فعلی هنوز دامنه را QPS متوسط تا پایین می‌گذارد و جدول n-gram را در QPS بالا «بهرهٔ متوسط» می‌خواند
- PR 49620 باز است: خروجی speculative بعد از preemption کهنه است و باید دور ریخته شود
- بودجهٔ دور ریختن: `1 + num_scheduled_spec`

## چه وارد پست نشد

- قیمت ۲/۱۰ در برابر ۱۰/۵۰ و امتیاز ۵۲ در برابر ۵۳. صفحهٔ Artificial Analysis این اجرا باز نشد و زاویه با پست نیمهٔ شب تکرار می‌شد
- آستانهٔ مثالی طول پیش‌نویس بر اساس همزمانی. در سند خوانده‌شده پیدا نشد
- حساب ۳۲ در ۹۶ و ۲۵۶ در ۷۶۸. ویدیو آن را بنچمارک نخواند
- ادعای ویدیو که پیش‌فرض نسخهٔ ۱ بازمحاسبه است، نه جابه‌جایی به CPU
