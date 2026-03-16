# 📱 Kalite Checker - APK Yapma Rehberi

## ⚡ Hızlı Özet
Bu klasörü GitHub'a yükleyin → GitHub otomatik APK yapar → İndirin!

---

## 📋 Adım Adım

### 1. GitHub'a Yükleyin
1. GitHub.com'a gidin → "New repository" → isim verin (örn: `kalite-apk`)
2. **Public** seçin → "Create repository"
3. Bu klasördeki TÜM dosyaları GitHub'a yükleyin:
   - Yeşil "Add file" → "Upload files" tıklayın
   - `.github` klasörü dahil HER ŞEYİ sürükleyip bırakın
   - "Commit changes" tıklayın

### 2. APK Otomatik Build Olur
- Yükleme biter bitmez GitHub otomatik APK yapmaya başlar
- Sağ üstte **"Actions"** sekmesine tıklayın
- Sarı daire → yeşil tik olunca bitti demektir ✅ (5-10 dakika sürer)

### 3. APK'yı İndirin
1. Actions → En son "Build APK" workflow'a tıklayın
2. Aşağıda **"Artifacts"** bölümünde `Kalite-Checker-APK` var
3. Tıklayın ve indirin!

---

## 🔧 Port Ayarı
Uygulamanız Termux'ta farklı bir portta çalışıyorsa:

`android-webview/app/src/main/java/com/kalitechecker/app/MainActivity.java` dosyasını açın:

```java
private static final String APP_URL = "http://localhost:5000";
```

`5000` yerine kendi port numaranızı yazın.

---

## ⚠️ Önemli Notlar
- APK'yı kurmadan önce tablette **"Bilinmeyen kaynaklara izin ver"** açın
- Uygulamayı açmadan önce **Termux'ta projenizi başlatın**
- APK sadece Termux çalışırken düzgün açılır
