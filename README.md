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

![Ekran görüntüsü 2024-07-12 163735](https://github.com/user-attachments/assets/2e1d2aa5-8999-4d3a-804f-90e42aebaeeb)
![Ekran görüntüsü 2024-07-12 163813](https://github.com/user-attachments/assets/ffa6c4d4-03a2-4416-a5d7-f188d5cf76d1)
![Ekran görüntüsü 2024-07-12 163744](https://github.com/user-attachments/assets/03d191fc-ad5b-426b-a86b-9cce2a17c0f2)

