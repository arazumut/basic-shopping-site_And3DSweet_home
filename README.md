  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
    </a> <h1>Basic Shopping Site</h1>
Bu kod, temel bir alışveriş sitesi için JavaScript ile yazılmış bir ön yüz (frontend) uygulamasıdır. Kullanıcıların ürünleri görüntüleyip sepete eklemelerine, sepeti görüntülemelerine ve sepeti yönetmelerine olanak tanır. İşte kodun ayrıntılı açıklaması:

HTML Elemanları
Kod, aşağıdaki HTML elemanlarına referanslar içerir:

productDOM: Ürünlerin görüntülendiği bölüm.
cartDOM: Sepet bölümünü temsil eder.
cartContent: Sepet içeriği.
openCart: Sepeti açmak için kullanılan ikon.
closeCart: Sepeti kapatmak için kullanılan buton.
overlay: Sepet açıldığında arka planda beliren kaplama.
cartTotal: Toplam sepet tutarını gösterir.
clearCartBtn: Sepeti temizlemek için kullanılan buton.
itemTotals: Sepetteki toplam ürün sayısını gösterir.
Değişkenler
cart: Sepetteki ürünleri saklar.
buttonDOM: Ürünlerin "Add to Cart" butonlarını saklar.
UI Sınıfı
Kullanıcı arayüzüyle ilgili işlemleri yönetir:

displayProducts: Ürünleri sayfada gösterir.
getButtons: "Add to Cart" butonlarını elde eder ve bunlara olay dinleyicileri ekler.
setItemValues: Sepetin toplam tutarını ve toplam ürün sayısını hesaplar ve günceller.
addCartItem: Ürünü sepete ekler ve sepet içeriğini günceller.
show: Sepeti gösterir.
hide: Sepeti gizler.
setAPP: Uygulama başlatıldığında gerekli ayarları yapar.
populate: Sepeti mevcut ürünlerle doldurur.
cartLogic: Sepetle ilgili işlemleri (ürün ekleme, çıkarma, artırma, azaltma) yönetir.
clearCart: Sepeti temizler.
removeItem: Sepetten ürün çıkarır.
singleButton: Tek bir ürünün "Add to Cart" butonunu döndürür.
Products Sınıfı
Ürünlerle ilgili işlemleri yönetir:

getProducts: Ürünleri bir JSON dosyasından getirir.
Storage Sınıfı
Yerel depolama (localStorage) işlemlerini yönetir:

saveProduct: Ürünleri yerel depolamaya kaydeder.
saveCart: Sepeti yerel depolamaya kaydeder.
getProduct: Belirli bir ürünü yerel depolamadan alır.
getCart: Sepeti yerel depolamadan alır.
DOMContentLoaded Olayı
Sayfa yüklendiğinde aşağıdaki işlemleri gerçekleştirir:

productList ve ui nesnelerini oluşturur.
setAPP methodunu çağırarak uygulamayı başlatır.
Ürünleri getirir ve sayfada gösterir.
Ürünleri yerel depolamaya kaydeder.
Butonları etkinleştirir ve sepet işlemlerini başlatır.
Bu kod, kullanıcıların ürünleri sepete ekleyip çıkarabilecekleri, sepetin toplam tutarını ve ürün miktarını görebilecekleri basit bir alışveriş deneyimi sağlar.
![Ekran görüntüsü 2024-03-23 215345](https://github.com/arazumut/basic-shopping-site/assets/150933483/c8761751-4967-4b10-af5d-46710a86c466)
![Ekran görüntüsü 2024-03-23 215408](https://github.com/arazumut/basic-shopping-site/assets/150933483/c2b406db-e5b1-47c0-a8d5-49156cac6f0e)
![Ekran görüntüsü 2024-08-01 232757](https://github.com/user-attachments/assets/0a4025d1-a28d-4ea6-9874-39934d6fea30)


  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
    </a> 
<h1>3D Home</h1>

Bu kod, Three.js kullanarak temel bir 3D sahne oluşturur ve bir web tarayıcısında görüntülenmesini sağlar. İşte kodun ayrıntılı açıklaması:

HTML Elemanları
canvas: WebGL içeriklerinin çizileceği <canvas> HTML elemanını seçer.
Three.js Sahne Kurulumu
scene: Yeni bir Three.js sahnesi oluşturur.
textureLoader: Doku yüklemek için kullanılır.
sizes: Tarayıcı penceresinin genişlik ve yüksekliğini içerir.
Kamera
camera: Perspektif kamera oluşturur ve sahneye ekler.
Kameranın pozisyonu ayarlanır (x: -14, y: 6, z: 16).
Kontroller
controls: Kamera kontrollerini sağlar (OrbitControls kullanılır).
Kamerayı döndürme, yakınlaştırma ve kaydırma özellikleri etkinleştirilir.
Minimum ve maksimum mesafe ile minimum ve maksimum polar açı sınırlandırılır.
Renderer
renderer: WebGLRenderer oluşturur.
Pencere boyutlarına göre render ayarları yapılır.
Pixel oranı ve çıktı kodlaması ayarlanır (sRGB).
Işıklar
light: Çeşitli yönlerde farklı ışıklar sahneye eklenir (Top, Left, Right, Front, Back).
rectLight: Dikdörtgen alan ışığı eklenir ve sahnenin ortasına yerleştirilir.
Malzemeler
bakedTexture: Bir doku yükler ve ters çevrilmesini önler.
normalTexture ve occlusionTexture: Normal ve ortam oklüzyon dokuları yüklenir (boş bırakılmış).
bakedMaterial ve metalicMaterial: MeshStandardMaterial ile iki malzeme oluşturur.
Model Yükleyici
loader: GLTFLoader kullanarak modelleri yükler.
İki model yüklenir ve malzemeleri atanır.
Yükleme durumu konsola yazdırılır.
Pencere Yeniden Boyutlandırma
Pencere boyutları değiştiğinde kamera ve renderer boyutları güncellenir.
Animasyon Döngüsü
tick: Animasyon döngüsünü başlatır.
Kontroller güncellenir.
Kameranın hedefi belirli sınırlar içinde kalacak şekilde ayarlanır.
Sahne render edilir.
requestAnimationFrame ile sürekli olarak güncellenir.
rectLight'ın rengini zamanla değiştirir.
Bu kod, tarayıcıda 3D sahneyi görselleştirmek, kamerayı kontrol etmek ve modelleri yüklemek için gerekli tüm temel işlemleri yapar. Sahneye ışıklar ekleyerek ve malzemeleri ayarlayarak gerçekçi bir görünüm sağlanır. Pencere yeniden boyutlandırıldığında sahnenin ve kameranın boyutlarını günceller, böylece her zaman doğru görünüm sağlar.


![Ekran görüntüsü 2024-07-12 163735](https://github.com/user-attachments/assets/2e1d2aa5-8999-4d3a-804f-90e42aebaeeb)
![Ekran görüntüsü 2024-07-12 163813](https://github.com/user-attachments/assets/ffa6c4d4-03a2-4416-a5d7-f188d5cf76d1)
![Ekran görüntüsü 2024-07-12 163744](https://github.com/user-attachments/assets/03d191fc-ad5b-426b-a86b-9cce2a17c0f2)

