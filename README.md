

Fikret ÇAKIRLI 140401099

bu programı asal sayıları içeren asallar.txt dosyasından verileri okuyup 
üçüncü dereceden polinoma uyudurup bulunduğu denkleminin birinci dereceden 
türevini bulan ve polinomu kullanmadan da sonucu elde eden bir yazılımdır.

programındaki fonksiyonları sırasıla çalışmaktadır
- ```asal_yaz(asal)``` fonksiyonu
ile bir kez çalıştırıp asallar.txt dosyası oluşturulur.
- ```f(denklem,x_degeri)``` fonksiyonu ise
denklemi kullanabilmesi ve denklemde ki x değişkenine değer atabilmesi kolaylaştıran
ve sonucu elde eden bir fonksiyondur.
- ```turev_bul_polinom(denklem)``` fonksiyonu
ileri fark türevi alma yöntemi  "a" değeri öğrenci numaramla son iki hanelik 
ile türevi polinom denklemi kullanarak ve sonucu return eden fonksiyondur.
- ```turev_bul_polinomsuz()```  fonksiyonu 
polinom denklemi kullanmadan ve aynı yöntemi "ileri fark" kullanarak
sayısal olarak hesaplar ve sonucu return eder.
- ```yorum_yap()``` fonksiyonu 
yaptığım çıkarımsalları yourum.txt şeklinde bir dosya olarak yazdırır.

**programının çalışma senaryosu:**
kısaca bu programı asal sayıları asallar dosyasından okur , xlerin toplamı 
ve ylerin toplamı ...vs matrisi oluşturan değişkenleri üzerinde işlemleri yapabilmekte
matrisinin determinantı bulup y"lerin sutünü matrisile yer değiştirerek tüm 
determinantları bulur , determinantları orginal matrisinin determinantıla bölerek 
a0 ,a1 ,a2 ..vs katsayıları bulurdur . ve bu adımda polinom denklemi elde edlmiş olur .
bulduğumuz denklemi ```turev_bul_polinom``` fonksiyonuna parametre olarak atılır 
, bu fonksiyonu h değeri 0.01 ve x0 değeri ise öğrenci numaramla son iki hanelik 
olarak bilirlenmişimdir , ileri fark türevi  formula f(x0+h)-f(x0) uygulanarak türevi elde
edilir ve kullancıya ekran çıktısı şeklinde gösterir. bu formula ile  "f(denklem,x_degeri)" yardımcı fonksiyonu ile bulunur .
sonraki satırda "turev_bul_polinomsuz" fonksiyonuna çağrılır , bu fonksiyonu direk 
asallar.txt dosyasından ki bulunan verilerile işlem yapar ileri fark yöntemi ile 
 sonucu elde eder ve kullancıya ekran çıktısı şeklinde gösterirdir.

**gereksinimler ve kullanımı:**
- işletim sistemi linux ise  genelde python veya python3 üyklüdür ,üyklü değilse 
kullandığın dağıtım"in deposu komutu yazıp install python3 şeklinde inmiş olur 
- işletim sistemi windows ise manuel python3 indirip bin dizisini program files içinde alıp 
windows environment path değişkenine eklemeniz gerekir  .

python kurduğunuz zaman indirmeniz gereken  numpy kitapliği bunu indirmeden kod çalışmıyabilirdir 
windows powershell den pip install numpy şeklinde indirebilirsiniz , linux ise terminal dan bunu yazarsınız.

kodu turev.py dosyasından ```python3 .\turev.py``` yazarak çaılştırabilirsiniz ,tabi ki asallar.txt dosyasi aynı dizinde 
olmalıdır . 




