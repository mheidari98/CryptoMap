---
title: Cryptography Mindmap
markmap:
  colorFreezeLevel: 3
  initialExpandLevel: 3
---

##  <div dir="rtl" align="right"><span title=" رمزنگاری کلاسیک نوعی رمزنگاری است که در گذشته مورد استفاده قرار می‌گرفت، شاید بتوان به لحاظ تاریخی گفت که الگوریتم‌های کلاسیک معمولا به رمزنگاری‌های تا جنگ حهانی دوم می‌گویند. اکنون بیشتر مواقع از این الگوریتم‌ها برای درک بهتر مبانی و اصول اولیه رمزنگاری استفاده می‌شود. برخلاف الگوریتم‌های رمزنگاری مدرن، اکثر رمزگذارهای کلاسیک می‌توانند دستی محاسبه و حل شوند.">  **Classical Cryptography**</span></div>

###  <div dir="rtl" align="right"><span title="این نوع از الگوریتم‌های کلاسیک با جابجایی  یا بهم ریختن ترتیب حروف یا گروهی از حرف‌های الفبا موجود در متن، آن را رمز می‌کند."> **Permutation Ciphers**</span></div>

  - <div dir="rtl" align="right"><span title=" یک روش باستانی رمزنگاری که در آن با استفاده از یک ابزار استوانه‌ای شکل (مانند خودکار امروزی)،  با یک نوار پوستی که دور آن پیچیده شده، پیام روی نوار نوشته می‌شود. این کار باعث می‌شود که بعد از باز کردن نوار از دور استوانه حروف جابه‌جا (رمزی) روی آن نوشته شده باشند.">Scytale</span></div>
  
  - <div dir="rtl" align="right"><span title="در این الگوریتم، حروف متن به صورت زیگزاگ روی دو یا چندین سطر نوشته می‌شوند و سپس سطرها به ترتیب نوشته می‌شوند تا متن رمز بدست آید. ">Rail Fence </span></div>
  
 - <div dir="rtl" align="right"><span title="در این سیستم رمزنگاری ابتدا متن اصلی را در ردیف‌هایی به طول معین قرار می‌دهیم سپس جدول به دست آمده را به صورت ستونی اما به صورت درهم ریخته می‌خوانیم.">Columnar Transposition</span></div>

  - <div dir="rtl" align="right"><span title="این سیستم در سال 1902 توسط مایژوفسکی پیشنهاد شد. این  رمزنگاری مشابه جابه‌جایی ستونی است با این تفاوت که کلید در رمز جابه‌جایی ستونی در صورتی که حروف تکراری داشته باشد از سمت چپ کوچکترین عدد اختصاص داده می‌شود در حالی که در این سیستم به حروف یکسان عدد یکسانی داده می‌شود و هنگامی که می‌خواهیم متن رمز شده را تشکیل دهیم، ستون‌های به عدد یکسان را به صورت ردیفی می‌خوانیم ">Myszkowski</span></div>

