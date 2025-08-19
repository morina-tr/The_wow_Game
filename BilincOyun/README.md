# 3D FPS Game with ESP & Aimbot

Gelişmiş 3D First Person Shooter (FPS) oyunu - React Three Fiber ve TypeScript ile geliştirilmiş, ESP (duvar hack) ve aimbot özellikleri içeren eğitici C++ programlama oyunu.

## 🎮 Özellikler

### Gelişmiş FPS Mekaniği
- **Birinci Şahıs Görünüm** - Gerçekçi FPS kontrolleri
- **4 Farklı Silah** - Tabanca, Tüfek, Sniper, Shotgun
- **Fizik Sistemi** - Gerçekçi hareket ve çarpışma
- **Atmosferik Grafikler** - Sis, gölge ve ışıklandırma

### Hack Özellikleri
- **ESP (Wall Hack)** - Düşmanları duvarların arkasından görme
- **Aimbot** - Otomatik nişan alma sistemi
- **Mesafe Göstergesi** - En yakın düşman bilgisi
- **Gelişmiş UI** - Gerçek zamanlı oyun bilgileri

### Zeki AI Sistemi
- **Gemini AI Entegrasyonu** - Düşman AI davranışları
- **Taktiksel Hareket** - Saldırı, savunma, çevirme, geri çekilme
- **Dinamik Düşman Saldırıları** - Mesafe bazlı hasar sistemi

### Eğitim İçeriği
- **C++ İpuçları** - Her level sonunda programlama tavsiyeleri
- **Interaktif Öğrenme** - Oyun içi eğitim modalları

## 🕹️ Kontroller

| Tuş | Fonksiyon |
|-----|-----------|
| `WASD` | Hareket |
| `Mouse` | Bakış yönü |
| `Sol Tık` | Ateş etme |
| `Q` | Aimbot açma/kapama |
| `E` | ESP açma/kapama |
| `1/2/3/4` | Silah değiştirme |
| `R` | Mermi doldurma |
| `Space` | Zıplama |
| `T` | Oyunu yeniden başlatma |

## 🛠️ Teknoloji Stack

### Frontend
- **React 18** - UI framework
- **TypeScript** - Type safety
- **React Three Fiber** - 3D graphics
- **@react-three/drei** - 3D utilities
- **Zustand** - State management
- **Tailwind CSS** - Styling
- **Radix UI** - Component library

### Backend
- **Express.js** - Web server
- **TypeScript** - Server-side types
- **PostgreSQL** - Database
- **Drizzle ORM** - Database operations

### AI & APIs
- **Google Gemini API** - AI düşman davranışları ve C++ eğitim içeriği

### 3D & Graphics
- **Three.js** - WebGL rendering
- **Post-processing** - Visual effects
- **Shadow mapping** - Realistic shadows
- **Fog effects** - Atmospheric rendering

## 🚀 Kurulum

### Gereksinimler
- Node.js 18+
- PostgreSQL database
- Gemini API key

### Adımlar

1. **Repository'yi klonlayın**
```bash
git clone https://github.com/[kullanici-adi]/3d-fps-game.git
cd 3d-fps-game
```

2. **Bağımlılıkları yükleyin**
```bash
npm install
```

3. **Environment değişkenlerini ayarlayın**
```bash
# .env dosyası oluşturun
VITE_GEMINI_API_KEY=your_gemini_api_key_here
DATABASE_URL=your_postgresql_url
```

4. **Veritabanını hazırlayın**
```bash
npm run db:generate
npm run db:migrate
```

5. **Geliştirme sunucusunu başlatın**
```bash
npm run dev
```

Oyun `http://localhost:5000` adresinde çalışacak.

## 🎯 Oynanış

1. **Oyunu Başlatın** - Sayfaya tıklayarak pointer lock'u etkinleştirin
2. **ESP'yi Açın** - `E` tuşuna basarak düşmanları duvar arkasından görün
3. **Aimbot'u Kullanın** - `Q` tuşuna basarak otomatik nişan alın
4. **Silah Değiştirin** - `1-4` tuşlarıyla farklı silahlar deneyin
5. **Düşmanları Eleyip** - Level'ları tamamlayarak C++ öğrenin

## 🏗️ Proje Yapısı

```
├── client/                 # Frontend React uygulaması
│   ├── src/
│   │   ├── components/     # 3D ve UI componentleri
│   │   ├── lib/           # Utilities ve stores
│   │   └── pages/         # Sayfa componentleri
├── server/                # Backend Express sunucusu
├── shared/                # Ortak TypeScript tipleri
└── docs/                  # Dokümantasyon
```

## 🔧 Geliştirme

### Yeni Silah Ekleme
```typescript
// useFPSGame.tsx içinde weapon tipini genişletin
weaponType: 'pistol' | 'rifle' | 'sniper' | 'shotgun' | 'newWeapon'

// Weapon.tsx içinde yeni silah modelini ekleyin
case 'newWeapon':
  return <WeaponModel />
```

### AI Davranışı Geliştirme
```typescript
// geminiAI.ts içinde yeni davranış türleri ekleyin
type AIBehavior = 'attack' | 'retreat' | 'flank' | 'defend' | 'newBehavior'
```

## 📊 Performans

- **60 FPS** - Smooth gameplay
- **WebGL optimization** - Efficient 3D rendering
- **LOD system** - Distance-based detail
- **Instanced rendering** - Multiple objects optimization

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/AmazingFeature`)
3. Commit yapın (`git commit -m 'Add some AmazingFeature'`)
4. Branch'e push yapın (`git push origin feature/AmazingFeature`)
5. Pull Request oluşturun

## 📝 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 🎓 Eğitim Amaçlı

Bu oyun C++ programlama öğrenmek isteyenler için eğitici içerikler sunar:
- Algoritma mantığı
- Performans optimizasyonu
- Bellek yönetimi
- Oyun geliştirme prensipleri

## 🙏 Teşekkürler

- React Three Fiber topluluğu
- Three.js geliştiricileri
- Google Gemini AI ekibi
- Açık kaynak katkıda bulunanlar

---

**Not**: Bu oyun eğitim amaçlıdır. Gerçek FPS oyunlarında hile kullanımı etik değildir.