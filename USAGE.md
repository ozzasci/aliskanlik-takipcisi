# Kullanım: manifest ve mobil patch ekleme

Bu repo için PWA ve mobil iyileştirmelerini etkinleştirmek için iki adım önerilir:

1) app.html içinde <head> bölümüne şu satırları ekleyin:

<link rel="manifest" href="/manifest.json">
<link rel="icon" href="/assets/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/assets/icon-192.svg">
<link rel="stylesheet" href="/assets/mobile-patch.css">

2) (Opsiyonel) Kullanıcı deneyimini geliştirmek için sayfaya alt gezinme eklemek isterseniz, body kapanışından hemen önce şu HTML bloğunu ekleyebilirsiniz:

<div class="mobile-bottom-nav">
  <a href="#">Ana</a>
  <a href="#">Görevler</a>
  <a href="#">Asistan</a>
  <a href="#">Profil</a>
</div>

Bu değişiklikleri yapmak isterseniz, ben sizin için app.html dosyasına güvenli bir patch de oluşturabilirim (ayrıca branch + PR şeklinde), ya da siz doğrudan ekleyebilirsiniz.