### <div dir="rtl" align="right"><span title="در این روش، هر حرف داخل متن را با حرف متفاوت دیگر یا یک نماد خاص، اغلب براساس یک اصول معین و ثابت جایگزین می‌شود. گرچه این روش قبلا به شکل تجربی استفاده می‌شد، اما اولین بار این روش توسط یک دانشمند عرب به نام «ابن الدريهم» در قرن 14 میلادی به شکل علمی در یک رساله تشریح و مطرح شده است ">**Substitution Ciphers**</span></div>

  - <div dir="rtl" align="right"><span title="روش تک‌الفبایی، نوعی رمز جانشینی است که در آن هر حرف از متن پیام تنها با یک حرف متناظر، جایگزین می‌شود. این جانشنینی ممکن است در کل متن پیام با یک الگو ثابت یا یک کلید از قبل تعریف شده تعیین شود.">Monoalphabetic</span></div>
  
    - <div dir="rtl" align="right"><span title="در این الگوریتم رمزنگاری باستانی، هر حرف در متن آشکار با حرف دیگری با فاصله‌ای ثابت در الفبا جایگزین می‌شود؛ به این فاصلهٔ ثابت «مقدار انتقال» گفته می‌شود. برای مثال اگر مقدار انتقال برابر ۳ انتخاب شود و رمزنگاری روی متن با الفبای انگلیسی انجام شود، حرف D به جای حرف A می‌نشیند.">Caesar</span></div>

    - <div dir="rtl" align="right"><span title="اولین رمزنگاری جانشینی دوتایی است که طرح آن اولین بار در سال 1854 توسط چارلز ویت‌استون اختراع شد ولی به دلیل ارتقای آن توسط لرد پلی‌فیر، نام آن رمز پلی‌فر است.این روش، از یک جدول &#x202B;5x5&#x202C; از حروف برای رمزگذاری استفاده می‌کند."> Playfair</span></div>

    - <div dir="rtl" align="right"><span title=" یک روش ساده جانشینی است که در آن برای رمز کردن پیام حروف الفبا متن به شکل معکوس (حرف اول با آخر) جایگزین می‌شوند.">Atbash </span></div>


  - <div dir="rtl" align="right"><span title="نوعی رمز جانشینی که از چندین الفبای جایگزین برای رمزگذاری پیام استفاده می‌کند. این سیستم جایگزینی حروف را در نقاط مختلف متن تغییر می دهد و آن را در برابر تحلیل فراوانی مقاوم‌تر می کند. یک دانشمند عرب مصری به نام «ابوالعباس قلقشندی» قرن 14 میلادی در کتابی به نام «صبح الأعشى» در مورد این روش بحث کرده است. اما گمان می‌رود که شاید الکندی، دیگر دانشمند عرب مبدع، این نوع از رمزنگاری باشد.">Polyalphabetic</span></div>

    - <div dir="rtl" align="right"><span title="این روش از یک کلمه یا عبارت به عنوان  کلید و یک جدول ۲۶×۲۶  (تعداد حروف انگلیسی) برای تعیین جانشینی هر حرف استفاده می‌کند. این روش از یک حروف الفبای جایگزینی متفاوت در هر موقعیت استفاده می‌کند که شکستن آن را سخت‌تر می‌کند. این رمز، یک روش متداول و مؤثر برای مخفی‌سازی اطلاعات به‌ویژه در قرون ۱۵ تا ۱۹ میلادی بود.">Vigenère</span></div>

    - <div dir="rtl" align="right"><span title="ایجاد شده توسط فرانسیس بوفور، رمز جایگزینی مشابه رمز Vigenère که به شکل جدولی و با کمی تغییر کار می‌کند. معروف‌ترین کاربرد این روش رمزنگاری در یک ماشین رمزگذاری مبتنی بر چرخانه (rotor)، مانند ماشین Hagelin M-209 بود.">Beaufort</span></div>

    - <div dir="rtl" align="right"><span title="این الگوریتم جز رمزنگاری‌های Polygraphic است که در آن حروف پیام را به شکل بلوکی از حروف با استفاده از ضرب ماتریس‌ها و یک ماتریس کلید رمزگذاری می‌کند. در سال ۱۹۲۹ توسط لسترهیل اختراع شد.">Hill</span></div>

    - <div dir="rtl" align="right"><span title="ماشین انیگما،  دستگاهی رمزنگار برای رمزگذاری پیام بود که از اوایل تا اواسط قرن بیستم توسط آلمان نازی، برای محافظت از ارتباطات تجاری، دیپلماتیک و نظامی مورد استفاده قرار می‌گرفت. بعدا در میانه جنگ جهانی دوم، پیام‌های رمز شده با این ماشین توسط انگلستان شکسته شد. این ماشین با استفاده از چرخانه و تغییرات مکرر مسیر الکتریکی از طریق درهم‌ساز انیگما یک رمز جانشینی چندالفبایی را پیاده‌سازی می‌کند تا امنیت انیگما را فراهم می‌کند.">Enigma machine</span></div>


### <div dir="rtl" align="right"><span title="این رویکرد ترکیبی از هر دو روش جانشینی Substitution و جابجایی Permutation را برای رمزکردن را استفاده می‌کند. این رمزنگاری‌های ترکیبی در واقع اولین ایده‌ها برای رمزنگاری‌های مدرن و قدرتمندتر آینده بودند.">**Hybrid Ciphers**</span></div>

  - <div dir="rtl" align="right"><span title="ADFGX یک سیستم رمزگذاری آلمانی مربوط به دوران جنگ جهانی اول است که از یک جدول مربعی ۵×۵ و مکانیزم دوگانه جایگزینی و سپس جابجایی استفاده می‌کند.">ADFGX</span></div>

  - <div dir="rtl" align="right"><span title="این رمزنگاری در واقع بسط و توسعه روی رمزنگاری قبلی بود که در آن یک حرف اضافی، V، به حروف رمز اضافه شد و جدول آن به ۶×۶ گسترش یافت تا امکان استفاده از 26 حرف لاتین و ارقام 0 تا 9 در پیام را فراهم کند. در نهایت، این روش توسط ستوان ارتش فرانسه «ژرژ پینوین» مورد تجزیه و تحلیل قرار گرفت و این الگوریتم در سال ۱۹۱۸ شکسته شد.">ADFGVX</span></div>

  - <div dir="rtl" align="right"><span title="رمز Bifid الگوریتمی است که جانشینی حروف در جدول مربعی را با جابه‌جایی ترکیب می‌کند. این روش در حدود سال ۱۹۰۱ توسط فلیکس «دلاستل پینوین» فرانسوی اختراع شد.">Bifid</span></div>


