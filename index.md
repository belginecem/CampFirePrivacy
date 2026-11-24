# Kamp Ateşi — Gizlilik Politikası

_Son güncelleme: 24 Kasım 2026_

Kamp Ateşi ("uygulama"), küçük grupların ortak görev listeleri ve bir duyuru panosu paylaşması için
geliştirilmiş bir mobil uygulamadır. Bu politika hangi verileri topladığımızı, nasıl kullandığımızı ve
haklarını açıklar.

## Topladığımız veriler

| Veri | Neden |
| --- | --- |
| E-posta adresi ve şifre (e-postayla kaydolursan) | Hesap oluşturma ve giriş. Şifre yalnızca Firebase Authentication tarafından şifrelenmiş olarak saklanır; biz göremeyiz. |
| Apple veya Google hesabından gelen ad, e-posta ve hesap kimliği (bu yöntemlerle girersen) | Hesap oluşturma ve giriş. Apple'da e-postanı gizlersen bize yalnızca Apple'ın verdiği yönlendirme adresi gelir. Apple veya Google şifreni hiçbir zaman görmeyiz. |
| Görünen ad | Kamp üyelerine kimin ne eklediğini göstermek. |
| Kamp içeriği (görev listeleri, görevler, son tarihler, atamalar, duyurular, emoji tepkileri) | Uygulamanın temel işlevi: kamp üyeleriyle gerçek zamanlı paylaşım. |
| Karakter bilgileri (XP, tamamlanan görev sayısı, avatar seçimleri) | Seviyeni ve karakterini sana ve kamp üyelerine göstermek. |
| Kamp üyeliği ve davet kodu | Kimin hangi kampa erişebileceğini belirlemek. |
| Push bildirim jetonu (izin verirsen) | Kampta görev eklendiğinde, tamamlandığında veya sana atandığında ve yeni duyuru paylaşıldığında bildirim göndermek. |

Konum, rehber, fotoğraf, reklam kimliği veya cihaz takibi verisi **toplamıyoruz**. Uygulamada reklam,
analitik veya üçüncü taraf takip aracı **yoktur**. Verilerin satılmaz ve reklam amacıyla kullanılmaz.

## Verileri kimler görebilir

- Kamp içeriğini, görünen adını, e-postanı ve karakter bilgilerini yalnızca **aynı kamptaki üyeler** (en fazla 5 kişi) görür.
  Bu erişim Firestore güvenlik kurallarıyla sunucu tarafında zorunlu kılınır.
- Kampa katılmak için davet kodu gerekir; kamp dışındaki kişiler içeriği okuyamaz.

## Cihazında tutulanlar

- Uygulama internetsiz de açılabilsin diye profilinin ve kampının son hali ile henüz gönderilmemiş
  değişikliklerin telefonunda saklanır. Çıkış yaptığında veya hesabını sildiğinde bunlar cihazdan silinir.
- Son tarih hatırlatmaları telefonun kendisi tarafından kurulur; bunun için bir sunucuya veri gönderilmez.

## Hizmet sağlayıcılar

- **Google Firebase** (Authentication ve Cloud Firestore): hesap ve kamp verilerini saklar.
  Veriler Google'ın sunucularında, Türkiye dışında işlenebilir.
  [Firebase gizlilik bilgisi](https://firebase.google.com/support/privacy)
- **Apple ile Giriş** ve **Google ile Giriş**: yalnızca bu yöntemi seçersen kimliğini doğrulamak için
  kullanılır. [Apple gizlilik politikası](https://www.apple.com/legal/privacy/) ·
  [Google gizlilik politikası](https://policies.google.com/privacy)
- **Apple App Store**: iPhone'da uygulamanın yeni sürümü olup olmadığını sormak için Apple'ın herkese
  açık adresine istek gönderilir; bu istekte hesap bilgin yer almaz.
- **Expo Push Notification Service** (Expo / 650 Industries): bildirimleri Apple ve Google'ın bildirim
  hizmetlerine iletir. Bildirim jetonu ile bildirim başlığı ve metni bu hizmetten geçer.
  [Expo gizlilik politikası](https://expo.dev/privacy)

## Saklama süresi ve silme

Veriler hesabın açık olduğu sürece saklanır. Hesabını istediğin zaman uygulama içinden silebilirsin:
**Karakter → sağ üstteki hesap silme simgesi**. Silme işlemi:

- Firebase hesabını ve profilini (görünen ad, e-posta, bildirim jetonu, XP, avatar) kalıcı olarak siler,
- Apple ile girdiysen uygulamanın Apple hesabına erişiminin iptalini ister,
- paylaştığın duyuruları siler,
- seni kamptan çıkarır; kamp lideriysen liderlik başka bir üyeye geçer.

Eklediğin görevler kampın ortak içeriği olduğu için diğer üyelerde kalır; bu görevlerde
adın değil, yalnızca anlamsız bir kullanıcı kimliği tutulur. Kampın son üyesi ayrıldığında kampa artık
kimse erişemez.

Çıkış yaptığında bildirim jetonun silinir ve o cihaza bildirim gönderilmez. İnternetsizken çıkış yaparsan
jeton o anda silinemeyebilir; tekrar giriş yapıp internet varken çıkman yeterlidir.

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

_Last updated: November 24, 2026_

- **Collected:** email and password (for sign-in, handled by Firebase Authentication) or, if you sign in
  with Apple or Google, the name, email and account identifier they provide; display name; camp content you
  create (lists, tasks, due dates, assignments, notes, reactions); camp membership; character data (XP,
  completed task count, avatar choices); and, if you allow notifications, an Expo push token.
- **On your device:** the latest copy of your profile and camp and any unsent changes, so the app works
  offline. Removed when you sign out or delete your account.
- **Not collected:** location, contacts, photos, advertising identifiers. No ads, no analytics, no
  tracking. Data is never sold.
- **Visibility:** only members of the same camp (max. 5) can see your camp content, name, email and character;
  this is enforced by Firestore security rules.
- **Processors:** Google Firebase (storage and authentication), Apple and Google (only if you use their
  sign-in), Expo Push Notification Service (delivery of notifications). On iPhone the app also asks Apple's
  public App Store address whether a newer version exists; no account data is sent.
- **Deletion:** delete your account anytime in the app with the delete icon at the top right
  of **Karakter**. This deletes your account and profile, removes your notes, takes you out of your camp and,
  for Apple accounts, requests that the app's access be revoked.
- **Children:** not directed at children under 13.
- **Contact:** Ecemnur Belgin — belginecem@gmail.com
