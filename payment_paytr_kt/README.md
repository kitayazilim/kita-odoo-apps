<h2>PayTR Ödeme Sağlayıcı Entegrasyonu</h2>

<p>
Bu modül, Odoo ile PayTR ödeme altyapısını entegre eder ve müşterilerinizin PayTR iframe çözümü ile güvenli şekilde ödeme yapmasını sağlar. PayTR, Türkiye'de yaygın olarak kullanılan ve kredi kartı, banka kartı, taksitli ödeme gibi birçok seçeneği destekleyen bir ödeme altyapısıdır.
</p>

<h3>Özellikler</h3>
<ul>
  <li>PayTR iframe ödeme çözümü ile tam entegrasyon</li>
  <li>Kredi kartı ile ödeme desteği</li>
  <li>Taksitli ödeme seçenekleri</li>
  <li>Troy kart sistemi desteği</li>
  <li>Otomatik işlem durumu güncellemeleri</li>
  <li>Geliştirme ve test için test modu</li>
</ul>

<h3>Gereksinimler</h3>
<ul>
  <li>Odoo v16.0, v17.0, v18.0</li>
  <li>PayTR mağaza hesabı</li>
  <li>PayTR API bilgileri (Mağaza Numarası, API Key, API Salt)</li>
</ul>

<h3>Kurulum</h3>
<ol>
  <li>Bu repoyu Odoo eklenti dizininize klonlayın:<br>
    <code>git clone https://github.com/kitayazilim/kita-odoo-apps /path/to/odoo/addons/payment_paytr_kt</code>
  </li>
  <li>Odoo'da Uygulamalar menüsüne gidin ve "Uygulama Listesini Güncelle" seçeneğine tıklayın.</li>
  <li>"PayTR iFrame" araması yaparak modülü yükleyin.</li>
  <li>Alternatif olarak ZIP dosyasını yükleyerek de kurulum yapabilirsiniz.</li>
</ol>

<h3>Yapılandırma</h3>
<ol>
  <li>Faturalandırma/Muhasebe > Yapılandırma > Ödeme Sağlayıcıları menüsüne gidin.</li>
  <li>Yeni bir ödeme sağlayıcı oluşturun veya mevcut PayTR sağlayıcısını düzenleyin.</li>
  <li>Sağlayıcıyı "PayTR" olarak seçin.</li>
  <li>PayTR mağaza bilgilerinizi girin:
    <ul>
      <li>Mağaza Numarası (Merchant ID)</li>
      <li>Mağaza API Key</li>
      <li>Mağaza API Salt</li>
    </ul>
  </li>
  <li>Ek ayarları yapılandırın:
    <ul>
      <li>Tek çekim seçeneği</li>
      <li>En fazla taksit sayısı</li>
      <li>Zaman aşımı limiti</li>
    </ul>
  </li>
  <li>Test için "Test Modu", canlı kullanım için "Etkin" olarak ayarlayın.</li>
</ol>

<h3 style="color:red">PayTR Canlıya Alma <span class="fa fa-plug"></span></h3>
<ol>
  <li>PayTR api hesabınıza girip Destek ve Kurulum Başlığı altındaki ayarlardan bildirim url ini değiştir diyerek site adresinizin sonuna <strong>/payment/paytr/return</strong> kısmını ekleyin</li>
  <li>Odoo uygulamazda Muhasebe > Yapılandırma > Ödeme Sağlayıcıları menüsünden PayTR iFrame sağlayıcısına girin.</li>
  <li>Ödeme Sistemini Test moduna geçirin ve web sayfanızdan sepetinizi bir ürün ekleyerek ilk test isteğiniz ile ödemeyi tamamlayın.</li>
  <li>Yukarıdaki adım PayTR hesabınızı canlıya almak için zorunludur.</li>
  <li>İlk test isteğiyle sipariş geçtikten sonra PayTR api hesabınıza girip canlıya alma yönergelerini takip edin</li>
  <li>Son olarak daha önce Odoo dan test moduna aldığınız PayTR Iframe i etkinleştirerek canlı moda geçirebilirsiniz</li>
</ol>

<h3>Kullanım</h3>
<p>
Yapılandırma tamamlandığında, PayTR ödeme seçeneği web sitenizin ödeme sayfasında görünecektir. Müşteriler bu yöntemi seçtiğinde, PayTR iframe ekranına yönlendirilerek ödemelerini güvenli şekilde tamamlayabilirler.
</p>

<h3>Destek</h3>
<p>
Destek için Kıta Yazılım ile iletişime geçebilirsiniz:<br>
Web: <a href="https://kitayazilim.com" target="_blank">https://kitayazilim.com</a><br>
E-posta: <a href="mailto:info@kitayazilim.com">info@kitayazilim.com</a><br>
Yardım Masası: <a href="mailto:destek@kitayazilim.com">destek@kitayazilim.com</a>
</p>

<h3>Lisans</h3>
<p>
Bu modül LGPL-3 lisansı ile lisanslanmıştır.
</p>
