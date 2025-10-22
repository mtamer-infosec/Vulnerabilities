# 🐛 Bug Bounty Terminology Dictionary

## 📡 Reconnaissance & Information Gathering

| English Term              | Arabic Explanation                      |
| ------------------------- | --------------------------------------- |
| **Reconnaissance**        | عملية جمع المعلومات والاستكشاف عن الهدف |
| **Subdomain Enumeration** | اكتشاف كافة النطاقات الفرعية للموقع     |
| **Port Scanning**         | فحص المنافذ المفتوحة على الخادم         |
| **OSINT**                 | جمع المعلومات من مصادر مفتوحة           |
| **Fingerprinting**        | تحديد التقنيات المستخدمة في التطبيق     |
| **Attack Surface**        | المساحة المتاحة للهجوم على النظام       |
| **Endpoint Discovery**    | اكتشاف كافة نقاط الوصول في التطبيق      |
| **Parameter Fuzzing**     | اختبار بارامترات المدخلات بشكل عشوائي   |
************
## 🎯 Common Vulnerabilities

| English Term | Arabic Explanation |
|-------------|-------------------|
| **XSS (Cross-Site Scripting)** | ثغرة تنفيذ شفرات برمجية عبر المواقع |
| **SQL Injection** | ثغرة حقن أوامر قواعد البيانات |
| **CSRF (Cross-Site Request Forgery)** | تزوير الطلبات عبر المواقع |
| **SSRF (Server-Side Request Forgery)** | تزوير الطلبات من جانب الخادم |
| **IDOR (Insecure Direct Object Reference)** | الوصول غير الآمن للمراجع المباشرة |
| **RCE (Remote Code Execution)** | تنفيذ أوامر عن بُعد على الخادم |
| **LFI/RFI** | ثغرة تضمين ملفات محلية/عن بُعد |
| **XXE (XML External Entity)** | ثغرة كيانات XML الخارجية |
| **Business Logic Flaw** | ثغرة في المنطق التشغيلي للتطبيق |

## ⚡ Exploitation Techniques

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Payload** | الشفرة أو البيانات المستخدمة لاستغلال الثغرة |
| **Proof of Concept (PoC)** | دليل عملي يثبت وجود وإمكانية استغلال الثغرة |
| **Exploitation** | عملية استغلال الثغرة فعلياً |
| **Privilege Escalation** | تصعيد الصلاحيات للوصول لمستويات أعلى |
| **Lateral Movement** | الانتقال الأفقي بين الأنظمة والخوادم |
| **Persistence** | آليات الحفاظ على الوصول للنظام |
| **Bypass** | تجاوز آليات الحماية والأمان |
| **Reverse Shell** | إنشاء اتصال عكسي للتحكم بالخادم |
| **Bind Shell** | فتح منفذ للاتصال المباشر بالخادم |

## 🔧 Testing & Methodology

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Manual Testing** | الاختبار اليدوي دون الاعتماد على الأدوات فقط |
| **Automated Scanning** | المسح الآلي لاكتشاف الثغرات |
| **Black-box Testing** | الاختبار دون معرفة مسبقة بالنظام |
| **White-box Testing** | الاختبار مع معرفة كاملة بكود التطبيق |
| **Gray-box Testing** | الاختبار بمعرفة جزئية عن النظام |
| **Penetration Testing** | اختبار الاختراق المحاكي للهجمات الحقيقية |
| **Vulnerability Assessment** | تقييم الثغرات وتحديد مستويات الخطورة |
| **Threat Modeling** | نمذجة التهديدات المحتملة للنظام |

## 📊 Severity & Impact

