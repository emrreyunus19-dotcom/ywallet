# 💰 Tron Wallet Dashboard

Kişisel kullanım için tasarlanmış, özel bir web tabanlı Tron (TRC-20) Cüzdan Panosu.

## 🚀 Özellikler

✅ **Kimlik Doğrulama**: Kodlanmış kimlik bilgileri ile güvenli giriş  
✅ **Tek Tık Cüzdan Oluşturma**: Anında yeni Tron cüzdanı oluşturma  
✅ **Bakiye Takibi**: TRX ve USDT (TRC-20) bakiyelerini gerçek zamanlı görüntüleme  
✅ **QR Kodu**: Hızlı para gönderimi için QR kod oluşturma ve indirme  
✅ **Fon Transferi**: TRX ve USDT gönderi fonksiyonu  
✅ **Duyarlı Tasarım**: Desktop ve mobil cihazlarda mükemmel deneyim  

## 🛠 Tech Stack

**Frontend:**
- React 18
- TypeScript
- Tailwind CSS
- Zustand (State Management)
- Vite
- QRCode.react

**Backend:**
- Node.js
- Express.js
- TypeScript
- TronWeb (Tron SDK)

## 📋 Gereksinimler

- Node.js v18+
- npm veya yarn

## ⚡ Hızlı Başlangıç

### 1. Projeyi Klonlayın

```bash
git clone https://github.com/emrreyunus19-dotcom/ywallet.git
cd ywallet
git checkout feature/tron-wallet-dashboard
```

### 2. Backend Kurulumu

```bash
cd backend
npm install
cp .env.example .env
```

`.env` dosyasını düzenleyin:
```env
PORT=5000
ADMIN_USERNAME=admin
ADMIN_PASSWORD=YourSecurePassword123!
AUTH_TOKEN=your-secret-jwt-token-here
```

Backend'i başlatın:
```bash
npm run dev
```

### 3. Frontend Kurulumu

```bash
cd ../frontend
npm install
cp .env.local.example .env.local
```

Frontend'i başlatın:
```bash
npm run dev
```

**Tarayıcıda açın:** http://localhost:5173

## 🔐 Login Bilgileri

```
Kullanıcı Adı: admin
Şifre: YourSecurePassword123!
```

## 📱 Kullanım

1. **Giriş Yapın**: Kimlik bilgilerinizi girin
2. **Cüzdan Oluşturun**: "Generate New Wallet" butonuna tıklayın
3. **Bakiyeyi Kontrol Edin**: TRX ve USDT bakiyelerini görüntüleyin
4. **Para Gönderin**: "Send Funds" formunu kullanarak transfer yapın
5. **QR Kodu Kullanın**: "Receive TRX" kısmından QR kodunu indirin

## 🔒 Güvenlik Bilgileri

- Private Key'ler bellekte depolanır, sunucuya gönderilmez
- Tüm işlemler localStorage'da saklanmaz
- .env dosyasında hassas bilgileri tutun
- Production'da HTTPS kullanın

## 📚 Proje Yapısı

```
ywallet/
├── backend/
│   ├── src/
│   │   ├── server.ts
│   │   ├── middleware/auth.ts
│   │   ├── services/tronService.ts
│   │   └── routes/tron.ts
│   ├── package.json
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── stores/
│   │   ├── services/
│   │   ├── types/
│   │   └── App.tsx
│   ├── package.json
│   └── .env.local
└── README.md
```

## 🚢 Production Deploy

### Docker ile Deploy

```bash
docker-compose up --build
```

### Build Etme

```bash
# Backend
cd backend
npm run build

# Frontend
cd frontend
npm run build
```

## 🐛 Sorun Giderme

**Port zaten kullanılıyorsa:**
```bash
# Farklı port kullanın
PORT=5001 npm run dev
```

**Module bulunamadı hatası:**
```bash
npm install
```

**Tron API bağlantısı başarısız:**
- `.env` dosyasında Tron ağını kontrol edin
- VPN kullanıyorsanız, API endpoint'leri değişebilir

## 📝 Lisans

Private use only - Kişisel kullanım için

## 👨‍💻 Geliştirici

emrreyunus19-dotcom

---

**⚠️ Uyarı**: Private Key'leriniz asla kimseyle paylaşmayın!
