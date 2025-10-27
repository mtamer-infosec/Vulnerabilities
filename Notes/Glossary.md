
## 🔑 مصطلحات عامة (General)
- Bug Bounty — برنامج صيد الثغرات — نظام يكافئ الباحثين عند الإبلاغ عن ثغرات.
- Vulnerability — ثغرة / ضعف — ضعف في النظام يمكن استغلاله.
- Exploit — استغلال — كود أو طريقة لاستغلال ثغرة.
- Payload — حمولة ضارة — البيانات أو الكود الذي ينفذ بعد الاستغلال.
- CVE (Common Vulnerabilities and Exposures) — معرف ثغرات عام — قاعدة بيانات للثغرات.
- CVSS (Common Vulnerability Scoring System) — نظام تقييم شدة الثغرة — مقياس رقمي لشدة الخطر.
- POC (Proof of Concept) — إثبات مفهوم — دليل يوضح أن الثغرة قابلة للاستغلال.
- RCE (Remote Code Execution) — تنفيذ كود عن بُعد — القدرة على تشغيل كود على الخادم الضحية.
- LPE (Local Privilege Escalation) — تصعيد امتيازات محلي — رفع صلاحيات داخل النظام.
- DoS (Denial of Service) — منع الخدمة — هجوم يوقف خدمة أو يبطئها.
- DDoS (Distributed DoS) — منع خدمة موزع — هجوم DoS من عدة مصادر.
- Disclosure — الإفصاح — نشر تفاصيل الثغرة (مسؤول/منسق أو علني).
- Responsible Disclosure — إفصاح مسؤول — إعلام المزود قبل النشر.
- Coordinated Disclosure — إفصاح منسق — تنسيق مع البائع/مزود الخدمة.
- Zero-day — يوم الصفر — ثغرة غير معروفة/بدون تصحيح.
- False Positive — إيجابي كاذب — تقرير عن مشكلة غير حقيقية.
- Impact — التأثير — مدى ضرر الثغرة (سرقة بيانات، RCE...).
- Likelihood — الاحتمالية — مدى سهولة استغلال الثغرة.
- Scope — نطاق — ما الذي يُسمح اختباره ضمن برنامج البوج.
- Out-of-scope — خارج النطاق — ما لا يجوز اختباره.

---

## 🕵️ Recon & Information Gathering
- Recon — الاستطلاع — جمع معلومات عن الهدف.
- Footprinting — بصمات — جمع بيانات ثابتة (WHOIS, DNS).
- Enumeration — تعداد — إيجاد موارد مثل صفحات، مستخدمين، خدمات.
- Subdomain — نطاق فرعي — مثال: admin.example.com.
- Subdomain Takeover — استيلاء على نطاق فرعي — وجود CNAME مؤدي إلى خدمة غير موجودة.
- DNS Harvesting — جمع سجلات DNS — العثور على سجلات A, CNAME, MX.
- OSINT (Open Source Intelligence) — استخبارات المصادر المفتوحة — البحث عبر الإنترنت.
- Shodan — محرك بحث للأجهزة المتصلة — للعثور على خدمات معرضة.
- Port Scanning — فحص المنافذ — معرفة الخدمات المفتوحة.
- Nmap — أداة فحص الشبكات — أداة مشهورة لفحص المنافذ والخدمات.
- Banner Grabbing — أخذ لافتات — قراءة معلومات الخدمة من الاستجابة.
- Directory Bruteforce — تخمين المسارات — العثور على ملفات/مجلدات مخفية.
- Wordlist — قائمة كلمات — تستخدم في التخمين والهجوم.

---

## 🌐 Web Application Vulnerabilities
- <mark style="background: #FFB86CA6;">XSS</mark> (Cross-Site Scripting) — حقن سكربت عبر الموقع — تنفيذ جافاسكربت في متصفح الضحية.
  - Stored XSS — دائم/مخزن — ينتشر من قاعدة البيانات.
  - Reflected XSS — منعكس — يظهر في استجابة مباشرة.
  - DOM XSS — عبر DOM — يحدث في جانب العميل فقط.