| English Term | Arabic Explanation |
|-------------|-------------------|
| **CVSS Score** | مقياس تقييم خطورة الثغرة عالمياً |
| **Critical** | مستوى خطورة حرج (أعلى مستوى) |
| **High** | مستوى خطورة عالي |
| **Medium** | مستوى خطورة متوسط |
| **Low** | مستوى خطورة منخفض |
| **Informational** | معلوماتية دون تأثير أمني |
| **Impact** | التأثير الناتج عن استغلال الثغرة |
| **Attack Vector** | المسار أو الوسيلة المستخدمة في الهجوم |
| **Attack Complexity** | مستوى تعقيد الهجوم المطلوب |

## 📝 Reporting & Communication

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Bug Report** | تقرير مفصل عن الثغرة المكتشفة |
| **Vulnerability Disclosure** | الإفصاح المسؤول عن الثغرة |
| **Triaging** | عملية فرز وتصنيف البلاغات |
| **Duplicate** | بلاغ مكرر لثغرة تم الإبلاغ عنها مسبقاً |
| **Bounty** | المكافأة المالية لاكتشاف الثغرة |
| **Scope** | النطاق المسموح اختباره في البرنامج |
| **Out of Scope** | خارج النطاق المسموح به للاختبار |
| **Reproduction Steps** | خطوات إعادة إنتاج الثغرة |
| **Remediation** | الإصلاحات والعلاجات المطلوبة |

## 🛠️ Tools & Technologies

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Burp Suite** | مجموعة أدوات لاختبار تطبيقات الويب |
| **sqlmap** | أداة مفتوحة المصدر لاكتشاف ثغرات SQL Injection |
| **Nmap** | أداة لفحص الشبكات واكتشاف الخدمات |
| **Metasploit** | إطار عمل لاختبار الاختراق |
| **OWASP** | مشروع الأمان المفتوح لتطبيقات الويب |
| **WAF** | جدار حماية لتطبيقات الويب |
| **Proxy** | وسيط لاعتراض وتحليل حركة المرور |
| **Encoder/Decoder** | أدوات التشفير وفك التشفير |

## 🔄 Advanced Concepts

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Zero-day** | ثغرة غير معروفة للمطورين ولا توجد تصحيحات لها |
| **Patch** | التصحيح الأمني للثغرة |
| **CVE** | الفهرس العالمي للثغرات والتعرضات |
| **Attack Chain** | سلسلة الهجوم المتتابعة لتحقيق الهدف |
| **Post-exploitation** | المراحل بعد تحقيق الاختراق الناجح |
| **Lateral Movement** | الانتقال الأفقي داخل الشبكة |
| **Pivoting** | استخدام نظام مخترق للوصول لأنظمة أخرى |
| **Red Team** | فريق المحاكاة الهجومية |
| **Blue Team** | فريق الدفاع والأمان |

## 🌐 Web Technologies

| English Term | Arabic Explanation |
|-------------|-------------------|
| **API** | واجهة برمجة التطبيقات |
| **REST** | نمط معماري لخدمات الويب |
| **GraphQL** | لغة استعلام للواجهات البرمجية |
| **JWT** | رمز الويب المصدَّق |
| **CORS** | مشاركة الموارد بين المصادر المختلفة |
| **HTTP Headers** | رؤوس بروتوكول HTTP |
| **Cookies** | بيانات تخزين على متصفح المستخدم |
| **Session** | جلسة المستخدم على التطبيق |

## ⚠️ Security Mechanisms

| English Term | Arabic Explanation |
|-------------|-------------------|
| **Input Validation** | التحقق من صحة وسلامة البيانات المدخلة |
| **Output Encoding** | تشفير المخرجات لمنع هجمات الحقن |
| **Authentication** | عملية التحقق من هوية المستخدم |
| **Authorization** | تحديد الصلاحيات والوصول |
| **Encryption** | تشفير البيانات لحمايتها |
| **Hashing** | تحويل البيانات إلى قيمة فريدة |
| **Salting** | إضافة قيم عشوائية لكلمات المرور قبل تشفيرها |
| **Rate Limiting** | تحديد معدل الطلبات المسموح بها |

---
