# 🤖 AI Telegram Bot

یک ربات تلگرام هوش مصنوعی با قابلیت مدیریت کاربران، حافظه شخصی، ذخیره مکالمات و کنترل دسترسی.

---

## ✨ امکانات

### 🧠 هوش مصنوعی
- اتصال به APIهای سازگار با OpenAI
- انتخاب خودکار بهترین مدل موجود
- پشتیبانی از حافظه پویا برای کاربران
- نگهداری تاریخچه مکالمات برای پاسخ‌های هوشمندتر
- سیستم پاسخ جایگزین (Fallback) هنگام خطا

### 👥 مدیریت کاربران
- افزودن کاربران مجاز
- حذف کاربران
- مشاهده لیست کاربران
- محدودسازی دسترسی به افراد مشخص

### 📊 پنل مدیریت
- مشاهده آمار ربات
- مشاهده تعداد پیام‌ها
- بررسی وضعیت سرویس AI
- ارسال پیام همگانی (Broadcast)

### 🛡️ امنیت
- Rate Limiting ضد اسپم
- جلوگیری از Prompt Injection
- فیلتر کلیدهای حساس حافظه
- جلوگیری از ارسال پیام‌های بیش از حد طولانی
- ثبت کامل لاگ‌ها

### 💾 ذخیره‌سازی
- SQLite Database
- ذخیره اطلاعات کاربران
- ذخیره حافظه اختصاصی هر کاربر
- ذخیره تاریخچه مکالمات

---

## 📁 ساختار پروژه

Ai-Telegram-Bot/
│
├── bot.py               # هسته اصلی ربات
├── ai_handler.py        # ارتباط با مدل هوش مصنوعی
├── database.py          # مدیریت دیتابیس SQLite
├── rate_limiter.py      # جلوگیری از اسپم
├── config.py            # تنظیمات پروژه
├── requirements.txt     # وابستگی‌ها
├── installer.sh         # نصب خودکار
│
├── logs/
│   └── bot.log
│
└── data/
    └── bot_database.db
---

## 🚀 نصب

### 1. کلون پروژه

git clone https://github.com/USERNAME/Ai-Telegram-Bot.git
cd Ai-Telegram-Bot
### 2. نصب وابستگی‌ها

pip install -r requirements.txt
### 3. ایجاد فایل .env

TELEGRAM_TOKEN=YOUR_BOT_TOKEN

OPENAI_API_KEY=YOUR_API_KEY
OPENAI_BASE_URL=https://api.openai.com/v1

ADMIN_IDS=123456789

MAX_USERS=100
RATE_LIMIT_MESSAGES=20
RATE_LIMIT_SECONDS=60
### 4. اجرا

python bot.py
---

## 👨‍💻 دستورات ادمین

### افزودن کاربر

/adduser USER_ID
یا

```text
/adduser USER_ID NAME

---

### حذف کاربر

text
/removeuser USER_ID

---

### مشاهده کاربران

text
/listusers

---

### آمار ربات

text
/stats

---

### ارسال پیام همگانی

text
/broadcast متن پیام

---

## 👤 دستورات کاربران

### شروع

text
/start

### راهنما

text
/help

### آمار شخصی

text
/mystats
`

---

## 🧠 سیستم حافظه

ربات می‌تواند اطلاعات مهم کاربران را به‌صورت خودکار ذخیره کند:

- نام
- شهر
- شغل
- علایق
- اطلاعات مهم مکالمه

در مکالمات بعدی این اطلاعات برای تولید پاسخ بهتر استفاده می‌شوند.

---

## 📈 ویژگی‌های فنی

- Python 3.10+
- SQLite
- OpenAI Compatible APIs
- TeleBot
- WAL Database Mode
- Logging System
- Automatic Model Discovery
- Conversation Context Management

---

## 🛡️ مکانیزم‌های امنیتی

✔ Rate Limiting

✔ Memory Validation

✔ Protected System Keys

✔ User Whitelist

✔ Error Handling

✔ HTML Escape Protection

✔ Safe Database Operations

---

## 🔧 بهینه‌سازی‌ها

- مناسب برای VPSهای ضعیف
- مصرف کم RAM
- بهینه‌سازی SQLite با WAL
- پاکسازی خودکار داده‌های قدیمی
- محدودسازی حجم تاریخچه مکالمات

---

## 📜 License

MIT License

---

## ❤️ مشارکت

Pull Request ها و پیشنهادات شما همیشه خوش‌آمد هستند.