## <div dir="rtl" align="right"><span title="رمزنگاری مدرن به شدت مبتنی بر ریاضیات، نظریه اطلاعات و علوم کامپیوتر است. الگوریتم‌های رمزنگاری حول مفروضات سختی محاسباتی طراحی شده‌اند که شکستن چنین الگوریتم‌هایی را در عمل حتی توسط کامپیوتر سخت می‌کند.">**Modern Cryptography**</span></div>
  

### <div dir="rtl" align="right"><span title="الگوریتم‌های متقارن از یک کلید رمزنگاری یکسان، هم برای رمزگذاری متن پیام و هم برای رمزگشایی متن رمز استفاده می‌کنند. این نوع رمزنگاری‌ها معمولا سرعت محاسباتی بالاتر و سربار کمتری نسبت به روش‌های نامتقارن دارند.">**Symmetric Cryptography**</span></div>

  - <div dir="rtl" align="right"><span title="این نوع از رمزنگاری که به دنباله‌ای معروف است در هر لحظه، هر بیت (بایت) متن پیام با استفاده از بیت (بایت) متناظر از کلید یک به یک رمزگذاری می‌شود تا دنباله‌ای از متن رمزگذاری شده حاصل شود.">Stream Ciphers</span></div>

    - <div dir="rtl" align="right"><span title="رمزنگاری است که در سال ۲۰۰۸ معرفی شد. آن عملکرد نرم‌افزاری سریعی دارد و معمولا سریع‌تر از AES-GCM است. ChaCha20 در بسیاری از پروتکل‌ها از جمله IPsec، SSH/TLS, WireGuard، OTRv4 و چندین پروتکل دیگر پیاده‌سازی شده است.">ChaCha20</span></div>

    - <div dir="rtl" align="right"><span title="Salsa20 از لحاظ ساختاری نزدیک به ChaCha است به شکلی که رمزها با استفاده تابع شبه تصادفی و براساس عملیات add ،rotate ،XOR ساخته تولید می‌شوند.">Salsa20</span></div>

    - <div dir="rtl" align="right"><span title="یکی از معروف‌ترین رمزهای دنباله‌ای است. در حالی که سادگی ساختاری و سرعت آن در نرم‌افزار قابل‌توجه است، اما آسیب‌پذیری‌های متعددی در RC4 کشف شده است. این رمزنگاری در پروتکل قدیمی WEP مورد استفاده در شبکه‌های Wi-Fi به کار گرفته شده بود.">RC4</span></div>


  - <div dir="rtl" align="right"><span title="در این روش پیام بعد تبدیل به رشته بیت آن را در به شکل بلوک‌ بلوک با اندازه ثابت (به عنوان مثال، 64 یا 128 بیت) رمزگذاری می‌کند. اساس این روش‌ها معمولا عمل جابجایی و جانشینی کاراکتر در دفعات زیاد استوار است.">Block Ciphers</span></div>

    - <div dir="rtl" align="right"><span title="ساختاری پایه‌ای و پدر معنوی بسیاری از الگوریتم‌ها بلوکی فعلی است. در آن داده‌ها به دو نیمه تقسیم شده و طی چندین دور، با استفاده از کلیدهای فرعی مشتق شده از کلید اصلی و جابه‌جایی نیمه‌ها، رمزنگاری و رمزگشایی انجام می‌شود.">Feistel</span></div>

    - <div dir="rtl" align="right"><span title="اولین الگوریتم رمزنگاری بلوکی استاندارد که از کلید 56 بیتی استفاده می‌کند؛ امنیت آن به دلیل اندازه کوچک کلید امروزه ضعیف تلقی می‌شود.">DES</span></div>

    - <div dir="rtl" align="right"><span title="نسخه تقویت شده DES که داده‌ها را سه بار رمزنگاری می‌کند و از کلیدهای 112 یا 168 بیتی استفاده می‌کند؛ امنیت بهتری نسبت به DES دارد اما کندتر است.">DES3</span></div>

    - <div dir="rtl" align="right"><span title="الگوریتم استاندارد رمزنگاری حال حاضر با کلیدهای 128، 192 یا 256 بیتی؛ امنیت و کارایی بالایی دارد و برای رمزنگاری داده‌ها در بسیاری از سیستم‌ها استفاده می‌شود.">AES</span></div>

    - <div dir="rtl" align="right"><span title="الگوریتم بلوکی سریع و امن با اندازه کلید متغیر از 32 تا 448 بیت؛ مناسب برای کاربردهای متنوع و به عنوان جایگزینی برای DES معرفی شد.">Blowfish</span></div>

    - <div dir="rtl" align="right"><span title="نسخه پیشرفته Blowfish و یکی از کاندیداهای استاندارد شدن با اندازه کلیدهای 128 تا 256 بیت. آن امنیت و کارایی بالا داشته و در سیستم‌های با منابع محدود به‌کار می‌رود.">Twofish</span></div>


  - <div dir="rtl" align="right"><span title="تکنیکی برای رمزنگاری ایمن پیام طولانی و بزرگ (بزرگتر از یک بلوک) است تا اثر پیام ثابت را در رمز حفظ نکند. ">Modes of Operation</span></div> 

    - <div dir="rtl" align="right"><span title="در حالت ECB (Electronic CodeBook) هر بلوک به طور مستقل با استفاده از همان کلید رمزگذاری می‌شود. با این حال، در برابر تکرار الگو آسیب‌پذیر است، زیرا بلوک‌های متن یکسان بلوک‌های متن رمزی یکسانی تولید می‌کنند.">ECB</span></div>

    - <div dir="rtl" align="right"><span title="در  Cipher Block Chaining (CBC) هر بلوک متن پیام قبل از رمزگذاری با بلوک متن رمز قبلی XOR می شود، که الگوها را پنهان می‌کند. بلوک اول از یک بردار اولیه (IV) برای تصادفی بودن استفاده می‌کند. ">CBC</span></div>
    - <div dir="rtl" align="right"><span title="این حالت (CFB) Cipher FeedBack یک رمز بلوکی را با رمزگذاری یک IV و XOR کردن نتیجه با متن ساده برای تولید متن رمز و سپس جابجایی IV، به یک رمز جریان تبدیل می‌کند. ">CFB</span></div>

    - <div dir="rtl" align="right"><span title=" این حالت (Output FeedBack) شبیه CFB است، اما با رمزگذاری IV و استفاده از آن در عملیات XOR، جریان کلید را از قبل تولید می‌کند و آن را مستقل از پیام، رمز می‌کند.">OFB</span></div>

    - <div dir="rtl" align="right"><span title="در حالت Counter Mode (CTR) هر  بلوک با ترکیب یک مقدار شمارنده (که برای هر بلوک افزایش می‌یابد با یک nonce  رمزگذاری می‌شود. متن پیام با کلید XOR شده است. این روش در صورت پیاده‌سازی درست بسیارامن و کارامد است.">CTR</span></div>


