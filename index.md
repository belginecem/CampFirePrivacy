# Kamp Ateşi — Gizlilik Politikası

_Son güncelleme: 19 Kasım 2026_

Kamp Ateşi ("uygulama"), küçük grupların ortak görev listeleri ve bir duyuru panosu paylaşması için
geliştirilmiş bir mobil uygulamadır. Bu politika hangi verileri topladığımızı, nasıl kullandığımızı ve
haklarını açıklar.

## Topladığımız veriler

| Veri | Neden |
| --- | --- |
| E-posta adresi ve şifre | Hesap oluşturma ve giriş. Şifre yalnızca Firebase Authentication tarafından şifrelenmiş olarak saklanır; biz göremeyiz. |
| Görünen ad | Kamp yoldaşlarına kimin ne eklediğini göstermek. |
| Kamp içeriği (görev listeleri, maddeler, duyurular, emoji tepkileri) | Uygulamanın temel işlevi: kamp üyeleriyle gerçek zamanlı paylaşım. |
| Kamp üyeliği ve davet kodu | Kimin hangi kampa erişebileceğini belirlemek. |
| Push bildirim jetonu (izin verirsen) | Kamp yoldaşların yeni görev veya duyuru eklediğinde sana bildirim göndermek. |

Konum, rehber, fotoğraf, reklam kimliği veya cihaz takibi verisi **toplamıyoruz**. Uygulamada reklam,
analitik veya üçüncü taraf takip aracı **yoktur**. Verilerin satılmaz ve reklam amacıyla kullanılmaz.

## Verileri kimler görebilir

- Kamp içeriğini ve görünen adını, e-postanı yalnızca **aynı kamptaki üyeler** (en fazla 5 kişi) görür.
  Bu erişim Firestore güvenlik kurallarıyla sunucu tarafında zorunlu kılınır.
- Kampa katılmak için davet kodu gerekir; kamp dışındaki kişiler içeriği okuyamaz.

## Hizmet sağlayıcılar

- **Google Firebase** (Authentication ve Cloud Firestore): hesap ve kamp verilerini saklar.
  Veriler Google'ın sunucularında, Türkiye dışında işlenebilir.
  [Firebase gizlilik bilgisi](https://firebase.google.com/support/privacy)
- **Expo Push Notification Service** (Expo / 650 Industries): bildirimleri Apple Push Notification
  service'e iletir. Bildirim jetonu ile bildirim başlığı ve metni bu hizmetten geçer.
  [Expo gizlilik politikası](https://expo.dev/privacy)

## Saklama süresi ve silme

Veriler hesabın açık olduğu sürece saklanır. Hesabını istediğin zaman uygulama içinden silebilirsin:
**Kamp → Hesabımı Sil**. Silme işlemi:

- Firebase hesabını ve profilini (görünen ad, e-posta, bildirim jetonu) kalıcı olarak siler,
- panoya astığın duyuruları siler,
- seni kamptan çıkarır; kamp lideriysen liderlik başka bir üyeye geçer.

Eklediğin görev listesi maddeleri kampın ortak içeriği olduğu için diğer üyelerde kalır; bu maddelerde
adın değil, yalnızca anlamsız bir kullanıcı kimliği tutulur. Kampın son üyesi ayrıldığında kampa artık
kimse erişemez.

Çıkış yaptığında bildirim jetonun silinir ve o cihaza bildirim gönderilmez.

## Çocuklar

Uygulama 13 yaşın altındaki çocuklara yönelik değildir ve bu yaş grubundan bilerek veri toplamaz.

## Hakların

6698 sayılı KVKK ve geçerli diğer mevzuat kapsamında verilerine erişme, düzeltme ve silinmesini isteme
hakkın vardır. Verilerinin çoğunu uygulama içinden görebilir ve hesabını silebilirsin. Diğer talepler için bize yaz.

## Değişiklikler

Bu politikayı güncellersek bu sayfadaki tarihi değiştiririz. Önemli değişiklikleri uygulama içinde
duyururuz.

## İletişim

Ecemnur Belgin — belginecem@gmail.com

---

# Kamp Ateşi — Privacy Policy (English summary)

_Last updated: November 19, 2026_

- **Collected:** email and password (for sign-in, handled by Firebase Authentication), display name,
  camp content you create (lists, items, notes, reactions), camp membership, and, if you allow
  notifications, an Expo push token.
- **Not collected:** location, contacts, photos, advertising identifiers. No ads, no analytics, no
  tracking. Data is never sold.
- **Visibility:** only members of the same camp (max. 5) can see your camp content, name and email;
  this is enforced by Firestore security rules.
- **Processors:** Google Firebase (storage and authentication) and Expo Push Notification Service
  (delivery of notifications).
- **Deletion:** delete your account anytime in the app under **Kamp → Hesabımı Sil**. This deletes
  your account and profile, removes your notes and takes you out of your camp.
- **Children:** not directed at children under 13.
- **Contact:** Ecemnur Belgin — belginecem@gmail.com
