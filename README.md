# توسعه‌دهنده در Directam

برای استخدام، اول تجربهٔ کاری را بخوان. ریپوهای پایین نمونهٔ شخصی‌اند و جای سابقهٔ کار را نمی‌گیرند.

## تجربهٔ کاری

**Directam** — کار فعلی.

جزئیات نقش و کارهایی که آنجا انجام شده را در رزومه و مصاحبه می‌گویم. برای بازار اصفهان این بخش از پروژه‌های گیت‌هاب مهم‌تر است.

## پروژه‌ها

### [Appointment](https://github.com/Artashok11228/appointment)

`API` رزرو نوبت با `Laravel` و `Sanctum`.

رزرو داخل `DB::transaction` است. قبل از چک خالی بودن اسلات، روی ردیف سرویس `lockForUpdate` گرفته می‌شود تا دو درخواست هم‌زمان هر دو اسلات را خالی نبینند. اگر این قفل رد شود، ایندکس یکتای اسلات فعال همان تداخل را به خطای `422` تبدیل می‌کند.

- مستندات: [`docs/openapi.yaml`](https://github.com/Artashok11228/appointment/blob/main/docs/openapi.yaml)
- تست‌ها روی `GitHub Actions` اجرا می‌شوند. تست همزمانی واقعی گروه `mysql` است و روی `SQLite` رد می‌شود.

### [URL Shortener](https://github.com/Artashok11228/Url-Shortener)

کوتاه‌کنندهٔ لینک با `Laravel`: ریدایرکت عمومی، کش `Redis`، ثبت کلیک با صف، و `API` با `Sanctum`.

- مستندات: [`docs/openapi.yaml`](https://github.com/Artashok11228/Url-Shortener/blob/main/docs/openapi.yaml)
- تست‌ها روی `GitHub Actions` اجرا می‌شوند.

فرانت همین رزرو نوبت: [appointment-front-end](https://github.com/Artashok11228/appointment-front-end)
