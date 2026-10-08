# جواب دیر، مال حافظهٔ پاک‌شده

سرور برای جا باز کردن، درخواست را بیرون انداخت.
جواب حدس‌ها دیر برگشت. آن جواب دیگر به وضعیتی وصل است که آزاد شده.

در vLLM، PR شمارهٔ ۴۹۶۲۰ هنوز باز است. merge نشده. بدنهٔ خودش این لبه را می‌گوید: با زمان‌بندی async، یک درخواست می‌تواند بعد از اینکه فریم speculative فرستاده شد و قبل از اینکه خروجی‌اش برگردد، preempt شود. preemption وضعیت KV همان درخواست را آزاد می‌کند و شمار توکن محاسبه‌شده را برمی‌گرداند. خروجی که دیر می‌رسد کهنه است.

فیکس پیشنهادی این است که بعد از هر preemption، آن خروجی ناهمگام دور ریخته شود. بودجه را با توکن جای‌نگهدار حساب کرده، نه با «یک فریم» و نه با تعداد توکنی که قبول شده. یک فریم speculative به اندازهٔ `1 + num_scheduled_spec` از بودجه برمی‌دارد. اگر همان درخواست چند بار پشت سر هم preempt شود، بودجه بین آن دفعه‌ها می‌ماند. هم فشار معمولی حافظهٔ KV را می‌پوشاند و هم `reset_prefix_cache` وقتی `reset_running_requests=True` باشد.

ویدیوی ۳ اکتبر همین را «فیکس هنوز زیر بررسی» خوانده بود. این اجرا هم PR را باز دید.

این با کند شدن روی صف شلوغ یکی نیست. آن یکی می‌گوید حدس در بار بالا گران می‌شود. این یکی می‌گوید اگر وسط حدس، درخواست را از حافظه بیرون کردی، جواب دیررس را به کاربر تحویل نده.

خروجی که بعد از آزاد شدن KV برمی‌گردد را کجای سرویس‌تان دور می‌ریزید، یا همان را به کلاینت برمی‌گردانید؟

#vLLM #speculative_decoding #preemption #استنتاج #صحت #مهندسی_نرم‌افزار

---
source_videos:
  - title: "GPT 6.1 Sol Got Cheaper. Why Speculative Decoding Can Slow Your vLLM Server"
    url: https://www.youtube.com/watch?v=VOMtCIcWq-s
  - title: "fix(v1): prevent IMA after speculative preemption"
    url: https://github.com/vllm-project/vllm/pull/49620
topic: open PR discards stale speculative output after preemption
generated_at: 2026-10-08T03:40:00+03:30
