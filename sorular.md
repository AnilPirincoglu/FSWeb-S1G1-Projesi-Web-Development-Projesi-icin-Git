# Araştırma Soruları

Artık yeni iş yerindeki ilk görevini gerçekleştirmek için hazırsın! Kullandığımız araçları biraz daha iyi anlama zamanı. Yapman istenilen şey, bu dokümanı güncelleyerek, aşağıdaki soruları soruları cevaplaman. Böylece Git yapısına biraz daha aşina olmaya başlayacaksın.

Soruları cevaplarken takıldığın yerlerde [GitHub docs](https://docs.github.com/en)'u kullanabilirsin. Docs, (ingilizce documentation'ın kısaltılmış halidir) bir programı veya dilin nasıl kullanılacağını anlatan dokümandır. Yazılım dünyasında sıkça kullanılır. Bir yazılımcı olarak _zamanınızın büyük çoğunluğu da bu tarz dokümanları okumakla ve üzerinde çalışmakla geçecek_.

![READ THE DOCS](https://github.com/Workintech/FSWeb-S1G1-Projesi-Web-Development-Projesi-icin-Git/blob/main/read-the-docs-wit.gif?raw=true)

Eğer aradığın soruların cevapları GitHub docs'ta yoksa, Google'lama becerileriniz size yardımcı olacak. Google'ı iyi kullanabilmek de aslında büyük bir dikkat ve çalışma gerektiriyor. Zamanla bu konuda da daha iyileştiğini göreceksin :)

## Sorular

1. Git nedir?

    - Git, yazılım geliştirme süreçlerinde kullanılan bir versiyon kontrol sistemidir. Git sayesinde gerçekleştirme sürecindeki projelerin versiyonlarının kopyalarını alarak daha sonra ihtiyaç halinde istediğiniz kopyalara yani versiyonlara kolayca dönebilirsiniz.

2. Git ile GitHub arasında ne fark var?

    - Git yerel bir versiyon kontrol sistemidir. Açık kaynak kodludur. Temel versiyon kontrol işlemlerini sağlar. Ücretsizdir. GitHub ise bulut tabanlı bir hizmettir. Birçok özellik ücretli abonelik gerektirir dolayısıyla kar amacı güden bir hizmettir. Kod yönetimi ve takım çalışması için gelişmiş özellikler sunar. 

3. Neden bir branch oluşturuyoruz?

    - Branch oluşturulmasının birçok farklı senaryoda çok sayıda farklı sebepleri olabilir. Fakat en temel sebebi halihazırda çalışan ve kullanılan bir uygulamanın geliştirilmesi aşamasında asıl uygulamanın geliştirme sürecinde zarar görmemesi, olumsuz olabilecek sonuçların son kullanıcılara yansımaması ve yazılımın sürekliliğinin zarar görmemesi gibi düşünülebilir. Bunun dışında eklenmek istenilen özelliğin gerçekten uygulanabilir olup olmadığı, tek başına yeterli gelmesi ya da farklı özelliklerinde bu süreçte gerekli görülüp gelişim sürecinin yeni branch ya da brachlar ile devam edecek şekilde yeniden planlanabilmesi de bu sebeplerden bazılarıdır. 

4. Pull Request'in amacı nedir?

    - Geliştirme sürecinde mainden ayrılan branch, geliştirme sürecinin sonunda hedefe ulaştıysa tekrar main branch ile birleştirilerek yeni versiyon oluşturulur. Bu dallanma ve birleştirme kendinize ait bir kodda olabileceği gibi, ekip halinde geliştirdiğiniz bir kodda ya da destek olmak için katıldığınız açık kaynak kodlu bir geliştirme sürecinde de olabilir. ekip olarak çalışılan süreçlerde birleştirme(merge) yapmak istediğiniz branch için bir pull request gönderilir. Böylelikle sizin dışınızdaki geliştiriciler main branchte bir değişiklik olmadan hem sizin kodlarınızı inceleme hem de kendi geliştirdikleri kodlarla karşılaştırma şansı bulurlar. Böylece birleştirme işlemi gerçekleşmeden geliştirlen programda olası bugların ve oluşabilecek sorunların önüne geçilebilir.

5. Bir Branchten diğerine geçmek için kullandığın KOMUT nedir? Mesela `isim-soyisim` branch'inde çalıştığını hayal et ve main branch'ine geçmek istiyorsun, ne yaparsın?

    - Bir branchten diğerine geçmek için "checkout" komutu kullanılır. Farklı bir branchten Main branchine geçmek istendiğinde "Git Bash" terminalinde "git checkout main" komutu çalıştırılarak geçiş sağlanır.
    *bazı geliştirmelerde main yerine master isimlendirmesi kullanılır. Böyle durumlarda main yerine master yazılarak geçiş yapılır.

6. `git fetch`, `git merge` ve `git pull` arasındaki farklıarı açıklayınız. Bu konutlar ne yapar açıklayınız.
    - `git fetch` komutu, yerel deponuzu bilgilerle güncelleyen ve çalışma dosyalarınızın üzerine yazmadan uzak depodan commitleri, dosyaları, referansları indiren bir komuttur. Yerel deponuzu güncel tutmak fakat değişiklik yapma riskine girmek istemediğiniz durumlarda kullanılır. `git merge` komutu ise indirdiğiniz değişikliklerin incelemesini tamamladıktan sonra birleştirme(değişiklikleri uygulama) işlemi için kullanılan bir komuttur. `git pull` komutu önceki iki komutun yaptığı işi tek başına yapar. Yani değişiklikleri yerel deponuza indirir ve yerel deponuzu bu değişikliklere göre günceller.

7. Merge conflict nedir?

    - İki veya daha fazla geliştiricinin aynı dosyada aynı satırı merge etmeye çalışması durumudur.

8. Merge conflict'i nasıl çözeriz?

    - Çakışmaya sebep olan merge işlemlerini geliştiren yazılımcılar, gönderdikleri kodları kontrol ederek ortak bir kod dizini ortaya çıkararak çakışma giderilebilir. Daha büyük çaplı geliştirmelerde kıdemli geliştirici merge edilen kodları kontrol ederek aynı şekilde tek bir kod elde edebilir ya da bütün merge işlemlerini iptal ederek çakışmayı çözebilir.