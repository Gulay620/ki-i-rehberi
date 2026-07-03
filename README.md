# Dijital Adres Defteri Projesi (Angular)

Bu proje, teknik şartnamede belirtilen tüm isterleri karşılayacak şekilde Angular framework'ü kullanılarak geliştirilmiş bir **Dijital Adres Defteri** uygulamasıdır.

## 🚀 Projede Uygulanan Teknik Özellikler
* **State Management (Signals & RxJS):** Uygulama durumu Angular Signals (`signal`, `computed`) ve RxJS `BehaviorSubject` kullanılarak reaktif bir şekilde yönetilmiştir.
* **Reactive Forms & Custom Validator:** Kişi ekleme/düzenleme formları `FormBuilder` ile kurulmuş, Türkiye telefon formatına uygun (`5XXXXXXXXX`) özel bir **`phoneValidator`** yazılmıştır.
* **Unsaved Changes Guard:** Formda değişiklik yapılıp kaydedilmeden sayfadan çıkılmak istendiğinde kullanıcıyı uyaran `CanDeactivateFn` tabanlı bir rota koruyucu (`unsavedChangesGuard`) eklenmiştir.
* **Custom Pipe (Avatar Pipe):** Kişilerin isim ve soyisimlerinin ilk harflerini alarak otomatik profil görseli oluşturan `avatar` pipe'ı yazılmıştır.
* **Veri Kalıcılığı:** Tüm rehber verileri `localStorage` üzerinde saklanmakta, sayfa yenilense bile kaybolmamaktadır.

## 🛠️ Kurulum ve Çalıştırma Adımları

Projeyi kendi yerel ortamınızda çalıştırmak için aşağıdaki adımları sırasıyla uygulayınız:

1. Proje ZIP dosyasını klasöre çıkartın.
2. Klasörün içinde bir terminal (CMD / Powershell) açarak gerekli paketleri yükleyin:
   ```bash
   npm install