- <mark style="background: #FFB86CA6;">SQL Injection</mark> (SQLi) — حقن استعلامات SQL — تعديل/استخراج بيانات من قاعدة البيانات.
- CSRF (Cross-Site Request Forgery) — تزوير طلب عبر الموقع — إجبار مستخدم على تنفيذ طلب.
- SSRF (Server-Side Request Forgery) — تزوير طلب من الخادم — الخادم يطلب داخليًا مصادر أخرى.
- RFI (Remote File Inclusion) — تضمين ملف عن بُعد — تحميل كود من URL خارجي.
- LFI (Local File Inclusion) — تضمين ملفات محلية — قراءة/تنفيذ ملفات على السيرفر.
- File Upload Vulnerability — ثغرة رفع ملفات — رفع ملفات خبيثة (مث: webshell).
- Directory Traversal — اجتياز الدليل — الوصول لملفات خارج الجذر (../etc/passwd).
- Authentication Bypass — تجاوز المصادقة — الدخول بدون صلاحية.
- Insecure Direct Object Reference (<mark style="background: #FFB86CA6;">IDOR</mark>) — مرجع كائن غير آمن — الوصول لبيانات مستخدمين آخرين بتغيير ID.
- Open Redirect — إعادة توجيه مفتوحة — إعادة توجيه لمواقع ضارة.
- Clickjacking — خداع النقر — وضع صفحة في iframe لالتقاط نقرات.
- Security Misconfiguration — خطأ تكوين أمني — إعدادات غير آمنة (مثل أخطاء CORS, directory listing).
- Sensitive Data Exposure — كشف بيانات حساسة — كلمات مرور/مفاتيح بدون تشفير.
- Business Logic Flaw — خلل في منطق التطبيق — تجاوز تدفق العمل لتحقيق هدف غير مقصود.
- API Abuse — إساءة استخدام واجهة برمجة التطبيقات — استدعاءات غير مرخصة/تجاوز قيود.
- Rate Limiting — تحديد المعدل — حماية ضد هجمات القوة العنيفة.
- JWT (JSON Web Token) — توكن مصادقة — قد تتعرض للسرقة أو التزوير إذا لم تُحمى.

---

## 🔐 Authentication & Authorization
- MFA / 2FA (Multi-Factor Authentication) — تحقق متعدد العوامل — خطوة أمان إضافية.
- Brute Force — هجوم القوة العمياء — تخمين كلمات المرور.
- Credential Stuffing — حقن بيانات اعتماد مسربة — تجربة بيانات مستخدمين من تسريبات.
- Session Hijacking — اختطاف الجلسة — سرقة كوكي الجلسة.
- Session Fixation — تثبيت الجلسة — إجبار الضحية على جلسة معروفة.
- Password Spraying — رش كلمات مرور — تجربة كلمات شائعة عبر مستخدمين كثيرين.
- SSO (Single Sign-On) — تسجيل دخول موحد — سلبيات/ثغرات محتملة في المزود.
- OAuth — بروتوكول تفويض — أخطاء إعادة التوجيه أو منح صلاحيات مفرطة قد تستغل.

---

## 🧩 Cryptography & Data Protection
- Encryption — تشفير — حماية البيانات بالمفتاح.
- Hashing — هاش — تلخيص بيانات (مث: SHA256).
- Salt — سالت — قيمة إضافية قبل الهاش لزيادة الأمان.
- Key Leakage — تسرب المفتاح — خطر كبير لو حصل.
- TLS/SSL — تشفير النقل — حماية اتصال HTTPS.
- Heartbleed — مثال شهير على ثغرة في OpenSSL.

---