### <div dir="rtl" align="right"><span title="الگوریتم‌های نامتقارن از یک جفت کلید (یک کلید عمومی و یک کلید خصوصی) که براساس ریاضی با هم مرتبط‌اند، برای رمز کردن استفاده می‌کنند. این روش امنیت بالاتر اما سرعت محاسباتی کمتری نسبت به روش متقارن دارد.">**Asymmetric Cryptography**</span></div>

  - <div dir="rtl" align="right"><span title="فرآیندی که از کلید عمومی برای رمزگذاری و کلید خصوصی مرتبط با آن برای رمزگشایی پیام استفاده می‌کند. این فرایند برای مخفی کردن پیام و ارسال به شکل محرمانه استفاده می‌شود.">Encryption</span></div>

    - <div dir="rtl" align="right"><span title="الگوریتم RSA (Rivest–Shamir–Adleman) رمزنگاری نامتقارن مبتنی بر سختی تجزیه (factorization) اعداد بزرگ (بیش از ۵۱۲ بیت) به عوامل اول آن است که در سال ۱۹۷۷ معرفی شد. سادگی و کارآمدی آن باعث استفاده گسترده در بسیاری از پروتکل‌ها شده است.">RSA</span></div>

    - <div dir="rtl" align="right"><span title=" رمزنگاریِ کوله‌پشتی مرکل-هلمن یکی از اولین رمزنگاری‌های کلید عمومی است که توسط رالف مرکل و مارتین هلمن در سال ۱۹۷۸ ارائه شد. این بر اساس مسئله «جمع زیرمجموعه‌ها» است (مورد خاصی از مسئله کوله پشتی). سرانجام، یک حمله توسط shamir  در سال ۱۹۸۴ منتشر شد باعث شد این رمزنگاری اکنون ناامن در نظر گرفته شود."> Merkle–Hellman knapsack</span></div>

    - <div dir="rtl" align="right"><span title="یک الگوریتم نامتقارن برای رمزنگاری و امضای دیجیتال است. امنیت آن بر پایه سختی مسئله لگاریتم گسسته (Discrete logarithms) در گروه‌های دوری (Cyclic group) است. این الگوریتم یک رمزنگاری احتمالاتی است که یک پیام ثابت ممکن است به رمزهای متفاوت تبدیل شود. از این رو امنیت خوبی دارد اما طول پیام‌های رمزنگاری‌شده نسبت به دیگر الگوریتم‌ها بزرگ‌تر است.">ElGamal</span></div>

    - <div dir="rtl" align="right"><span title="الگوریتم‌های ECC (Elliptic-Curve Cryptography) براساس ساختارهای جبری روی منحنی‌های بیضوی متفاوت در میدان‌های متناهی است. ECC به کلیدهای با اندازه کوچکتر اجازه می‌دهد تا همان امنیت معادل با سیستم‌های رمزنگاری مانند RSA و ElGamal را فراهم کند که نشان‌دهنده کارآمدی این نوع رمزنگاری است.">ECC</span></div>

      - <div dir="rtl" align="right"><span title="در رمزنگاری، Curve25519 یک منحنی بیضوی (y^{2}=x^{3}+486662x^{2}+x) است که در رمزنگاری منحنی بیضوی (ECC) استفاده می‌شود که 128 بیت امنیت (اندازه کلید 256 بیت) ارائه می‌کند. این یکی از سریع‌ترین منحنی ها در ECC است.">Curve25519</span></div>

      - <div dir="rtl" align="right"><span title="P-256 که با نام secp256r1 نیز شناخته می‌شود، یک منحنی بیضوی پرکاربرد در رمزنگاری است که امنیت 128 بیتی را ارائه می‌دهد. این منحنی در پروتکل‌هایی مانند TLS، SSL و امضاهای دیجیتال استفاده می‌شود و تعادلی از امنیت و کارایی قوی با اندازه کلید 256 بیتی را فراهم می‌کند.">P-256</span></div>
      
  - <div dir="rtl" align="right"><span title="در این روش، از رمزنگاری نامتقارن و جفت کلید آن برای تبادل امن یک کلید متقارن (مثلا کلید AES)  در یک کانال ناامن استفاده می‌شود.">Key Exchange</span></div> 
    
    - <div dir="rtl" align="right"><span title=" روش مبادله کلید Diffie–Hellman (DH) مبتنی بر رمزنگاری نامتقارن بر دشواری مسئله لگاریتم گسسته متکی است، که تضمین می‌کند حتی اگر مهاجم داده‌های مبادله شده را رهگیری کند، نمی‌تواند به راحتی کلید مشترک را محاسبه کند. با این حال این روش نمی‌تواند احراز هویت طرفین مبادله را تصدیق کند.">DH</span></div> 
    
    - <div dir="rtl" align="right"><span title=" گونه‌ای از DH است که از رمزنگاری منحنی بیضوی (ECC)  برای تبادل کلید استفاده می‌کند. این گونه کارکرد مشابه DH ، اما با اندازه‌ کلید کوچک‌تر ارائه می‌کند. ECDH به طور گسترده در پروتکل‌های مدرن مانند TLS و Signal  برای ارتباطات ایمن استفاده می‌شود.">ECDH</span></div> 

  - <div dir="rtl" align="right"><span title="در این الگوریتم‌ها می‌توان تایید هویت پیام یا اسناد دیجیتال را بررسی کنید. در این الگوریتم‌ها با کلید خصوصی عمل امضا صورت می‌گیرد و با استفاده از کلید عمومی مرتبط‌ اش، امضا قابل اعتبارسنجی است.">Signature</span></div>

    - <div dir="rtl" align="right"><span title=" امضای RSA همان ساختار روش رمزنگاری آن را دارد اما از کلید خصوصی برای امضای پیام استفاده می‌کند تا صحت و یکپارچگی پیام امضا شده را تضمین کند. سپس با رمزگشایی امضا با کلید عمومی و مقایسه آن با پیام، آن امضا را تأیید می‌کند. امضای RSA در برابر حمله Chosen-Message آسیب‌پذیر است.">RSA</span></div>

    - <div dir="rtl" align="right"><span title="اساس امضای ElGamal همان روش رمزنگاری آن یعنی لگاریتم گسسته است. از کلید خصوصی برای امضا کردن و از کلید عمومی برای اعتبارسنجی آن استفاده می‌شود. این الگوریتم به ندرت به شکل عملی استفاده می‌شود.">ElGamal</span></div>

    - <div dir="rtl" align="right"><span title="امضای Digital Signature Algorithm (DSA)، بر پایه مفهوم ریاضی توان‌رسانی پیمانه‌ای و مسئله لگاریتم گسسته است. آن در واقع گونه‌ای از امضای الجمال است که در سال ۱۹۹۱ توسط NIST به عنوان امضای استاندارد در نظر گرفت.">DSA</span></div> 

    - <div dir="rtl" align="right"><span title="گونه‌ای از DSA  با اندازه‌ کلید کوچکتر و کارایی بالاتر در مقایسه با DSA  که از رمزنگاری منحنی بیضوی استفاده می‌کند. ECDSA به طور گسترده در پروتکل های ارتباطی امن مانند SSL/TLS و بیت کوین برای تأیید تراکنش‌ها استفاده می‌شود.">ECDSA</span></div>

    - <div dir="rtl" align="right"><span title=" امضای Schnore به دلیل سادگی، کارایی و امنیت قوی بر اساس دشواری مسئله لگاریتم گسسته شناخته شده است. امضاهای کوتاه تولید می کند. Schnorr کارآمدتر از DSA و ECDSA است و مبنایی برای طرح‌های چندامضایی است که در بیت کوین Taproot با مجتمع کردن امضاها باعث مقیاس‌پذیری (Scalability) می‌شود.">Schnorr</span></div>  


