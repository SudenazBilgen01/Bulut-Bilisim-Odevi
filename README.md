# Bulut-Bilisim-Odevi

## 1. GİRİŞ

Bulut bilişim, bilişim kaynaklarının internet üzerinden esnek, ölçeklenebilir ve isteğe bağlı olarak sunulmasını sağlayan bir teknolojidir. Günümüzde uygulamaların fiziksel sunucular yerine bulut ortamlarında çalıştırılması, maliyet, erişilebilirlik ve yönetim açısından önemli avantajlar sağlamaktadır.

Bu projede, bulut bilişim kavramlarının anlaşılması amacıyla basit bir web uygulamasının Amazon Web Services (AWS) bulut platformu üzerinde dağıtımı gerçekleştirilmiştir. Projede, uygulama karmaşıklığından ziyade bulut ortamında uygulama dağıtım sürecinin doğru ve eksiksiz şekilde uygulanması hedeflenmiştir.

## 2. PROJENİN AMACI VE HEDEFLERİ

Bu projenin temel amaçları aşağıda listelenmiştir:

-Bir bulut servis sağlayıcısı üzerinde sanal sunucu oluşturmak

-Güvenlik ve ağ yapılandırmalarını gerçekleştirmek

-Basit bir web uygulamasını bulut ortamına taşımak

-Uygulamayı internet üzerinden erişilebilir hale getirmek

-Dağıtım sürecini rapor ve sunum ile belgelemek

## 3. UYGULAMA SEÇİMİ

Projede, HTML tabanlı basit bir web uygulaması (Hello World) tercih edilmiştir.

Bu uygulamanın seçilme nedenleri:

-Bulut ortamında dağıtım sürecine odaklanabilmek

-Ekstra backend veya veritabanı gereksinimi olmaması

-Kurulum ve yapılandırma adımlarının net şekilde gösterilebilmesi

Bu doğrultuda, uygulama içeriği bilinçli olarak basit tutulmuş, asıl vurgu bulut altyapısının doğru şekilde yapılandırılmasına verilmiştir.

## 4. BULUT PLATFORMU SEÇİMİ

Proje kapsamında Amazon Web Services (AWS) platformu kullanılmıştır.

AWS’nin tercih edilme nedenleri:

-Yaygın kullanım ve endüstri standardı olması

-Geniş servis çeşitliliği

-Öğrenciler için ücretsiz (Free Tier) kaynaklar sunması

-Uygulama dağıtımı için AWS EC2 (Elastic Compute Cloud) servisi kullanılmıştır.

## 5. KULLANILAN TEKNOLOJİLER

Amazon Web Services (AWS)

EC2 (Elastic Compute Cloud)

Amazon Linux 2023

Apache Web Server

HTML

SSH (Secure Shell)

## 6. UYGULAMA MİMARİSİ

Uygulama mimarisi basit ve anlaşılır bir yapıdadır:

Kullanıcı (Web Tarayıcı)
        |
        v
İnternet
        |
        v
AWS EC2 Sanal Sunucu
        |
        v
Apache Web Server
        |
        v
HTML Web Sayfası

## 7. DAĞITIM SÜRECİ (ADIM ADIM)
### 7.1 EC2 Sanal Sunucu Oluşturulması

AWS Management Console üzerinden EC2 servisine erişildi

Amazon Linux 2023 işletim sistemi seçildi

Free Tier uyumlu sanal sunucu oluşturuldu

### 7.2 Ağ ve Güvenlik Yapılandırması

Otomatik public IP atanması etkinleştirildi

Güvenlik grubu ayarlarında aşağıdaki portlar açıldı:

SSH (22)

HTTP (80)

HTTPS (443)

### 7.3 Sunucuya Bağlantı

EC2 Instance Connect kullanılarak sunucuya SSH bağlantısı sağlandı

### 7.4 Web Server Kurulumu

Apache Web Server kuruldu

Servis başlatıldı ve otomatik çalışacak şekilde ayarlandı

### 7.5 Uygulamanın Yayınlanması

HTML tabanlı web sayfası oluşturuldu

Dosya /var/www/html dizinine yerleştirildi

Tarayıcı üzerinden public IP adresi ile erişim sağlandı

## 8. KARŞILAŞILAN ZORLUKLAR VE ÇÖZÜMLER

Proje sırasında başlangıçta web sayfasına dış erişim sağlanamamıştır. Yapılan kontroller sonucunda Apache servis durumu ve güvenlik ayarları incelenmiş, gerekli düzenlemeler yapılarak sorun giderilmiştir.

Bu süreç, bulut ortamlarında servis durumu ve ağ yapılandırmasının ne kadar kritik olduğunu göstermiştir.

## 9. ÖĞRENİLEN DERSLER VE OLASI İYİLEŞTİRMELER

Bu proje sayesinde:

Bulut ortamında sanal sunucu oluşturma süreci öğrenilmiştir

Güvenlik grubu ve ağ yapılandırmalarının önemi anlaşılmıştır

Basit bir uygulamanın internet üzerinden yayınlanma süreci deneyimlenmiştir

Gelecekteki çalışmalarda:

HTTPS yapılandırması yapılabilir

Docker veya otomasyon araçları kullanılabilir

Daha kapsamlı uygulamalar dağıtılabilir

## 10. SONUÇ

Bu projede, basit bir web uygulaması AWS bulut platformu üzerinde başarıyla dağıtılmış ve internet üzerinden erişilebilir hale getirilmiştir. Proje, bulut bilişimin temel prensiplerini anlamak ve uygulamalı olarak deneyimlemek açısından başarılı bir çalışma olmuştur.
