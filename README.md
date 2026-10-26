# Prompter (TV ekranı için)

Sahnedeki konuşmacının metnini bir TV'den okuyabilmesi için tek dosyalık bir uygulama. İnternet gerekmez; kurulum yok.
(src: Claude, 2026-10-26 — tasarım: claude.ai "TV Prompter" canvas'ı, https://claude.ai/artifact/JZj8uhyYcXLT5c4dJEZTie)

## Açmak
- `prompter.html` dosyasına çift tıklayın. En iyi sonuç için **Chrome** ya da **Edge** kullanın.
- `fonts/` klasörü dosyanın yanında durmalı (Paribu yazı tipi). Yoksa sistem yazı tipine düşer, uygulama yine çalışır.

## İki ekranla kullanım (dizüstü + TV)
1. TV'yi HDMI ile bağlayın ve ekranı **genişletin** (yansıtma değil).
2. `prompter.html`'i açın, metni yapıştırın ya da **Metni içe aktar** ile .txt yükleyin (dosyayı metin alanına sürüklemek de olur).
3. **TV penceresini aç**'a basın. Chrome/Edge izin isterse verin: pencere doğrudan TV'de açılır. Açılmazsa pencereyi TV'ye sürükleyin.
4. TV penceresinde **Tam ekran için tıklayın** yazısına bir kez tıklayın (ya da `F`).
5. Dizüstündeki panelden yönetin: metin, hız, yazı boyutu, okuma çizgisi, metin genişliği, ayna ve zamanlayıcı TV'ye anında gider.

Tek ekran (ya da yansıtma) ile: **Bu pencerede TV** düğmesi aynı pencereyi TV görünümüne çevirir; `Esc` ile panele dönülür.

## Kısayollar
| Tuş | İş |
|---|---|
| Boşluk | Başlat / duraklat |
| ↑ / ↓ | Bir satır geri / ileri |
| Page Up / Page Down | Paragraf geri / ileri — sunum kumandaları (clicker) bu tuşları gönderir |
| + / − | Hızlandır / yavaşlat |
| R | Başa dön |
| M | Ayna |
| F | Tam ekran (TV görünümünde) |

Önizleme ve TV ekranı fare tekerleği ya da sürükleme ile de kaydırılır; akış açıksa metin yeni konumdan devam eder.

## Metin biçimi
- Paragrafları boş satırla ayırın.
- Tek başına `[ ... ]` içindeki paragraf TV'de yeşil işaret olarak görünür, ör. `[Duraklat]`, `[Kameraya bak]`.

## Notlar
- Metin ve ayarlar tarayıcıda hatırlanır (aynı bilgisayar + aynı tarayıcı). Gösteriden önce **Metni kaydet** ile .txt yedeği alın.
- Zamanlayıcı yalnızca metin akarken ilerler. Geri sayımda son 30 saniyede sarı, süre aşılınca kırmızı olur.
- Panel ile TV penceresi arasındaki bağ, panelden açılan pencerede her tarayıcıda çalışır. Elle açılan ikinci pencere (`prompter.html#tv`) ancak tarayıcı izin verirse eşitlenir; Chrome'da `file://` için bu doğrulanmadı ❓ — sorun olursa TV penceresini hep paneldeki düğmeyle açın.