##  <div dir="rtl" align="right"><span title="رمزنگاری پس کوانتومی (PQC)، توسعه الگوریتم‌های رمزنگاری (معمولاً الگوریتم‌های کلید عمومی) است که در برابر حمله رمزنگاری توسط رایانه‌های کوانتومی ایمن هستند. PQC یک رمزنگاری براساس مبانی کلاسیک ریاضی و مسائل NP-hard است که می‌تواند در مقابل حملات کوانتومی مقاومت کند در حالی که قابل اجرا بر روی رایانه‌های فعلی است و نیازی به هیچ سخت افزار جدیدی ندارند. این الگوریتم ها معمولا اندازه کلید بزرگی دارند. تحقیقات رمزنگاری پساکوانتومی، بیشتر بر روی پنج رویکرد مختلف متمرکز است:">**Post-quantum Cryptography**</span></div>

### <div dir="rtl" align="right"><span title="رمزنگاری مشبک-مبنا (Lattice -based) شاخه‌ای از رمزنگاری نامتقارن است.این نوع رمزنگاری از یکی گزینه‌های اصلی برای رمزنگاری پساکوانتومی است. این رمزنگاری بر مسائل سختی مانند مسئله یادگیری با خطا (LWE) با مسئله کوتاه‌ترین بردار (ُSVP) استوار هستند.">**Lattice-based**</span></div>

  - <div dir="rtl" align="right"><span title="کپسوله کردن کلید (KEM)، یک سیستم رمزنگاری نامتقارن است که به فرستنده اجازه می‌دهد تا علی‌رغم شنود متخاصم، یک کلید مخفی تولید کرده و به طور ایمن آن را به گیرنده ارسال کند. تفاوت بین طرح‌های رمزنگاری نامتقارن و KEM در این است که یک رمزنگاری نامتقارن به فرستنده اجازه می‌دهد تا یک پیام دلخواه را انتخاب کند، در حالی که یک KEM کلید مخفی را به طور تصادفی توسط الگوریتم تولید و برای فرستنده ارسال می‌کند این کپسوله مردن در رمزنگاری‌های پساکوانتمی بکار می‌روند..">Key Encapsulation</span></div>

    - <div dir="rtl" align="right"><span title="NTRU یک سیستم رمزنگاری کلید عمومی منبع باز است. اولین نسخه از نوع که NTRU نام داشت در سال 1996 توسط ریاضیدانان جفری هافستاین، جیل پیفر و جوزف سیلورمن توسعه یافت. NTRUencrypt ثبت اختراع شده است، اما در سال 2017 در معرض مالکیت عمومی قرار گرفت.">NTRUEncrypt</span></div>  

    - <div dir="rtl" align="right"><span title="یک سازوکار کپسوله سازی کلید (KEM) طراحی شده برای مقاومت در برابر رایانه های کوانتومی قدرتمند آینده است. از آن برای ایجاد یک کلید مخفی مشترک بین دو طرف در ارتباط استفاده می شود تا یک مهاجم با شرایط (IND-CCA2) در سیستم انتقال قادر به رمزگشایی آن نباشد. این سیستم بر اساس مسئله گونه پیمانه‌ای از LWE به نام (M-LWE)است.">Kyber</span></div>  

    - FrodoKEM
  - Signature
    - Dilithium
    - Falcon

