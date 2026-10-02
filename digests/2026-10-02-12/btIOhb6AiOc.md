# 94: CSS carousels (and scroll)

- platform: youtube
- url: https://www.youtube.com/watch?v=btIOhb6AiOc
- channel: Chrome for Developers
- creators: Una و Bramus (CSS Podcast)
- published: 2026-09-28
- views: 4817
- duration_seconds: 997
- topic: CSS carousel APIs / scroll

## خلاصه

اپیزود ۹۴ پادکست CSS می‌گوید کاروسل در اصل یک اسکرولر افقی است، نه الگوی هیروی بدِ تمام‌صفحه. پایه: `overflow-x: auto`، `scroll-snap-type: x mandatory`، و `scroll-snap-align: center` روی بچه‌ها. `scrollbar-width: none` نوار را پنهان می‌کند ولی اسکرول می‌ماند.

از مجموعهٔ APIهای کروم ۱۳۵: `::scroll-button()` با جهت (`left` / `right` یا ویژگی منطقی). تا `content` چیزی غیر از `none` نباشد شبه-عنصر ساخته نمی‌شود. داخل `content` می‌شود آیکون و متن جایگزین دسترس‌پذیر گذاشت. دکمه وقتی دیگر اسکرولی در آن جهت نیست `:disabled` می‌گیرد. جایگاهشان با anchor positioning تنظیم می‌شود.

`::scroll-marker` نقطه‌های پایین کاروسل است. والد باید `scroll-marker-group` غیر از `none` داشته باشد (`before` یا `after`). مارکر فعال با `:target-current` استایل می‌گیرد. از حدود کروم ۱۴۰ می‌شود شمارندهٔ CSS را داخل متن جایگزین گذاشت تا «آیتم ۵» خوانده شود.

`scroll-target-group: auto` (کروم ۱۴۰) محدودیت شبه-عنصر را دور می‌زند: لینک‌های واقعی DOM مارکر می‌شوند و استایل کامل دارند. اسکرول‌اسپای فهرست مطالب با دو خط ممکن است: `scroll-target-group: auto` روی فهرست، و استایل `:target-current` روی لینک‌ها. گروه شبه‌عنصر semantics تب دارد؛ گروه لینک واقعی پیش‌فرضش لینک است و کنترل دست نویسنده است.

کاروسل را با scroll-driven animation و scroll state queries ترکیب می‌کنند. گالری و پیکربند CSS را به کار Adam Argyle نسبت می‌دهند.

## نکته‌ها

- دکمه، نقطه، و حالت فعال کاروسل دیگر پیش‌فرضشان کتابخانهٔ جاوااسکریپت نیست.
- اسکرول‌اسپای داخل صفحه با `scroll-target-group` و `:target-current` بدون اسکریپت درمی‌آید.
- کاروسل بد، هیروی تمام‌صفحه است؛ کاروسل به‌دردبخور، اسکرول افقی محتوایی است که در عرض جا نمی‌شود.
