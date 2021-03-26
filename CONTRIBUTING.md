# Katkı

 Katkılarınızı bekliyoruz!  İşte projenin nasıl tasarlandığına dair bazı yönergeler.

 ### CodeStyle

 - PEP8'e mümkün olduğunca bağlı kalın.

 - Satır uzunlukları 120 karakterin altında olmalıdır, harita / filtre üzerinde liste anlayışlarını kullanın, sonunda boşluk bırakmayın.

 - Daha karmaşık kod parçaları, ileride başvurmak üzere yorumlanmalıdır.

 ### Yapı

 Projeyi olabildiğince derli toplu tutmak için proje yapısında kendiliğinden empoze edilen birkaç kural vardır.
 - Tüm modüller "module /" dizinine girmelidir.
 - Herhangi bir veritabanı erişimi "modüller / sql /" içinde yapılmalıdır - hiçbir SESSION örneği başka bir yere aktarılmamalıdır.
 - Veritabanı oturumlarınızın kapsamının uygun şekilde ayarlandığından emin olun!  Her zaman düzgün şekilde kapatın.
 - Yeni bir modül oluştururken, onu dahil etmek için diğer dosyalarda mümkün olduğunca az değişiklik olmalıdır.
 Modül dosyasını kaldırmak, hala mükemmel çalışma durumunda olan bir botla sonuçlanmalıdır.
 - Bir modül, yüklenemeyebilecek birden çok başka dosyaya bağımlıysa, modülde bir liste oluşturun
 özniteliklere bakarak, "__main__" içinde yükleme süresi.  Geçiş, / help, / stats, / info ve diğer pek çok şey bu şekilde
 dayanmaktadır.  Botun LOAD ve NO_LOAD yapılandırmalarıyla sorunsuz çalışmasını sağlar.
 - Bazı şeylerin çakışabileceğini unutmayın;  ör. bir normal ifade işleyicisi bir komut işleyiciyle çakışabilir - bu durumda,
 onları farklı sevk gruplarına koymalısınız.

 Karmaşık görünebilir, ancak içine girdiğinizde mantıklı olacaktır.  Benden yardım / tavsiye istemekten çekinmeyin!

`Thanks for https://github.com/TGExplore/Marie-2.0-English`
