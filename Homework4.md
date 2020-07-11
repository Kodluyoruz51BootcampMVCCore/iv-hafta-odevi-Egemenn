Geri dönen bilgiye göre yeşil renkte onay mesajı gösterilmesi. (örneğin:view bag)

-ASP.NET MVC ViewBag, Controller sınıfları ve View sayfaları arasında veri taşımamıza yardımcı olacak nesneler vardır. Bunlardan en önemlisi ViewData, ViewBag ve TempData nesneleridir. ViewBag, Controller'da oluşturulan bir yapıyı View kısmına taşımak için kullanılır. Kendi içerisinde birden fazla yapının aktarılmasına olanak sunmaktadır. İçerisine bir string ifade, integer ifade yada list gönderebilmek ya da eşitleyebilmek mümkündür.

AddMVC - AddMVCCore - AddDateAnnotations nedir? Nerelerde eklenmelidir?

-Startup sınıfının ConfigureServices() öğesinde bu iki yöntem (AddMvc() ve AddMvcCore()) kullanılmaktadır .ConfigureServices() yöntemine gidildiğinde IServiceCollection-AddMvc() ve AddMvcCore()'de iki yöntem bulunur.AddMvcCore(), adından da anlaşılacağı gibi, MVC pipeline'ın yalnızca core bileşenlerini ve projeniz için gerekli başka bir ara katman eklemenizi gerektirir. AddMvc(), AddMvcCore() öğesini çağırır ve razor view motoru gibi diğer ara katman yazılımlarını ekler.

Shanpshot nedir? nasıl değişir? neden alınır?

-Aslında sanallaştırma ortamını kullanan birçok kişi snapshot'ı aktif olarak kullanıyor. Ben bu yazımda Snapshot kavramını biraz daha detaylı olarak anlatacağım çünkü hala snapshot'ı backup gibi kullanılıyor.

Basit olarak açıklamak gerekirse, snapshot'ı kısa süreli çalışmalar öncesinde backup almak yerine snapshot'ı kullanabiliriz. Snapshot sayesinde sanal makinamızın anlık ekran görüntüsü alınır ve siz herhangi bir sebepten dolayı sanal makina üzerinde yaptığınız işlemleri geri almak istediğinizde almış olduğunuz snapshot'a revert diyerek eski haline geri dönüş yapabilirsiniz.

Snapshot'ı sanal makinanız power off, suspend veya power on durumdayken alabilirsiniz. Snapshot alırken karşınıza çıkan seçenekler ile ilgili aşağıdaki yazımı okuyabilirsiniz.

https://www.tayfundeger.com/snapshot-nedir.html

https://www.learnentityframeworkcore.com/migrations/model-snapshot#:~:text=Entity%20Framework%20Core.-,The%20Model%20Snapshot%20In%20Entity%20Framework%20Core,updated%20with%20each%20subsequent%20migration

Jquery Calender--&gt; Datapicker --&gt; DueAt'i takvim tipinde eklemek nasıl yapılır? Araştırınız. (DateTimeUffset tipinden atamalar oluşucak)

-Bkz. https://stackoverflow.com/questions/38711170/datetimeoffset-in-fullcalendar-using-asp-net-mvc

First- FirstOrDefault ve Single- SingleOrDefault nedir? Aralarındaki farkı araştırınız.

-Single : Eğer tek bir eleman dönüyorsa Single komutunu kullanırız.Birden fazla eleman dönüyorsa sorgumuz patlayacaktır.

SingleOrDefault : Single'daki gibi tek bir eleman dönüyorsa kullanabiliriz.Ancak Single'dan farkı şartın sağlanmadığı durumunda hata yerine o tipin varsayılan değerini döndürür.

First : Dönen sonucun ilk elemanını alır.

FirstOrDefault : Dönen sonucun ilk elemanını alır.First'ten farkı eleman dönmezse o tipin varsayılan değerini döndürür.

En kısa null check nasıl yapılır?

-Genelde null check String.IsNullOrEmpty(String) kullanılarak yapılır. Daha kısa şekilde if(obj is null) if(!obj) şeklinde yapılabilir.

Partial view nedir?

-Partial View, view content'inin bir bölümünü oluşturan özel bir view'dır. Tıpkı bir web formu uygulamasının kullanıcı denetimi gibidir. Birden çok görünümde yeniden kullanılabilir.

Farklı authentication bulup,aynı işleri farklı yollar ile yapanları araştırınız.

-Doğrulama organizasyonların ağlarını güvenli bir şekilde sadece izin verilen kullanıcılar veya işlemler tarafından erişilebilir ve tüketilebilir olmasını sağlar.

Bilgi Faktörü (Knowledge Factor):Bu faktörde kullanıcıya ait bilgilere erişirken genellikle bir kullanıcı adı veya email kullanılır ve bu şekilde kullanıcının bildiği şeye erişim sağlanır.

Mülk Faktörü (Possession Factor):Örneğin güvenli bir anahtar taşıyan flash bellek, bir telefon veya farklı bir donanım ile sağlanan bilgilerdir.

Varlık Faktörü (Inherence Factor):Basitçe ayırt edici bilginin vucudunuzda olduğu senaryodur.

İki Faktörlü Doğrulama:İki doğrulama faktörünün birbirini tamamlayıcı olarak veya doğrulamanın çok mühim olduğu ortamlarda çaprazlama yapmak amaçlı kullanıldığı yöntemdir.

Razor Pages/MVC Projects karşılaştırmasını yapınız.

-Razor Pages, asp.net core 2 ile birlikte gelen yeni bir özelliktir. Daha önce kullandığımız asp.net web forms çatısına yaklaşım olarak benzemekle birlikte klasik asp.net webforms'u kullanmadan asp.net mvc üzerine geliştirilmiştir. Razor Pages, sayfa bazlı senaryolar için bildiğimiz mvc (model view controller)'a göre daha kolay uygulama geliştirmeyi sağlayan bir platformdur. Frontend çatılarda kullanılan yaklaşım olan mvvm (model view view model) yapısına benzeşen çift yönlü bağlantı (two way binding) özelliğini desteklemektedir. Razor Pages'in tek sorumluluk prensibine (single responsibility) uygun bir yaklaşımı vardır.
