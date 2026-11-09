<div align="center">

# ARAL URANIUM · V1.1 — REACTOR DECK · URANIUM EDITION

**نسل تازهٔ پنل آزاد و رایگانِ مدیریت اشتراک VLESS، Trojan و Shadowsocks و پروکسی رسمی تلگرام روی شبکهٔ ابری کلادفلر — با طراحی کاملاً بازنویسی‌شدهٔ Uranium**
*The brand-new generation of the free serverless VLESS, Trojan & Shadowsocks panel on Cloudflare Workers & Pages — fully redesigned Uranium edition*

![Version](https://img.shields.io/badge/Version-1.1.0_URANIUM-00ff9d?style=flat-square) ![Runtime](https://img.shields.io/badge/Cloudflare-Workers%20%26%20Pages-050807?style=flat-square) ![Theme](https://img.shields.io/badge/Theme-Uranium%20Reactor%20Deck-00b36f?style=flat-square)

[کانال رسمی / Official Channel — Telegram](https://t.me/AralDev)

</div>

---

> ### اطلاعیه (رایگان و غیرقابل فروش)
> **ARAL URANIUM** نرم‌افزار آزاد و رایگان است؛ خرید و فروش سورس، پنل یا لینک اشتراکِ ساخته‌شده با آن مجاز نیست.
> **ARAL URANIUM is free software — strictly not for sale.**

---

## URANIUM چیست؟ / What is Uranium?

**ARAL URANIUM** بازطراحی کامل نسل قبلی پنل‌های ARAL است — همان هستهٔ اثبات‌شدهٔ تونل و مدیریت اشتراک، در یک بدنهٔ تازه:

- **دیزاین جدید Reactor Deck** — زبان بصری Aral CF: پس‌زمینهٔ شطرنجی متحرک، شبکهٔ اورانیومی، خطوط اسکن و رادار چرخان؛ کارت‌های شیشه‌ای با گوشه‌های بریده، تایپوگرافی Orbitron + Vazirmatn + JetBrains Mono، افکت گلیچ روی واترمارک و پری‌لودر بوت.
- **چیدمان sidel بیو (Sidebar Deck)** — پنل مدیریت با نوار کناری شماره‌گذاری‌شده (۰۱ تا ۰۶)، آمار زندهٔ سیستم، و کلیدهای عملیات؛ همه‌چیز سر جای درست خودش، بدون پراکندگی.
- **صحنهٔ تعاملی قلهٔ آرال** — به‌جای تصویر ثابت، پایین صفحهٔ ورود و کارت مشترک، یک صحنهٔ پیکسل‌آرت زنده از قلهٔ آرال در شبِ اورانیومی رندر می‌شود: ماه، ستاره‌ها، ابرهای متحرک، پرچم قله و کلمهٔ «Aral» حک‌شده روی کوه — با موس تکانش بده و روی قله کلیک کن تا باد برف را بلند کند.
- **موتور تله‌متری اورانیومی** — نمودار زندهٔ سرعت/پینگ با ردِّ سبز اورانیوم و خط‌چین نارنجی RTT.
- **نماد اتم اورانیوم** — آیکن و PWA تازه با مدارِ سبزِ درخشان.

*Uranium is a full redesign: the same battle-tested tunnel & subscription core, wrapped in the Aral CF design language — glass panels, cut corners, uranium-green glow on near-black, glitch wordmark, radar sweep — plus a numbered sidebar deck layout and a live interactive pixel-art summit scene instead of a static image.*

## ویژگی‌ها / Features

### هستهٔ تونل / Core
- **VLESS + Trojan + Shadowsocks روی WebSocket** — سه پروتکل همزمان؛ رمز ss به‌صورت خودکار از UUID ساخته می‌شود
  *VLESS + Trojan + Shadowsocks over WS — all three protocols, ss secrets auto-derived from the UUID*
- **Fragment (۱-۱ / tlshello) + Pattern JSON (fm) + Cipher Suites (cs) + TLS Mask** ضد DPI
  *Anti-DPI: fragment + advanced pattern JSON + custom cipher suites + TLS masking*
- **ECH (Encrypted Client Hello)** — سازندهٔ ترکیب‌های `dom+udp/tcp/https://dns`
  *ECH combo builder (UDP / TCP / DoH)*
- **اثر انگشت TLS** به انتخاب: chrome, firefox, safari, ios, android, edge, 360, qq, random, randomized, unsafe
  *Selectable uTLS fingerprint per subscriber*
- **ProxyIP · NAT64 · زنجیرهٔ SOCKS5/HTTP/SOCKS4** برای رفع بلاک و خروج چندلایه
  *ProxyIP, NAT64 and multi-hop chain proxy fallbacks*

### قابلیت‌های مدیریتی / Panel Features
- **لوکیشن‌های خروجی چندگانه (تا ۱۵ لوکیشن)** برای هر مشترک — هر لوکیشن یک مسیر `/loc-N` و یک گروه مستقل در اشتراک با پرچم کشور
  *Up to 15 per-user exit locations, each a `/loc-N` node group with country flags*
- **تعویض خودکار پروکسی خراب** از مخازن داده، با حفظ کشورِ همان لوکیشن
  *Broken-exit auto-replacement from data pools, country-preserving*
- **چرخش خودکار IP تمیز** برای هر مشترک (ترکیب IPv4/IPv6/دامنه، تعداد قابل تنظیم، هر بار دریافت اشتراک تازه می‌شود)
  *Per-user clean-IP auto-rotation (mixed v4/v6/domains) on every subscription fetch*
- **سهمیهٔ تعداد اتصال (Request Quota) و حد دستگاه همزمان (IP Limit)** — با اعمال واقعی روی خط
  *Request quota + concurrent-device limits — actually enforced on the tunnel*
- **ریست خودکار حجم/سهمیه هر N روز** و **شروع اعتبار از اولین اتصال**
  *Auto-reset schedules and start-on-first-connect*
- **مسدودسازی بزرگسال/تبلیغات** به‌ازای هر مشترک با DoH خانواده + تشخیص غیرفعالِ SNI (fail-open)
  *Per-user adult/ads blocking via family DoH + passive SNI sniffing (fail-open)*
- **عملیات گروهی**: انتخاب چندتایی، فعال/غیرفعال‌سازی، ریست حجم/سهمیه/زمان و حذف گروهی
  *Bulk operations: multi-select enable/disable/reset/delete*
- **مخازن داده (Pools)**: IP تمیز و پروکسی عمومی — آپلود مستقیم در KV یا دریافت خودکار از مخزن GitHub خودتان
  *Data pools: paste into KV or auto-fetch from your own GitHub repo (`data/` folder)*
- **دریافت کامل مخزن داده** — «دریافت کامل از گیت‌هاب» هر چهار فایل مخزن را مستقیم می‌خواند و **همهٔ موارد معتبر** را (تا سقف هر مخزن) در KV ذخیره می‌کند؛ با «بارگذاری کل مخزن» فهرست کامل در ویرایشگر باز می‌شود و ذخیرهٔ ناگهانیِ مخزن بزرگ با متن کوچک، هشدار تأیید می‌گیرد
  *Full repository fetch — pulls all four repo files directly and persists every valid entry (up to each pool cap); “load full pool” opens the complete list in the editor and shrink-on-save is confirmation-guarded*
- **انتخابگر آی‌پی تمیز در فرم مشترک** — نوع آدرس (IPv4 / IPv6 / دامنه / ترکیبی) و تعداد را مشخص کنید؛ کل مخزن ذخیره‌شده اسکن و همان تعداد برای مشترک انتخاب و درج می‌شود (موجودی هر مخزن هم نمایش داده می‌شود)
  *Clean-IP picker in the subscriber form — choose type & count; the entire saved repository is scanned and the requested number of addresses is inserted (live per-pool availability readout)*
- **هشدار عبور از ۲۰۰ کانفیگ** — شمارندهٔ زندهٔ تعداد کانفیگ هر مشترک (فرمول: آدرس‌ها × پورت‌ها × پروتکل‌ها × (لوکیشن‌ها + ۱)) داخل فرم؛ هنگام ذخیره اگر از ۲۰۰ بگذرد، هشدار «ادامه می‌دهم / بازگشت و کاهش» نمایش داده می‌شود و در کارت هر مشترک، چیپ تعداد کانفیگ با حالت هشدار دیده می‌شود
  *>200-config warning — live per-subscriber config counter inside the form; saving above the 200-node cap triggers a continue-or-reduce warning and every subscriber card shows a config-count chip*
- **ثابت‌کردن آی‌پی کانفیگ (قفل آی‌پی)** — برای هر مشترک می‌توانید آی‌پی‌های کانفیگ را قفل کنید: چرخش خودکار کامل خاموش می‌شود و فهرست آی‌پی‌ها همیشه ثابت می‌ماند؛ با فعال‌سازی قفل روی فهرست خالی، پیش‌فرض پنل به‌صورت خودکار ثبت می‌شود و در کارت مشترک «ثابت (قفل‌شده)» دیده می‌شود
  *Fixed/pinned config IPs per subscriber — IP lock fully disables rotation and freezes the list (auto-snapshotted from panel defaults when empty); the subscriber card shows “FIXED (LOCKED)”*
- **پیش‌تنظیم‌های اپراتوری ایران**: همراه اول، ایرانسل، رایتل، مخابرات و گیمینگ — یک‌ضرب روی هر مشترک
  *Iranian ISP fragmentation presets (MCI / Irancell / Rightel / TCI / Gaming) per subscriber*
- **بات مدیریتی تلگرام** — توکن بات + آیدی عددی ادمین را در پنل ثبت کنید؛ وبهوک خودکار ست می‌شود. `/start` منوی «مشترکین» و «پنل» را می‌دهد و با انتخاب هر مشترک، QR پنل + همهٔ لینک‌های اشتراک + نودهای اصلی در تلگرام ارسال می‌شود.
  *Telegram management bot — paste a BotFather token + numeric admin ID; the webhook is set automatically and every subscriber's QR & links are one tap away.*
- **آی‌پی تمیزِ آماده از مخزن رسمی** — در اولین اجرا، IP تمیز/دامنه/پروکسی از پوشهٔ `data/` مخزن رسمی بارگذاری می‌شود
  *Clean-IPs ready by default — official repo data pools auto-load on first boot*
- **اعمال قوانین در میانهٔ اتصال (Heartbeat)** — اتمام حجم/سهمیه، انقضا، توقف یا حذف، تونلِ زنده را بلافاصله قطع می‌کند
  *Mid-connection enforcement heartbeat: quota/expiry/pause/deletion kills live tunnels instantly*
- **حسابداری عمر و مشترکین حذف‌شده** — مصرفِ کلِّ عمر هر مشترک هرگز ریست نمی‌شود و با حذف مشترک به حساب سرور منتقل می‌شود
  *Lifetime (never-reset) per-user accounting + deleted-subscriber traffic preserved in server totals*
- **پورت‌های اختصاصی هر مشترک**، **نوع مخزن چرخش** و **زمان‌بندی جداگانهٔ ریست سهمیهٔ اتصال**
  *Per-user port overrides, rotation pool type, independent request-quota reset schedule*
- **پرکردن هوشمند لوکیشن‌ها** — نمونه‌گیری از مخزن پروکسی، آزمودن زنده و انتخاب ۵ خروجی سالم با کم‌ترین پینگ
  *Smart location fill: sample the proxy pool, live-probe, auto-fill the 5 healthiest exits*
- **بروزرسانی خودکار هسته** (اختیاری، هر ۵ دقیقه) + **ری‌استارت هسته** + **بازیابی رمز با توکن کلادفلر**
  *Optional core auto-update, restart-core, Cloudflare-token password recovery*

### پنل و اشتراک / Panel & Subscriptions
- **اشتراک هوشمند چندقالبی** — Base64، Xray JSON، Sing-box، Clash/Mihomo + صفحهٔ «کارت مشترک» زنده با نوارهای مصرف/اعتبار/سهمیه، QR و صحنهٔ قلهٔ آرال
  *Multi-format subscriptions + live status page with progress bars, QR and the summit scene*
- **پروکسی رسمی تلگرام** (`tg://webproxy`) بدون برنامهٔ جانبی + **DoH خصوصی** برای هر مشترک
  *Official Telegram Web Proxy + per-subscriber Private DoH*
- **نوسان‌نگار زنده** پینگ/سرعت، اسکنر IP تمیز با رنج‌های رسمی کلادفلر و مشاور هوشمند ISP
  *Live RTT/speed telemetry, clean-IP scanner with official CF ranges, smart ISP advisor*
- **PWA** — نصب‌شدن به‌عنوان اپلیکیشن روی موبایل و دسکتاپ
  *Installable Progressive Web App*
- **تم Uranium Reactor Deck** با حالت دارک/لایت، دوزبانه (فارسی/انگلیسی) و بدون هیچ لوگوی تصویری
  *Uranium Reactor Deck theme, dark/light, bilingual FA/EN — logo-free (wordmark only)*
- **پشتیبان‌گیری/بازیابی JSON**، مانیتور سهمیهٔ روزانهٔ کلادفلر و **بروزرسانی هسته از گیت‌هاب**
  *JSON backup/restore, CF daily-quota monitor, GitHub core self-updater*
- **امنیت**: PBKDF2-SHA256، نشست امضاشدهٔ HMAC، محدودسازی تلاش ناموفق ورود
  *PBKDF2-HMAC sessions, login throttling*

## تایپوگرافی و هویت / Typography & Identity

| نقش | فونت |
| --- | --- |
| واترمارک و اعداد / Display | **Orbitron** (variable) |
| فارسی / Farsi | **Vazirmatn** |
| کد و اعداد فنی / Mono | **JetBrains Mono** |

نسخهٔ URANIUM عمداً **بدون لوگو** منتشر می‌شود؛ هویت فقط با واترمارک متنی `Aral Uranium` در نام نودها و سربرگ پنل حفظ می‌شود.
*The URANIUM edition is deliberately logo-free — the `Aral Uranium` text watermark lives in the masthead and node remarks.*

## استقرار سریع — Workers / Quick Deploy (Workers)

1. در کلادفلر یک **KV namespace** با نام `aral` بساز.
2. یک Worker جدید بساز (Hello World) و کل محتوای `worker-single-file.js` را در **Edit code** جای‌گذاری و **Deploy** کن.
3. از **Settings → Bindings → KV namespace** متغیر `KV` را به فضای `aral` وصل کن.
4. صفحهٔ پنل را باز کن — فرم انتخاب رمز مدیر ظاهر می‌شود.

*Full English steps are rendered inside the panel itself (stateless view).*

## استقرار — Pages / Deploy (Pages)

پوشهٔ `dist/` (شامل `index.html` و `_worker.js`) یا بستهٔ آمادهٔ `aral-uranium-pages.zip` را در **Workers & Pages → Create → Pages → Upload assets** آپلود کن.

*Upload `dist/` or the ready-made `aral-uranium-pages.zip` via Workers & Pages → Create → Pages → Upload assets.*

## توسعهٔ محلی / Local Development

```bash
npm install          # نصب وابستگی‌ها / install dependencies
npm run build        # ساخت worker-single-file.js + panel-preview.html + dist/
npm run dev          # اجرای محلی با wrangler
npm test             # تست E2E با playwright (18/18)
node shot-verify.mjs # اسکرین‌شات بصری همهٔ نماها / visual screenshots
```

## مخازن داده / Data Pools

پوشهٔ `data/` شامل فهرست‌های عمومیِ IP تمیز و پروکسی‌های خروجی است. برای فعال‌سازی چرخش IP و لوکیشن‌های آماده، متن فایل‌ها را در پنل (`شبکه و ضد فیلتر → مخازن داده`) ذخیره کن یا این پوشه را در یک ریپوی GitHub خودت منتشر و در پنل `owner/repo` را ثبت کن. جزئیات: `data/README.md`.

*The bundled `data/` folder feeds clean-IP rotation and exit locations — upload it via the panel or point the panel at your own GitHub repo.*

## اسکریپت‌های جانبی / Side Scripts

- `aral-relay.sh` — نصب‌کنندهٔ ریلی SOCKS5 (GOST + systemd) برای سرور شخصی؛ خروجی را مستقیم در «لوکیشن‌های خروجی» مشترک بگذار.
  *SOCKS5 relay builder for your own VPS — paste the output as a subscriber location.*
- `aral-scanner.txt` — اسکنر چندگانه (مرورگر/پایتون/پاورشل) برای یافتن IP تمیز با SNI دامنهٔ خودت.
  *Polyglot SNI clean-IP scanner (browser / Python / PowerShell).*

## بروزرسانی هسته / Core Self-Updater

پنل به‌صورت پیش‌فرض نسخهٔ جدید را از مخزن رسمی `Aral-Dev/Aral-Uranium` بررسی و نصب می‌کند. اگر مخزن شخصی خودت را می‌خواهی، ثابت‌های `GITHUB_REPO` را در `src/storage.js` و `OFFICIAL_GITHUB_REPO` را در `src/ui/app.js` تغییر بده.

*The updater checks the official `Aral-Dev/Aral-Uranium` repo — point those two constants at your own fork if needed.*

## ساختار مخزن / Repository Layout

```
├─ build.mjs               # پایپ‌لاین ساخت (فونت‌سابی، فشرده‌سازی، استلث، ممیزی امضا)
├─ worker-single-file.js   # خروجی نهایی برای Workers
├─ aral-uranium-pages.zip  # بستهٔ آمادهٔ Pages
├─ wrangler.toml / config.json
├─ aral-relay.sh           # نصب‌کنندهٔ ریلی SOCKS5
├─ aral-scanner.txt        # اسکنر چندگانهٔ SNI
├─ data/                   # مخازن داده (IP تمیز، دامنه، پروکسی‌های عمومی، ECH)
├─ src/
│  ├─ worker.js            # ورودی Worker (API + مسیریابی + PWA)
│  ├─ sub.js               # مولد اشتراک و کارت مشترک (لوکیشن‌ها، fm/cs/mask/ECH)
│  ├─ protocols.js         # موتور تونل VLESS/Trojan/ss + سهمیه‌ها + DoH
│  ├─ sslib.js             # موتور Shadowsocks AEAD + اسنiffer و مسدودساز
│  ├─ pools.js / poolutil.js # لایهٔ مخازن داده
│  ├─ tgproxy.js           # پروکسی رسمی تلگرام
│  ├─ tgbot.js             # بات مدیریتی تلگرام
│  ├─ storage.js           # لایهٔ KV و ثابت‌های برند
│  ├─ crypto.js            # توابع رمزنگاری
│  └─ ui/                  # رابط کاربری (HTML/CSS/JS + فونت‌ها + صحنهٔ قله)
└─ assets/                 # فونت‌های ساب‌ست‌شده (کش ساخت)
```

---

<div align="center">

**ARAL URANIUM** — راکتور آزادِ اشتراک روی کلادفلر · `t.me/AralDev`

*Made with ⚛ & ☕ — 100% free, forever.*

</div>