## 🧰 Tools & Techniques
- Burp Suite — إطار عمل اختبار اختراق ويب — للالتقاط/التعديل والتحليل.
- Burp Intruder — أداة داخل Burp لهجمات القوة/التخمين.
- Burp Repeater — إعادة إرسال وتعديل الطلبات.
- Burp Scanner — ماسح ثغرات تلقائي (في النسخة المدفوعة).
- ZAP (OWASP Zed Attack Proxy) — بديل مفتوح المصدر لـ Burp.
- Nikto — ماسح خوادم ويب قديمة/مشكلات.
- sqlmap — أداة أوتوماتيكية لاختبار SQL Injection.
- ffuf / gobuster — أدوات تخمين مسارات ونطاقات.
- Metasploit — إطار عمل استغلالات (exploits).
- nmap — ماسح شبكات ومنافذ.
- Hydra — أداة قوة عمياء لكلمات المرور.
- Wireshark — تحليل باكيتات الشبكة.

---

## 🖥️ Infrastructure & Network
- Remote Code Execution (RCE) — تنفيذ كود عن بُعد.
- Command Injection — حقن أوامر على النظام.
- Open Port — منفذ مفتوح — يعرض خدمة خارجية.
- Firewall — جدار ناري — قواعد تحمي الشبكة.
- VPN (Virtual Private Network) — شبكة خاصة افتراضية — قد يستخدم للوصول الداخلي.
- Container Escape — الهروب من الحاوية — اختراق حدود الحاويات (Docker).
- SSR (Server-Side Request Forgery) — مذكور قبلًا لكنه مهم للشبكات الداخلية.

---

## 📱 Mobile & IoT
- Insecure Storage — تخزين غير آمن — حفظ بيانات حساسة محليًا بدون تشفير.
- Reverse Engineering — الهندسة العكسية — تفكيك التطبيقات لمعرفة مفاتيح/آليات.
- APK — ملف تطبيق Android — يمكن فك ضغطه وتحليله.
- Jailbreak / Rooting — فكّ الحماية على الجهاز مما يفتح سطح هجوم أكبر.

---

## 📝 Reporting & Triaging
- Report — تقرير — وصف الثغرة، خطوات إعادة الإنتاج، التأثير، اقتراح التصحيح.
- Steps to Reproduce — خطوات إعادة الإنتاج — خطوة بخطوة لعمل الثغرة.
- Impact Assessment — تقييم التأثير — ماذا يمكن للمهاجم فعله؟
- Remediation — تصحيح — كيفية إصلاح الثغرة.
- Proof of Concept (PoC) — مذكور أعلاه.
- Severity — شدة الثغرة — عادة: Low / Medium / High / Critical.
- Confidence — مستوى الثقة — هل PoC قوي أم ضعيف؟
- Triage — تصنيف التقارير — فرز وتقييم الأولوية.

---

## ⚖️ قانوني وأخلاقي
- Authorization — تفويض — هل لديك إذن للاختبار؟
- Terms of Service (ToS) — شروط الخدمة — قد تمنع بعض الأنشطة.
- Ethical Hacking — الاختراق الأخلاقي — الالتزام بالقانون والخطوط التوجيهية.
- Bug Bounty Program Policy — قوانين البرنامج — ما يُسمح وما لا يُسمح.

---

## 📦 مصطلحات إضافية ومفيدة
- Webshell — شيل ويب — كود يسمح بالتحكم عن بُعد في خادم الويب.
- Shell — سطر أوامر — للتحكم في النظام.
- Reverse Shell — اتصال عكسي من الهدف للمهاجم.
- Bind Shell — هدف يستمع لاتصال المهاجم.
- Sandbox — بيئة معزولة — لتشغيل كود بأمان.
- Canary Token — علامة تحذيرية — ملف/رابط يُبلغ عند الوصول.
- Honeypot — فخ أمني — يتم استدراج المهاجم وتحليله.
- Enumeration — مذكور أعلاه.
- Pivoting — التحرك داخل الشبكة بعد اختراق نقطة بداية.
- Privilege Escalation — تصعيد صلاحيات — الحصول صلاحيات أعلى. 