---
title: ربات تلگرام
---


# ربات تلگرام

به کمک این آموزش، شما می‌توانید ربات تلگرام مرزبان را راه‌اندازی کنید تا علاوه بر پنل مرزبان از طریق ربات تلگرام نیز بتوانید کاربرهای خود را مدیریت کنید. برخی از قابلیت‌های ربات تلگرام شامل موارد زیر می‌شوند.

- آمار پنل با جزئیات بیشتر، مانند میزان دانلود و آپلود، سرعت لحظه‌ای دانلود و آپلود
- امکان ایجاد تغییر روی همه کاربرها مانند اضافه یا کم کردن تعداد روز‌ها یا حجم تعیین شده
- حذف کردن همه کاربرهای منقضی شده یا کاربرهایی که حجم آن‌ها به پایان رسیده
- برداشتن تیک اینباند به خصوص یا گذاشتن تیک آن برای همه کاربرها
- ساخت کاربر از طریق قالب از پیش تعیین شده
- ریستارت کردن Xray

## راه‌اندازی ربات تلگرام

1. شما باید یک ربات از طریق https://t.me/BotFather  بسازید و توکن ربات را کپی کنید تا در مرحله بعد از آن استفاده کنید.

2. از آنجایی که دسترسی به این ربات تنها برای شما یا لیست محدودی از مدیران در دسترس خواهد بود، باید شناسه تلگرام افرادی که مجاز به استفاده از آن هستند را مشخص کنید. برای دریافت شناسه تلگرام خود به این ربات https://t.me/userinfobot رجوع کنید. 
<br>

::: tip  نکته 
اگر قصد دارید که لاگ‌های پنل جدا باشد یک کانال ایجاد کنید در آن یک متن بفرستید و متن را برای همان رباتی که در مرحله دوم گفته شده فوروارد کنید تا آیدی کانال را دریافت کنید، برای اینکه لاگ‌ها به کانال فرستاده بشه ربات تلگرام باید عضو کانال و ادمین باشد.
:::

<br>
3. اکنون باید تمام متغیرها را در مرزبان مشخص کنید، برای این کار باید متغیرها را در فایل .env با برداشتن کامنت # اول آن‌ها و گذاشتن مقادیر خواسته شده در فایل تنظیم کنید.


| متغیرها                    |  معنی  |
|----------------:|-----------:|
| `TELEGRAM_API_TOKEN`           | توکن ربات تلگرام|       
| `TELEGRAM_ADMIN_ID`|آیدی عددی ادمین در تلگرام (اگر نیاز به دسترسی چند ادمین به ربات دارید، آیدی آن‌ها را مشخص کرده و با کاما از هم جدا کنید.)|
| `TELEGRAM_LOGGER_CHANNEL_ID` | آیدی عددی کانال برای لاگ‌های پنل در صورت تمایل        |  
| `TELGRAM_DEFAULT_VLESS_FLOW`  | تعیین Flow پیش‌فرض برای پروتکل Vless در ربات تلگرام  |    
| `TELEGRAM_PROXY_URL`       | اجرای ربات از طریق پروکسی (در صورتی که در سرور شما سرورهای تلگرام مسدود شده‌اند.) |

<br>

4. پس از قرار دادن مقدار‌های خواسته شده، با دستور زیر مرزبان را ریستارت کنید تا تغییرات اعمال شود.

  ```bash
  marzban restart
  ```

  در نهایت پس از ریستارت کردن مرزبان رباتی که پیش‌تر ساخته بودید با وارد کردن دستور start در دسترس شما خواهد بود.