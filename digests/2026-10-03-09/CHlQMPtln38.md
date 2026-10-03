# Why Your Agent Still Needs Retrieval - Carly Richmond, Elastic

- platform: youtube
- url: https://www.youtube.com/watch?v=CHlQMPtln38
- channel: Mastra
- speaker: Carly Richmond، لید developer advocate در Elastic
- published: Sep 30, 2026 (dateText صفحهٔ watch در همین اجرا)
- views: 496
- views_source: `viewCount.simpleText` صفحهٔ watch در همین اجرا
- likes: 8
- likes_source: متن دسترسی «8 likes» همان صفحه
- duration: 21:38
- duration_source: نشان مدت در نتیجهٔ جست‌وجوی «RAG agent tool calling patterns» با فیلتر این هفته
- topic: RAG عاملیتی، جست‌وجوی برداری در برابر واژگانی، شرح ابزار
- text_source: شرح منتشرشدهٔ صفحهٔ watch. پلیر `LOGIN_REQUIRED` بود و زیرنویس جدا گرفته نشد
- recorded: TypeScript AI Conference، لندن، ۲۳ ژوئیه ۲۰۲۶، ارائهٔ Mastra (طبق همان شرح)

## خلاصه

ریچموند استدلال می‌کند ایجنت هنوز retrieval می‌خواهد. بدون آن فقط از چیزی جواب می‌دهد که مدل در آموزش دیده. آن دانش تاریخ انقضا دارد، سوگیری داده را با خود می‌آورد، و ارزیابی‌هایی شکلش داده‌اند که حدس مطمئن را به اعترافِ ندانستن ترجیح می‌دهند. retrieval اطلاعات درست را قبل از جواب جلوی مدل می‌گذارد.

مثال، ایجنت Mastra است که دربارهٔ فیلم علمی‌تخیلی جواب می‌دهد. جست‌وجوی برداری با معنی نزدیک می‌کند، پس کوئری Han Solo کنار Luke و Leia می‌نشیند. جست‌وجوی واژگانی عبارت دقیق را می‌زند و برای چیزی مثل نام شرکت هنوز مناسب‌تر است. RAG عاملیتی retrieval را ابزار می‌کند تا خود ایجنت تصمیم بگیرد کی بگردد. rerank ترتیب همان نتایج را با reciprocal rank fusion، امتیاز وزنی، یا مدل reranker عوض می‌کند.

لغزش را شرح ابزار می‌داند. اگر مبهم باشد، ایجنت یا هیچ ابزاری را صدا نمی‌زند، یا ابزار غلط، یا ابزار درست با پارامتر غلط. دمو روی vector store الاستیک در Mastra است و ربط را با scorer در Mastra Studio چک می‌کند. پرسش‌وپاسخ به سند نزدیک‌به‌تکراری در مقیاس، و غلط املایی می‌رسد.

شرح به مقالهٔ Why Language Models Hallucinate (`https://arxiv.org/abs/2509.04664`) لینک داده. عدد تازه‌ای از آن مقاله در خود شرح نیست.

## نکته‌ها

- بازدید پایین است (۴۹۶) ولی شرح، برخلاف خیلی از نتیجهٔ همین هفته، ادعای مشخص دارد.
- «شرح ابزار را مثل پرامپت بنویس» در فهرست فصل‌ها هم هست (۱۱:۳۱). جزئیات جملهٔ روی صحنه در شرح نیامده.
