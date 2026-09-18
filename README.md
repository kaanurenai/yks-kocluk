# YKS Bilgi ve Güven Çalışma Paneli

Tarayıcıda çalışan, kurulum gerektirmeyen YKS çalışma ve YOP takip panelidir.

## GitHub ve Vercel kurulumu

1. ZIP dosyasını çıkarın.
2. İçindeki dosyaları yeni bir GitHub deposunun kök dizinine yükleyin.
3. Vercel'de **Add New → Project** seçeneğine girin.
4. GitHub deposunu seçip **Deploy** düğmesine basın.

Framework seçmeniz veya build komutu girmeniz gerekmez.

## AI deneme analizi kurulumu

Deneme kitapçığı ve fotoğraf/PDF analizinin çalışması için Vercel projesinde:

1. **Settings → Environment Variables** bölümünü açın.
2. `OPENAI_API_KEY` adında bir değişken oluşturup OpenAI API anahtarını girin.
3. İsterseniz `OPENAI_MODEL` değişkeniyle modeli değiştirebilirsiniz. Varsayılan model `gpt-4.1`'dir.
4. Projeyi yeniden deploy edin.

API anahtarını `index.html`, GitHub veya başka bir herkese açık dosyaya yazmayın.

## Veri saklama

Deneme analizinde üç giriş yöntemi vardır: hazır analiz raporu yükleme, deneme kitapçığı yükleme ve dosyasız manuel giriş. Manuel girişte TYT/AYT branşları ve konuları hazır gelir; her konu için toplam soru, doğru, yanlış ve boş adetleri girilir, sıfır bırakılan konular kayda alınmaz. Çalışma ve deneme kayıtları tarayıcının yerel depolama alanında saklanır. Farklı cihaz veya tarayıcıda kayıtlar otomatik olarak taşınmaz. Yüklenen dosyalar tarayıcıda saklanmaz. Paneldeki JSON yedekleme özelliğiyle çalışma kayıtlarının yedeği alınabilir.