### <div dir="rtl" align="right"><span title="سیستم‌های رمزنگاری PQC که امنیت آنها تا حدی یا به طور کامل به دشواری رمزگشایی یک کد تصحیح خطای خطی (linear error-correcting) مانند کد Goppa باینری بستگی دارد.">**Code-based**</span></div>   

  - <div dir="rtl" align="right"><span title="کپسوله کردن کلید (KEM)، یک سیستم رمزنگاری نامتقارن است که به فرستنده اجازه می‌دهد تا علی‌رغم شنود متخاصم، یک کلید مخفی تولید کرده و به طور ایمن آن را به گیرنده ارسال کند. تفاوت بین طرح‌های رمزنگاری نامتقارن و KEM در این است که یک رمزنگاری نامتقارن به فرستنده اجازه می‌دهد تا یک پیام دلخواه را انتخاب کند، در حالی که یک KEM کلید مخفی را به طور تصادفی توسط الگوریتم تولید و برای فرستنده ارسال می‌کند این کپسوله مردن در رمزنگاری‌های پساکوانتمی بکار می‌روند..">Key Encapsulation</span></div>

    - Niederreiter
    - Classic McEliece
    - Bike
  - Signature
    - Niederreiter

###  <div dir="rtl" align="right"><span title="ایده قدیمی و اصطلاح عمومی برای رمزنگاری  بر اساس امنیت توابع Hash  است که به عنوان نوعی رمزنگاری پسا کوانتومی مورد توجه است. این نوع برای ارائه طرح‌های امضای دیجیتال مانند طرح امضای مرکل استفاده می‌شود. ">**Hash-based Signatures**</span></div>

  - XMSS
  - Sphincs+

