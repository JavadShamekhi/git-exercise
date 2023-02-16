## ۱- گیت چیست و چه کاربردی دارد ؟

گیت یکی از محبوب‌ترین سیستم‌های کنترل ورژن (VSC) توزیع‌شده و متن‌باز جهان است که در سال ۲۰۰۵، لینوس توروالدز (Linus Torvalds)، خالق هسته سیستم‌عامل لینوکس، آن را ایجاد کرد. Git بیشتر برای ردیابی تغییرات فایل‌های پروژه به‌کار برده می‌شود. تعداد بسیار زیادی از پروژه‌های دنیا از سیستم گیت برای کنترل ورژن نرم‌افزارهای خود استفاده می‌کنند. همچنین، گیت روی بسیاری از سیستم‌عامل‌ها و IDEها به‌طور پیش‌فرض وجود دارد که می‌توانید از آن استفاده کنید.
گیت از بسیاری از سیستم‌های کنترل ورژن (VCS) مشابه مانند CVS و SVN و Mercurial قوی‌تر است. انجام تغییرات جدید، شاخه‌بندی، ادغام و مقایسه نسخه‌های قبلی همگی برای مدیریت پروژه شما دردسترس هستند. گیت از سیستم توزیع خوشه‌ای یا درختی استفاده می‌کند. برخلاف برخی از نرم‌افزارهای کنترل ورژن، Git هنگام ذخیره تاریخچه و نسخه‌های فایل، نام فایل‌ها را در نظر نمی‌گیرد و روی محتوای فایل متمرکز است. همچنین، مخزن گیت از ترکیب رمزگذاری دلتا برای ذخیره تفاوت‌های کد استفاده و درادامه با فشرده‌سازی، فایل‌ها را کاملاً ذخیره می‌کند.

## ۲ - دستور git init چه کاری انجام میدهد ؟

برای ایجاد مخزن جدید، از دستور git init استفاده می‌شود. git init دستوری یک‌بارمصرف است که فقط هنگام راه‌اندازی اولیه و ایجاد مخزن جدید استفاده می‌شود. اجرای این دستور پوشه‌ای جدید به نام git. در دایرکتوری فعلی شما ایجاد می‌کند.
این دستور دایرکتوری (directory) پروژه را آغاز می‌کند

## ۳ - دستور git status چه کاری انجام میدهد ؟

دستور Git Status برای نمایش وضعیت مخزن و ناحیه مرحله‌بندی استفاده می‌شود. با استفاده از این دستور، می‌توانید فایل‌های موجود در ناحیه مرحله‌بندی و فایل‌های ویرایش‌شده‌ و نیازمند به ثبت را مشاهده کنید. این دستور اطلاعاتی از Commitهای ثبت‌شده را نشان نمی‌دهد و برای نمایش وضعیت بین Git Add و Git Commit استفاده می‌شود. اگر گیت تغییرات فایل‌ها را به‌درستی ردیابی کند، پس از تغییر فایل، باید آن را در Git Status ببینیم.

## ۴ - دستور git add چه کاری انجام میدهد ؟

دستور git add فایل‌های فعلی را به ناحیه نسخه‌بندی (Staging) اضافه می‌کند (قبل از ثبت تغییرات با Commit). هربار که فایلی را در پروژه خود اضافه یا به‌روز می‌کنید، برای ثبت تغییرات، باید به‌روز‌رسانی‌ها را به قسمت Staging ارسال کنید. دستور git add را می‌توان چندین‌بار قبل از انجام Commit اجرا کرد. در‌نهایت، همه این فایل‌ها را می‌توان با یک Commit ثبت کرد. دستور add فایل‌هایی را اضافه می‌کند که در خط فرمان مشخص شده‌اند.

## ۵ - دستور git commit چه کاری انجام میدهد ؟

این دستور برای ثبت تغییرات فایل‌ها در مخزن و معمولاً بعد از git add استفاده می‌شود. هر Commit حاوی اطلاعات و پیام‌های مربوط به آن Commit است. وقتی فایلی را در Git با استفاده از دستور git add اضافه می‌کنید، در قسمت مرحله‌بندی ذخیره می‌شود. به‌عبارت‌دیگر، هر کامیت فایل‌های درون منطقه مرحله‌بندی را به مخزن گیت اضافه می‌کند.

کامیت ها مانند عکس فوری از فایل‌ها هستند که به همان صورت ذخیره می‌شوند و هیچ‌گاه تغییردادنی نیستند. هر Commit در شاخه اصلی مخزن ثبت می‌شود که می‌توانید آن‌ها را ببینید و درصورت نیاز، کدها را بازیابی کنید. هر Commit حاوی یک commit-id است. این commit-id شماره‌ای رمزنگاری شده است که الگوریتم Secure Hash Algorithm (به‌اختصار SHA) آن را ایجاد کرده است.

## ۶ - دستور git log چه کاری انجام میدهد ؟

این دستور ابزاری کاربردی برای بررسی تغییرات ایجاد‌شده در مخزن گیت است. برای مشخص‌کردن تاریخچه سورس کد، می‌توانید از این دستور استفاده کنید. به‌طور‌کلی، Git Log رکوردی از Commitهای ثبت شده است. Git log داده‌های زیر را از هر Commit به ما نشان می‌دهد:

- هش commit: متنی ۴۰کاراکتری است که الگوریتم Secure Hash Algorithm (به‌اختصار SHA) آن را تولید می‌کند و کاراکتری یونیک است.
- اطلاعات ایجاد‌کننده commit: اطلاعات کاربر ثبت‌کننده آن کامیت مانند نام و ایمیل را نشان می‌دهد.
- تاریخ commit: تاریخ ایجاد کامیت را نشان می‌دهد.
- عنوان/پیام commit: نمای کلی Commit است که در پیام Commit ثبت شده است.
