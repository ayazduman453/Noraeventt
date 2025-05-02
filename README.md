<!DOCTYPE html> <html lang="tr"> <head> <meta charset="UTF-8">
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nora Event | Davet & Organizasyon</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #fff0f5;
      color: #4b2e2e;
    }
    header {
      background: #8b5e83;
      color: white;
      padding: 30px 20px;
      text-align: center;
    }
    nav {
      background: #6d4c66;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }
    section {
      padding: 40px 20px;
    }
    .hero {
      background: url('https://via.placeholder.com/1200x400') center/cover no-repeat;
      color: white;
      text-align: center;
      padding: 100px 20px;
    }
    .hero h1 {
      font-size: 48px;
      text-shadow: 2px 2px 4px #000;
    }
    .gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.gallery img {
  flex: 1 1 calc(33% - 20px);
  margin: 10px;
  max-width: calc(33% - 20px);
}
@media (max-width: 768px) {
  .gallery img {
    max-width: 100%;
    flex: 1 1 100%;
  }
}
    }
    .contact, .form-container {
      background: #f8e1ec;
      padding: 30px;
      border-radius: 10px;
      max-width: 600px;
      margin: 30px auto;
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      background-color: #8b5e83;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      background: #4b2e2e;
      color: white;
      text-align: center;
      padding: 20px;
    }
    .whatsapp-button {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #25d366;
      color: white;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 30px;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3);
      z-index: 1000;
      text-decoration: none;
    }
  </style>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
  <header>
    <h1>NORA EVENT</h1>
    <p>Davet & Organizasyon</p>
  </header>
  <nav>
    <a href="#hakkimizda">Hakkımızda</a>
    <a href="#hizmetler">Hizmetler</a>
    <a href="#galeri">Galeri</a>
    <a href="#iletisim">İletişim</a>
    <a href="#rezervasyon">Rezervasyon</a>
  </nav>
  <div class="hero">
    <h1>Hayalinizdeki Davet İçin Nora Event</h1>
    <p>Düğün, nişan, doğum günü ve özel kutlamalar için profesyonel hizmet</p>
  </div>
  <section id="hakkimizda">
    <h2>Hakkımızda</h2>
    <p>Nora Event, Sakarya'nın Erenler ilçesinde yer alan gösterişli davet ve organizasyon salonudur. En özel günlerinizde yanınızda olmak için buradayız.</p>
  </section>
  <section id="hizmetler">
    <h2>Hizmetlerimiz</h2>
    <ul>
      <li>Düğün Organizasyonları</li>
      <li>Nişan Törenleri</li>
      <li>Doğum Günü Kutlamaları</li>
      <li>Özel Partiler</li>
    </ul>
  </section>
  <section id="galeri">
    <h2>Galeri</h2>
  </section>
  <section id="rezervasyon" class="form-container">
    <h2>Rezervasyon Formu</h2>
    <form id="reservationForm">
      <input type="text" name="isim" placeholder="Adınız Soyadınız" required>
      <input type="tel" name="telefon" placeholder="Telefon Numaranız" required>
      <input type="date" name="tarih" required>
      <textarea name="not" placeholder="Etkinlik hakkında not..." rows="4"></textarea>
      <button type="submit">Gönder</button>
    </form>
  </section>
  <section id="iletisim" class="contact">
    <h2>İletişim</h2>
    <p>Adres: Meydan 54 AVM, Erenler Mahallesi 1193. Sokak No:4/1 B1 Blok, Erenler/Sakarya</p>
    <p>Telefon: <a href="tel:05337100054">0533 710 00 54</a> - <a href="tel:05305945054">0530 594 50 54</a></p>
    <p><a href="https://wa.me/905337100054" target="_blank">WhatsApp ile İletişime Geç</a></p>
  </section>
  <a href="https://wa.me/905337100054" class="whatsapp-button" target="_blank">
    <i class="fab fa-whatsapp"></i>
  </a>
  <footer>
    <p>© 2025 Nora Event | Tüm hakları saklıdır.</p>
  </footer>
  <script>
    document.getElementById('reservationForm').addEventListener('submit', function(e) {
      e.preventDefault();
      var isim = document.querySelector('input[name=isim]').value;
      var telefon = document.querySelector('input[name=telefon]').value;
      var tarih = document.querySelector('input[name=tarih]').value;
      var not = document.querySelector('textarea[name=not]').value;
      var message = 'Merhaba Nora Event,%0AAdım: ' + encodeURIComponent(isim) + '%0ATelefon: ' + encodeURIComponent(telefon) + '%0ATarih: ' + encodeURIComponent(tarih) + '%0ANot: ' + encodeURIComponent(not);
      var whatsappURL = 'https://wa.me/905337100054?text=' + message;
      window.open(whatsappURL, '_blank');
    });
  </script>
</body>
</html>