### <div dir="rtl" align="right"><span title=" رمزنگاری چندمتغیره (Multivariate) اصطلاحی برای نوعی رمزنگاری‌های نامتقارن بر اساس چند جمله‌ای‌های با چند متغیر در یک میدان متناهی F است. ">**Multivariate-based**</span></div>


  - <div dir="rtl" align="right"><span title="کپسوله کردن کلید (KEM)، یک سیستم رمزنگاری نامتقارن است که به فرستنده اجازه می‌دهد تا علی‌رغم شنود متخاصم، یک کلید مخفی تولید کرده و به طور ایمن آن را به گیرنده ارسال کند. تفاوت بین طرح‌های رمزنگاری نامتقارن و KEM در این است که یک رمزنگاری نامتقارن به فرستنده اجازه می‌دهد تا یک پیام دلخواه را انتخاب کند، در حالی که یک KEM کلید مخفی را به طور تصادفی توسط الگوریتم تولید و برای فرستنده ارسال می‌کند این کپسوله مردن در رمزنگاری‌های پساکوانتمی بکار می‌روند..">Key Encapsulation</span></div>

    - Matsumoto-Imai
    - HFE
  - Signature
    - Matsumoto-Imai
    - Rainbow

###  <div dir="rtl" align="right"><span title=" نوعی رمزنگاری نسبتا جدید که اساس آن منحنی بیضوی است که امنیت آن بر (تجسم‌های مختلف) مشکل یافتن یک isogeny صریح بین دو منحنی بیضوی فوق‌منفرد (supersingular elliptic curves) روی یک میدان متناهی F متکی است.">**Isogeny-based**</span></div>
  
  - Sike


