# VestaCP + Nginx + PHP-FPM + SSL + Wordpress Nginx Ayarları
VPS sunucunuza VestaCP ve nginx kurulumu yaptıysanız ve wordpress kulllanıyorsanız bir takım ayarlamalar yapmak gerekiyor. Wordpress kullanıp üstüne bir de SSL kullanmak istiyorsanız bu paylaştığım nginx.conf dosyası işinizi görecektir. 

Wordpress'in kalıcı bağlantı ayarları bir bakıma self-url yapısı ve SSL için'de gerekli ayarlar dosyada mevcuttur.

Wordpress için önerilen ve ideal optimasyon ayarlamalarıda yapılmış vaziyettedir. İhtiyacınıza göre düzenlemeler yapabilirsiniz.

# VestaCP nginx.conf dizini 
VestaCP'de 2 adet nginx.conf dosyası mevcut fakat bu 2 dosyadan bir tanesi çalışmakta diğeri vestacp için ayarlar içeriyor. Bu paylaştığım dosyayı aşağıda belirttiğim dizine yükleyeceksiniz ve varolan dosyayı silmeniz gerekiyor.

<strong>/home/admin/conf/web</strong> Bu dizine yükledikten sonra aşağıda ki işlemleri yapmanız gerekiyor.

# Nginx'i Yeniden Derleme ve Yapılan Ayarlamaları Aktif Hale Getirme

<code>nginx -t </code>
Bu komut yapmış olduğunuz nginx.conf dosyasında hata olup olmadığını kontrol eden linux komutudur. Ve bu komutu girdiğinizde size syntax ok mesajını döndürüyorsa nginx.conf dosyasınız hatasız demektir. Eğer bu sonucu döndürmüyorsa size hatalı kısımları SSH ekranında size göstermektedir.

Hata yok ise aşağıda ki işlemi gerçekleştirin.

<code>service nginx stop</code>
<code>service nginx start</code>

Hepsi bu kadar kolay gelsin.

# Detaylı bilgi ve Demo Adres

https://huseyinkorbalta.com