##  <div dir="rtl" align="right"><span title=" آنها می توانند برای نگاشت داده‌هایی با اندازه دلخواه به مقادیر با اندازه ثابت استفاده شوند. آنها الگوریتم‌های معکوس‌ناپذیر هستند و احتمال اینکه دو متن به یک مقدار نگاشت شود بسیار بسیار کم است.">**Hash Functions**</span></div> <!-- markmap: fold -->

  - **MD5**
  - **SHA-1**
  - **SHA-2 (SHA-256, SHA-512)**
  - **SHA-3 (Keccak)**
  - **HMAC (Hash-based Message Authentication Code)**
  - **BLAKE2**
  - **PBKDF2 (Password-Based Key Derivation Function 2)**
  - **bcrypt**
  - **Argon2**


## <div dir="rtl" align="right"><span title="تعدادی از تهدیدات مهم موجود در دنیای رمزنگاری که ممکن است به عنوان یک آسیب‌پذیری یک الگوریتم رمزنگاری لحاظ شود.">**Main Threats**</span></div> <!-- markmap: fold -->


  -  <span title="Tries every possible key until the correct one is found">**Brute Force Attack**</span>

  -  <span title="A method used to crack substitution ciphers by analyzing how frequently certain letters appear in the ciphertext and comparing these frequencies to typical letter distributions in the language. For example, in English, E is the most common letter. If the most frequent letter in the ciphertext is Q, it might correspond to E in the plaintext.">**Frequency Analysis (Classical Ciphers)**</span>
  
  - <span title="The attacker has access to both the plaintext and its corresponding ciphertext and uses this information to derive the key">**Known-plaintext Attack**</span>

  - <span title="The attacker can choose arbitrary plaintexts and obtain their corresponding ciphertexts, allowing them to gather information to break the encryption">**Chosen-plaintext Attack**</span>
  
  - <span title="The attacker can decrypt chosen ciphertexts and use this to gain information about the encryption key or algorithm">**Chosen-ciphertext Attack**</span>

  -  <span title="A known-plaintext attack that targets block ciphers by using a space-time tradeoff, working faster than brute force by exploiting the structure of two-key encryption schemes">**Meet-in-the-Middle Attack**</span>

  - <span title="Exploits physical leakages like timing or power consumption to break encryption">**Side-Channel Attacks**</span>
    -  <span title="Measures the time it takes to perform cryptographic operations to deduce secret keys">Timing Attacks</span>

    - <span title="Monitors power consumption during encryption to extract information about the key">Power Analysis</span>

  - <span title="Analyzes the differences in ciphertexts resulting from slight differences in the plaintext to discover the secret key"> **Differential Cryptanalysis**</span>

  - <span title="Uses linear approximations to describe the behavior of block ciphers and analyzes the relationships between plaintext, ciphertext, and key bits">**Linear Cryptanalysis**</span>

  - <span title="Exploits incorrect padding in cryptographic systems to recover plaintext by sending carefully crafted ciphertexts">**Padding Oracle Attacks**</span>

  - <span title="Use quantum computer to break the existing cryptography algorithms">**Quantum computing**</span>
    - <span title="Breaks RSA by efficiently factoring large numbers and ECC by discrete logarithm">Shor's Algorithm </span>
    - <span title="Speeding up Symmetric Key Search">Grover's Algorithm </span>

## <div dir="rtl" align="right"><span title=" الگوریتم‌های مهم و کاربردی دیگر که در دسته‌بندی‌های بالا قرار نمی‌گیرند در اینجا قرار دارند.">**Misc Algorithms**</span></div> <!-- markmap: fold -->
  - <span title="a form of encryption with an additional evaluation capability for computing over encrypted data without access to the secret key"> **Homomorphic Encryption** </span> 

    - Partial Homomorphic (PHE)
      - <span title=" RSA is only a multiplicatively homomorphic."> RSA </span> 
      - <span title=" The scheme is an additive homomorphic cryptosystem; this means that, given only the public key and the encryption of m1 and m2, one can compute the encryption of m1+m2"> Paillier </span> 
      
    - Fully Homomorphic (FHE)
      - CKKS 
      - BVG
  - <span title="Methods for distributing a secret among a group, in such a way that no individual holds any intelligible information about the secret, but when a sufficient number of individuals combine their 'shares', the secret may be reconstructed"> **Secret Sharing** </span>  
  - <span title="a shift register whose input bit is a linear function of its previous state."> **Linear Feedback Shift Register (LFSR)** </span>   
  - **Commitment scheme**
    - Pedersen Commitment



