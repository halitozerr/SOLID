# S.O.L.I.D
S.O.L.I.D., yazılım geliştirme prensiplerinin bir akronimidir. Bu prensipler, nesne yönelimli programlama (OOP) uygulamalarında temiz, sürdürülebilir ve esnek bir kod tabanı oluşturmayı amaçlar. Her bir harf, bir prensibi temsil eder.  Bu Repo S.O.L.I.D'e ait harf açılımlarını ve her bir prensip hakkında detaylı bir açıklama içeririr.


## Yazarlar

- [@halitozer](https://github.com/halitozerr)


## Konular

 - [S.O.L.I.D. Nedir?](https://github.com/halitozerr/solid)
 - [S - Tek Sorumluluk Prensibi (Single Responsibility Principle):](https://github.com/matiassingers/awesome-readme)
 - [O - Açık Kapalılık Prensibi (Open-Closed Principle): ](https://github.com/halitozerr/solid)
 - [L - Liskov Yerine Geçme Prensibi (Liskov Substitution Principle): ](https://github.com/halitozerr/solid)
 - [I - Arayüz Ayrımı Prensibi (Interface Segregation Principle): ](https://github.com/halitozerr/solid)
 - [D - Bağımlılıkları Tersine Çevirme Prensibi (Dependency Inversion Principle): ](https://github.com/halitozerr/solid)






# ✨ S.O.L.I.D. Nedir? 


S.O.L.I.D., yazılım geliştirme prensiplerinin bir akronimidir. Bu prensipler, nesne yönelimli programlama (OOP) uygulamalarında temiz, sürdürülebilir ve esnek bir kod tabanı oluşturmayı amaçlar. Her bir harf, bir prensibi temsil eder. İşte S.O.L.I.D.'in açılımı ve her bir prensip hakkında kısa bir açıklama:

**S - Tek Sorumluluk Prensibi (Single Responsibility Principle):** ⬇️

Bir sınıfın yalnızca bir sorumluluğu olmalıdır. Sınıfların tek bir işlevi veya sorumluluğu olması, kodun anlaşılır olmasını, bağımlılıkların azalmasını ve değişikliklerin kolay yapılmasını sağlar.

**O - Açık Kapalılık Prensibi (Open-Closed Principle):** ⬇️

Mevcut kodu değiştirmeden yeni işlevselliğin eklenmesini sağlar. Sınıflar, değişikliklere kapalı (closed) olmalı ancak yeni işlevsellik eklemeye açık (open) olmalıdır. Bu, kodun genişletilebilir ve değişikliklere karşı dirençli olmasını sağlar.

**L - Liskov Yerine Geçme Prensibi (Liskov Substitution Principle):** ⬇️

Bir üst sınıfın yerine alt sınıfı geçebilmesini ifade eder. Yani, bir üst sınıfın yerine geçen alt sınıflar, aynı davranışı sergilemelidir. Bu, kodun genellemelerin (abstractions) sağladığı esnekliği korumasını ve beklenen davranışlarda tutarlılığı sağlamasını sağlar.

**I - Arayüz Ayrımı Prensibi (Interface Segregation Principle):** ⬇️

İstemciler, ihtiyaçlarına uygun özel arayüzlerle ilişkilendirilmelidir. Bir sınıf, kullanmadığı metotları içeren geniş arayüzlerle bağlantılandırılmamalıdır. Bunun yerine, daha özelleştirilmiş arayüzler kullanarak sınıfların yalnızca ihtiyaç duydukları metotlara erişmeleri sağlanmalıdır. Bu, bağımlılıkları azaltır, sınıfların bağımsızlığını artırır ve kodun daha sürdürülebilir olmasını sağlar.

**D - Bağımlılıkları Tersine Çevirme Prensibi (Dependency Inversion Principle):** ⬇️

Üst seviye modüller, alt seviye modüllere bağımlı olmamalıdır. Bağımlılıklar, soyutlamalar üzerinden yönetilmeli ve istemci kodlarının somut uygulamalara değil, arayüzlere bağımlı olması sağlanmalıdır. Bu, kodun değişikliklere karşı esnek olmasını sağlar ve bağımlılıkların daha kolay yönetilebilmesini sağlar. Soyutlamalar ve arayüzler, bağımlılıkları gevşetir ve farklı uygulamaların kolayca yerine geçebilmesini sağlar.

--
S.O.L.I.D. prensipleri, kodun daha temiz, sürdürülebilir, genişletilebilir ve esnek olmasını sağlamak için kullanılan önemli yönergelerdir. Bu prensiplerin uygulanması, kod tabanının daha iyi bir tasarımına ve gelecekteki değişikliklere daha kolay uyum sağlayabilmesine yardımcı olur. Ayrıca, yazılımın test edilebilirliğini artırır, kod tekrarını azaltır ve daha yüksek kalitede bir kod tabanı oluşturur.




## ⚡ Tek Sorumluluk Prensibi (Single Responsibility Principle) ℹ️

Tek Sorumluluk Prensibi (Single Responsibility Principle - SRP), nesne yönelimli programlamada önemli bir prensiptir. Bu prensibe göre, bir sınıfın yalnızca bir sorumluluğu olmalı ve bu sorumluluğu en iyi şekilde yerine getirmelidir.
Tek Sorumluluk Prensibi, bir sınıfın birden fazla sorumluluğu üstlenmesinin dezavantajlarını ortadan kaldırmayı amaçlar. Bir sınıfın birden fazla sorumluluğu olduğunda, bu sınıfın değişikliklere karşı daha kırılgan hale gelme olasılığı artar. İçerdiği birden fazla sorumluluk nedeniyle, bir sorumlulukta yapılan değişiklikler diğer sorumlulukları etkileyebilir ve beklenmedik yan etkilere neden olabilir.

➕ **SRP'nin temel faydaları şunlardır:**

1.	📦 **Daha iyi kod organizasyonu:** 
Tek Sorumluluk Prensibi, kodu daha iyi organize etmeyi sağlar. Bir sınıfın yalnızca belirli bir sorumluluğu olduğunda, kod daha anlaşılır, okunabilir ve sürdürülebilir hale gelir. Sınıfın ismi ve yapısı, sorumluluğunu doğru şekilde yansıtır.

2.	📦 **Daha az bağımlılık:** 
Bir sınıfın birden fazla sorumluluğu olduğunda, bu sınıf diğer sınıflarla daha sıkı bir şekilde bağlantılı hale gelir. Bu da bağımlılıkları artırır ve kodun yeniden kullanılabilirliğini zorlaştırır. Tek Sorumluluk Prensibi, sınıflar arasındaki bağımlılıkları azaltarak, bağımsız ve birbirinden bağımsız bileşenlerin oluşturulmasını sağlar.

3.	📦 **Kolay sürdürme ve değiştirme:** 
Sınıfların tek bir sorumluluğu olduğunda, bu sınıfları sürdürmek ve değiştirmek daha kolay olur. Bir sorumlulukta yapılan değişiklikler, diğer sorumlulukları etkilemez ve beklenmedik hatalara neden olmaz. Kodunuzda değişiklik yapmanız gerektiğinde, yalnızca ilgili sınıfı etkileyen değişiklikler yapmanız yeterlidir.

4.	📦 **Test edilebilirlik:** 
Tek Sorumluluk Prensibi, kodun daha test edilebilir olmasını sağlar. Bir sınıfın yalnızca bir sorumluluğu olduğunda, bu sorumluluğa odaklanarak daha küçük ve daha özgün test senaryoları oluşturmak daha kolaydır.

Örneğin, bir Müşteri sınıfını düşünelim. Müşteri sınıfının sorumlulukları müşteri bilgilerini tutmak, hesap işlemlerini yapmak ve e-posta göndermek olabilir. Ancak, bu sınıfın birden fazla sorumluluğu olduğunda, değişiklik yapmak veya hata ayıklamak zorlaşabilir.
Tek Sorumluluk Prensibi'ne göre, bu sorumluluklar ayrı sınıflara ayrılmalıdır. Örneğin, MüşteriBilgileri sınıfı müşteri bilgilerini tutarken, HesapIslemleri sınıfı hesap işlemlerini yapabilir ve EpostaGonderici sınıfı e-posta gönderme işlemlerinden sorumlu olabilir. Her bir sınıf yalnızca tek bir sorumluluğa odaklanır ve bu sorumluluğu en iyi şekilde yerine getirir.

➕ **Bu yaklaşımın faydaları şunlardır:**

•	Sınıflar arasındaki bağımlılıklar azalır ve değişikliklerin etki alanı daralır.

•	Kod daha modüler hale gelir, böylece her bir sınıfı bağımsız olarak geliştirebilir, test edebilir ve sürdürebilirsiniz.

•	İlgili sınıfların tek sorumluluğu olduğu için, kod daha anlaşılır ve bakımı daha kolay hale gelir.

•	Birden fazla sorumluluğu olan bir sınıf yerine, daha küçük ve özgün sınıfların kullanılması, kodun yeniden kullanılabilirliğini artırır ve kod tekrarını azaltır.

--Tek Sorumluluk Prensibi, yazılım geliştirme sürecinde temiz kod yazmaya ve düzenli bir yapı oluşturmaya yardımcı olur. Bu prensibi uygulayarak, kodunuzun daha sürdürülebilir, esnek ve anlaşılabilir olmasını sağlayabilirsiniz.


## ⌨️ Kullanım/Örnek 

```c#
using System;

// Veritabanına kaydetme işlemlerini gerçekleştiren sınıf
public class DatabaseManager
{
    public void SaveData(string data)
    {
        // Veritabanına kaydetme işlemleri
        Console.WriteLine("Veri kaydedildi: " + data);
    }
}

// Veri işleme işlemlerini gerçekleştiren sınıf
public class DataProcessor
{
    public string ProcessData(string data)
    {
        // Veri işleme işlemleri
        Console.WriteLine("Veri işlendi: " + data);
        return "İşlenmiş veri: " + data;
    }
}

// Ana uygulama sınıfı
public class Program
{
    static void Main(string[] args)
    {
        string rawData = "Örnek veri";

        DataProcessor processor = new DataProcessor();
        string processedData = processor.ProcessData(rawData);

        DatabaseManager dbManager = new DatabaseManager();
        dbManager.SaveData(processedData);

        Console.ReadLine();
    }
}

```



## ⚡ Açık Kapalılık Prensibi (Open-Closed Principle) ℹ️

Açık Kapalılık Prensibi (Open-Closed Principle - OCP), nesne yönelimli programlamada önemli bir prensiptir. Bu prensibe göre, mevcut kodu değiştirmeden yeni işlevselliği eklemek mümkün olmalıdır. Yani, bir sınıfın davranışını değiştirmek için sınıfın kendisini değiştirmek yerine, yeni davranışları eklemek için sınıfın genişletilebilir olması gerekmektedir.
Açık Kapalılık Prensibi, yazılım bileşenlerinin genişletilebilir olmasını ve değişikliklere karşı kapalı olmasını hedefler. Bu prensip, kodun esnekliğini ve sürdürülebilirliğini artırır.
Prensibin temel fikri, mevcut kodu değiştirmeden yeni gereksinimlere uyum sağlamaktır. Bu, mevcut sınıfların işlevselliğini korurken, yeni gereksinimleri karşılamak için yeni sınıflar veya modüller ekleyebileceğimiz anlamına gelir.

➕ **Açık Kapalılık Prensibi'nin bazı anahtar noktaları şunlardır:**

1.	📦 **Değişikliklere kapalı (Closed) olma:**
 Mevcut kodda bir değişiklik yapmak, değişiklikleri uyguladığınız sınıfın kaynak kodunu değiştirmenizi gerektirmez. Mevcut kodun çalışmasını etkilemeden yeni işlevselliği eklemek için mevcut kodun kapalı olması gerekmektedir.

2.	📦 **Yeni işlevselliğe açık (Open) olma:**
 Yeni gereksinimler ortaya çıktığında, mevcut kodu değiştirmeden yeni işlevselliği eklemek mümkün olmalıdır. Bu genellikle sınıfın genişletilebilir olmasıyla sağlanır. Yeni gereksinimler, mevcut kodun etkilenmediği yeni sınıflar veya modüller kullanılarak gerçekleştirilir.

3.	📦 **Soyutlamalar (Abstractions) kullanma:**
 Açık Kapalılık Prensibi'ni uygulamak için soyutlamalar (abstractions) kullanılır. Soyutlama, ortak davranışları ve özellikleri tanımlayan arayüzleri veya soyut sınıfları içerir. Bu sayede, yeni işlevselliği eklemek için bu soyutlamaları uygulayan yeni sınıflar oluşturulabilir.


➕ **Açık Kapalılık Prensibi'nin avantajları şunlardır:**

•	Mevcut kodun değişmeden kalması, mevcut işleyişin bozulmasını önler ve hatalı kod düzeltmelerinin ortaya çıkmasını engeller.

•	Kodun genişletilebilirliği artar, yeni gereksinimler daha kolay bir şekilde karşılanabilir.

•	Kodun yeniden kullanılabilirliği artar. Mevcut sınıfların veya bileşenlerin başka projelerde veya farklı bağlamlarda kullanılması daha kolay hale gelir.

•	Birbirine bağımlı olan bileşenlerin azaltılmasıyla, değişikliklerin yayılma etkisi azalır ve hata riski düşer.

•	Test edilebilirlik artar. Mevcut kodun değişikliklere kapalı olması, bir bileşenin işlevselliğini bağımsız olarak test etmenizi sağlar.

➕ **Açık Kapalılık Prensibi'nin uygulanması, genellikle aşağıdaki yaklaşımları içerir:**

•	**Soyutlama kullanımı:** Soyutlama, kodun genişletilebilirliğini sağlamak için önemlidir. Soyut sınıflar veya arayüzler tanımlanarak, genel davranışlar ve özellikler belirlenir. Yeni gereksinimler için bu soyutlamaları uygulayan yeni sınıflar oluşturulabilir.

•	**Polimorfizm kullanımı:** Polimorfizm, farklı sınıfların aynı arayüzü uygulayabilmesini sağlar. Bu, mevcut kodun yeni sınıflarla genişletilebilmesini ve farklı davranışların elde edilebilmesini sağlar.

•	**Tasarım desenlerinin kullanımı:** Açık Kapalılık Prensibi, tasarım desenlerinin uygulanmasıyla desteklenir. Özellikle, Strateji Deseni, Fabrika Deseni ve Yönlendirici (Router) Deseni gibi desenler, yeni işlevselliği eklemek için mevcut kodu değiştirmeden uygulanabilir.

Açık Kapalılık Prensibi, kodun daha esnek, sürdürülebilir ve genişletilebilir olmasını sağlar. Bu prensibi uygulayarak, gelecekteki değişikliklere daha kolay uyum sağlayabilir ve yazılımınızı daha kaliteli hale getirebilirsiniz.




## ⌨️ Kullanım/Örnek 

```c#
using System;

// Şekilleri temsil eden soyut sınıf
public abstract class Shape
{
    public abstract double CalculateArea();
}

// Dikdörtgen sınıfı
public class Rectangle : Shape
{
    public double Width { get; set; }
    public double Height { get; set; }

    public override double CalculateArea()
    {
        return Width * Height;
    }
}

// Çember sınıfı
public class Circle : Shape
{
    public double Radius { get; set; }

    public override double CalculateArea()
    {
        return Math.PI * Radius * Radius;
    }
}

// Alan hesaplama işlemlerini gerçekleştiren sınıf
public class AreaCalculator
{
    public double CalculateTotalArea(Shape[] shapes)
    {
        double totalArea = 0;

        foreach (Shape shape in shapes)
        {
            totalArea += shape.CalculateArea();
        }

        return totalArea;
    }
}

// Ana uygulama sınıfı
public class Program
{
    static void Main(string[] args)
    {
        Shape[] shapes = new Shape[2];
        shapes[0] = new Rectangle { Width = 5, Height = 3 };
        shapes[1] = new Circle { Radius = 2.5 };

        AreaCalculator calculator = new AreaCalculator();
        double totalArea = calculator.CalculateTotalArea(shapes);

        Console.WriteLine("Toplam alan: " + totalArea);

        Console.ReadLine();
    }
}


```



## ⚡ Liskov Yerine Geçme Prensibi (Liskov Substitution Principle) ℹ️

Liskov Yerine Geçme Prensibi (Liskov Substitution Principle - LSP), nesne yönelimli programlamada önemli bir prensiptir. Bu prensibe göre, bir sınıf, türetilen sınıfların yerine geçebilmeli ve bu değişiklik hiçbir şekilde programın doğruluğunu etkilememelidir.
LSP, açıkça ifade edilmiş olan ve türetilen sınıfın davranışını tanımlayan bir sözleşmenin (contract) yerine getirilmesini vurgular. Sözleşme, üst sınıfın davranışlarını ve işlevlerini belirler. Türetilen sınıflar, bu sözleşmeyi tam anlamıyla yerine getirmelidir ve aynı şekilde kullanılabilir olmalıdır.
LSP'nin ana prensipleri şunlardır:
1. 📦 **Alt türlerin davranışı:** Bir türetilen sınıf, üst sınıfın davranışlarını değiştirmeden veya kısıtlamadan yerine geçebilmelidir. Yani, türetilen sınıfın üst sınıfın tanımladığı işlevlere aynı şekilde cevap vermesi gerekmektedir.

2.	📦 **Önkoşul ve sonuç koşulları:** Bir türetilen sınıf, üst sınıfın belirlediği önkoşulları gevşetemez veya sonuç koşullarını sıkılaştıramaz. Yani, üst sınıfın bir işlevi belirli bir önkoşula bağlıysa, türetilen sınıf bu önkoşulu daha da gevşetemez. Benzer şekilde, üst sınıfın bir işlevi belirli bir sonuç koşuluna bağlıysa, türetilen sınıf bu sonuç koşulunu daha da sıkılaştıramaz.


LSP'nin temel amacı, bir kod parçasının bir sınıfın yerine geçen herhangi bir alt sınıfı kullanarak çalışmasını sağlamaktır. Bu prensibi uygulamak, kodun genişletilebilirliğini ve değiştirilebilirliğini artırır. Aynı zamanda, LSP, modüler ve yeniden kullanılabilir kod yazmanın önemli bir unsuru olarak kabul edilir.

➕ **LSP'nin faydaları şunlardır:**

•	Kodun yeniden kullanılabilirliği artar. Üst sınıfın yerine geçen herhangi bir alt sınıf, aynı şekilde kullanılabilir ve mevcut kodla uyumlu olabilir.

•	Sürdürülebilirlik iyileşir. Kodun belirli bir yerinde yapılan değişiklikler, diğer yerlerde beklenmedik hatalara veya yan etkilere neden olmaz.

•	Test edilebilirlik artar. Bir bileşeni veya sınıfı test etmek için, üst sınıfı temsil eden bir sınıfın yerine geçen alt sınıfları kullanabilirsiniz. Bu şekilde, testler daha genel ve daha az spesifik olabilir.

•	Modülerlik sağlanır. LSP, birbirine bağımlı bileşenler arasındaki sıkı bağımlılığı azaltır ve bileşenlerin daha bağımsız bir şekilde geliştirilmesini ve değiştirilmesini sağlar.

•	Takım çalışmasını kolaylaştırır. LSP, birden fazla geliştiricinin aynı projede çalışmasını kolaylaştırır. Bir geliştirici, üst sınıflara bağlı olarak kod yazabilirken, başka bir geliştirici de bu üst sınıfları temsil eden alt sınıflar üzerinde çalışabilir.

➕ **LSP'nin uygulanması için bazı temel stratejiler şunlardır:**

•	İnterface veya Soyut Sınıflar kullanma: Üst sınıfın davranışlarını tanımlayan interface'ler veya soyut sınıflar kullanarak LSP'yi uygulayabilirsiniz. Türetilen sınıflar bu interface'leri veya soyut sınıfları uygulayarak aynı sözleşmeyi yerine getirir ve yerlerine geçebilir.

•	Önkoşul ve sonuç koşullarını iyi tanımlama: Üst sınıfın belirlediği önkoşul ve sonuç koşullarını dikkatlice tanımlayarak, türetilen sınıfların bu koşulları korumasını sağlayabilirsiniz.

•	LSP'yi test etme: LSP'nin doğru bir şekilde uygulandığını doğrulamak için testler oluşturabilirsiniz. Türetilen sınıfların üst sınıfların yerine geçebildiğini ve aynı davranışı sergilediğini doğrulayan testler yazabilirsiniz.

Liskov Yerine Geçme Prensibi, kodunuzun daha esnek, sürdürülebilir ve genişletilebilir olmasını sağlar. Bu prensibi doğru bir şekilde uygulayarak, kodunuzun daha güvenilir ve daha kolay yönetilebilir hale gelmesini sağlayabilirsiniz.

## ⌨️ Kullanım/Örnek 

```c#
using System;

// Hayvanları temsil eden soyut sınıf
public abstract class Animal
{
    public abstract void MakeSound();
}

// Kuş sınıfı
public class Bird : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Chirp chirp!");
    }
}

// Köpek sınıfı
public class Dog : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Woof woof!");
    }
}

// Hayvan seslerini çalan sınıf
public class AnimalSoundPlayer
{
    public void PlayAnimalSound(Animal animal)
    {
        animal.MakeSound();
    }
}

// Ana uygulama sınıfı
public class Program
{
    static void Main(string[] args)
    {
        AnimalSoundPlayer soundPlayer = new AnimalSoundPlayer();

        Animal bird = new Bird();
        soundPlayer.PlayAnimalSound(bird);

        Animal dog = new Dog();
        soundPlayer.PlayAnimalSound(dog);

        Console.ReadLine();
    }
}



```


## ⚡ Arayüz Ayrımı Prensibi (Interface Segregation Principle) ℹ️

Arayüz Ayrımı Prensibi (Interface Segregation Principle - ISP), nesne yönelimli programlamada bir prensiptir ve arayüzlerin tasarımını etkiler. ISP, bir sınıfın ihtiyaç duymadığı metotlara veya özelliklere bağımlı olmamasını ve yalnızca ihtiyaç duyduğu işlevselliği içermesini hedefler.

ISP, bir arayüzün birçok küçük ve özelleştirilmiş arayüzlere bölünmesini teşvik eder. Bu, her sınıfın yalnızca kendi ihtiyaç duyduğu metotları içeren arayüzleri uygulamasını sağlar, gereksiz metotlarla yüklenmeyi önler.

➕ **ISP'nin temel prensipleri şunlardır:**

1.	📦 **İstemciye özelleştirilmiş arayüzler sağlama:** İstemciler, yalnızca ihtiyaç duydukları metotları içeren arayüzleri kullanmalıdır. Böylece, istemciler sadece kendi ihtiyaçlarına uygun metotları kullanabilirler ve gereksiz metotlarla uğraşmak zorunda kalmazlar.

2.	📦 **Bağımlılıkları azaltma:** ISP, bir sınıfın yalnızca ihtiyaç duyduğu arayüzleri uygulamasını sağlar. Bu, sınıfların gereksiz bağımlılıklardan kaçınmasına ve daha esnek bir yapıya sahip olmasına olanak tanır.

3.	📦 **Arayüzlerin özelleştirilmesi:** ISP, genel ve çok amaçlı arayüzler yerine daha özelleştirilmiş ve spesifik arayüzlerin oluşturulmasını teşvik eder. Böylece, sınıflar yalnızca kendi ihtiyaçlarına uygun metotları içeren arayüzleri uygularlar.

➕ **ISP'nin amaçları şunlardır:**

•	Sınıfların bağımlılıklarını azaltmak ve bağımlılık prensibini uygulamak.

•	Sınıfların gereksiz kodla yüklenmemesini ve gereksiz metotlara sahip olmamasını sağlamak.

•	Sınıfların daha esnek ve yeniden kullanılabilir olmasını sağlamak.

•	Kodun bakımını kolaylaştırmak ve değişiklikleri daha az riskli hale getirmek.

➕ **ISP'nin uygulanması için bazı temel stratejiler şunlardır:**

•	**Arayüzleri bölme:** Geniş arayüzleri daha küçük ve daha özelleştirilmiş arayüzlere bölerek, her sınıfın yalnızca ihtiyaç duyduğu arayüzleri uygulamasını sağlayabilirsiniz.

•	**Arayüzleri birleştirme:** Benzer özelliklere sahip olan arayüzleri birleştirerek, gereksiz tekrarları önleyebilirsiniz. Bu sayede sınıflar, yalnızca bir arayüzü uygulayarak ihtiyaç duydukları işlevselliği elde edebilirler.

•	**Arayüz ayırımıyla bağımlılıkları kontrol etme:** Sınıfların yalnızca ihtiyaç duydukları arayüzleri kullanmalarını sağlayarak, bağımlılıkları azaltabilirsiniz. Bu, sınıfların değişikliklere daha esnek bir şekilde uyum sağlamasını ve kodun bakımını kolaylaştırır.

•	**İstemci odaklı arayüzler tasarlama:** Arayüzleri, istemci kodunun ihtiyaçlarını karşılayacak şekilde tasarlayın. İstemci, yalnızca kendi ihtiyaçlarına uygun metotları kullanabilmelidir. Bu, istemci kodunun daha anlaşılır ve daha az karmaşık olmasını sağlar.

➕ **ISP'nin faydaları şunlardır:**

•	**Bağımlılıkları azaltır:** ISP, sınıfların gereksiz bağımlılıklardan kaçınmasını sağlar. Böylece, sınıfların değişikliklere daha dirençli olmaları ve daha kolay test edilebilir olmaları sağlanır.

•	**Kodun anlaşılırlığını artırır:** Sınıfların yalnızca ihtiyaç duydukları metotları içeren arayüzleri uygulaması, kodun daha anlaşılır ve daha kolay takip edilebilir olmasını sağlar.

•	**Yeniden kullanılabilirliği artırır:** Özelleştirilmiş arayüzlerin kullanılması, sınıfların daha bağımsız ve yeniden kullanılabilir olmasını sağlar. Böylece, bir sınıfın farklı bağlamlarda kullanılması daha kolay hale gelir.

•	**Paralel geliştirmeyi kolaylaştırır:** Küçük ve özelleştirilmiş arayüzler, farklı geliştiricilerin aynı anda çalışmasını kolaylaştırır. Her geliştirici, ihtiyaç duyduğu arayüzleri kullanarak bağımsız olarak çalışabilir.

ISP prensibi, sınıfların ihtiyaçlarına uygun arayüzleri kullanmalarını ve gereksiz bağımlılıklardan kaçınmalarını sağlar. Bu, kodun daha modüler, esnek ve sürdürülebilir olmasını sağlar. ISP'nin doğru bir şekilde uygulanması aşağıdaki avantajlara sahiptir:

1.	📦 **Bağımlılıkları azaltır:** Her sınıfın yalnızca ihtiyaç duyduğu arayüzleri kullanması, gereksiz bağımlılıkları ortadan kaldırır. Bu, değişikliklerin bir sınıfın diğer sınıflara olan etkisini azaltır ve kodun değişime daha dirençli olmasını sağlar.

2.	📦 **Modülerlik sağlar:** Arayüzlerin küçük ve spesifik olması, kodun modüler bir şekilde organize edilmesine olanak tanır. Bir sınıfın yalnızca ilgili arayüzleri uygulaması, sınıfın işlevselliğini açık ve anlaşılır hale getirir.

3.	📦 **Kodun anlaşılırlığını artırır:** İstemciler, yalnızca kendi ihtiyaçlarına uygun arayüzleri kullanır. Bu, kodun daha anlaşılır olmasını sağlar çünkü her sınıfın neyle ilgilendiği açık bir şekilde görülür.

4.	📦 **Yeniden kullanılabilirlik ve bakım kolaylığı:** ISP, sınıfların daha bağımsız ve yeniden kullanılabilir olmasını sağlar. Bir arayüzün değişmesi durumunda, yalnızca ilgili sınıflar etkilenir ve diğer sınıflarda bir değişiklik yapılmasına gerek kalmaz. Bu da kodun bakımını kolaylaştırır ve değişikliklerin yayılma riskini azaltır.

5.	📦 **Paralel geliştirmeyi destekler:** ISP, farklı geliştiricilerin aynı anda çalışmasını kolaylaştırır. Her bir geliştirici, ihtiyaç duyduğu arayüzleri kullanarak kendi modüllerini geliştirebilir. Bu, geliştirme sürecini hızlandırır ve işbirliği olanaklarını artırır.

ISP prensibi, kodun daha temiz, daha anlaşılır ve daha esnek olmasını sağlar. İhtiyaç duyulan özelliklere sahip küçük ve spesifik arayüzlerin kullanılması, kodun daha modüler bir yapıya sahip olmasını ve değişikliklere daha adapte olmasını sağlar. Bu da yazılım projelerinin sürdürülebilirliğini artırır ve gelecekteki genişlemelere uyum sağlama kolaylığı sağlar.


## ⌨️ Kullanım/Örnek 

```c#
using System;

// IAnimal arayüzü
public interface IAnimal
{
    void Eat();
    void Sleep();
}

// IFlyable arayüzü
public interface IFlyable
{
    void Fly();
}

// IHopable arayüzü
public interface IHopable
{
    void Hop();
}

// Kuş sınıfı, IAnimal ve IFlyable arayüzlerini uygular
public class Bird : IAnimal, IFlyable
{
    public void Eat()
    {
        Console.WriteLine("The bird is eating.");
    }

    public void Sleep()
    {
        Console.WriteLine("The bird is sleeping.");
    }

    public void Fly()
    {
        Console.WriteLine("The bird is flying.");
    }
}

// Tavşan sınıfı, IAnimal ve IHopable arayüzlerini uygular
public class Rabbit : IAnimal, IHopable
{
    public void Eat()
    {
        Console.WriteLine("The rabbit is eating.");
    }

    public void Sleep()
    {
        Console.WriteLine("The rabbit is sleeping.");
    }

    public void Hop()
    {
        Console.WriteLine("The rabbit is hopping.");
    }
}

// Hayvan bakıcısı sınıfı
public class AnimalCareTaker
{
    public void PerformDailyTasks(IAnimal animal)
    {
        animal.Eat();
        animal.Sleep();
    }
}

// Uçabilen hayvan bakıcısı sınıfı
public class FlyableAnimalCareTaker
{
    public void PerformDailyTasks(IFlyable flyableAnimal)
    {
        flyableAnimal.Fly();
    }
}

// Sıçrayabilen hayvan bakıcısı sınıfı
public class HopableAnimalCareTaker
{
    public void PerformDailyTasks(IHopable hopableAnimal)
    {
        hopableAnimal.Hop();
    }
}

// Ana uygulama sınıfı
public class Program
{
    static void Main(string[] args)
    {
        AnimalCareTaker animalCareTaker = new AnimalCareTaker();
        FlyableAnimalCareTaker flyableAnimalCareTaker = new FlyableAnimalCareTaker();
        HopableAnimalCareTaker hopableAnimalCareTaker = new HopableAnimalCareTaker();

        IAnimal bird = new Bird();
        animalCareTaker.PerformDailyTasks(bird);
        flyableAnimalCareTaker.PerformDailyTasks(bird);

        IAnimal rabbit = new Rabbit();
        animalCareTaker.PerformDailyTasks(rabbit);
        hopableAnimalCareTaker.PerformDailyTasks(rabbit);

        Console.ReadLine();
    }
}



```


## ⚡ Bağımlılıkları Tersine Çevirme Prensibi (Dependency Inversion Principle) ℹ️

Bağımlılıkları Tersine Çevirme Prensibi (Dependency Inversion Principle - DIP), nesne yönelimli programlamada bir prensiptir ve yazılım bileşenlerinin tasarımını etkiler. DIP, yüksek seviyeli modüllerin düşük seviyeli modüllere doğrudan bağımlı olmamasını, bunun yerine soyutlamalara ve arayüzlere bağımlı olmasını hedefler.

➕ **DIP, aşağıdaki temel prensipleri içerir:**

1.	📦 **Yüksek seviyeli modüller düşük seviyeli modüllere bağımlı olmamalıdır:** Yüksek seviyeli modüller, düşük seviyeli detaylara doğrudan bağımlı olmamalıdır. Bunun yerine, soyutlamalara ve arayüzlere bağımlı olmalıdır. Yani, yüksek seviyeli bir modül, düşük seviyeli bir modülün detaylarına doğrudan erişmek yerine, bir arayüz üzerinden etkileşim kurmalıdır.

2.	📦 **Soyutlamalara ve arayüzlere bağımlı olunmalıdır:** Modüller, soyutlamalara ve arayüzlere bağımlı olmalıdır, somut implementasyonlara değil. Böylece, modüller arasındaki bağımlılıklar soyutlamalar üzerinden gerçekleşir ve daha esnek bir yapı elde edilir. Bu, bileşenlerin birbirleriyle daha az sıkı bağlantılı olmasını ve değişikliklerin daha az etkilenmesini sağlar.

➕ **DIP prensibinin amaçları şunlardır:**

•	**Bağımlılıkları azaltmak:** DIP, yüksek seviyeli modüllerin düşük seviyeli detaylara bağımlılığını azaltır. Bu, modüllerin daha bağımsız bir şekilde çalışmasını ve değişikliklere daha dirençli olmasını sağlar.

•	**Modülerlik sağlamak:** Soyutlamalara ve arayüzlere bağımlı olmak, modüler bir yapı sağlar. Modüller birbirinden bağımsız olarak geliştirilebilir, test edilebilir ve yeniden kullanılabilir hale gelir.

•	**Esneklik sağlamak:** DIP, yazılımın esnekliğini artırır. Değişikliklerin yüksek seviyeli modülleri etkilemesi gerekmez, sadece düşük seviyeli detaylara ilişkin kodlar değiştirilir.

•	**Test edilebilirlik:** DIP, yazılımın test edilebilirliğini artırır. Modüller arasındaki bağımlılıkların arayüzler üzerinden gerçekleşmesi, bileşenlerin izole edilmiş bir şekilde test edilmesini kolaylaştırır.

➕ **DIP'nin uygulanması için aşağıdaki stratejiler kullanılabilir:**

1.	📦 **Arayüzlerin kullanımı:** Modüller arasındaki bağımlılıklar, soyutlama düzeyindeki arayüzler üzerinden gerçekleştirilir. Yüksek seviyeli modüller, düşük seviyeli modüllere doğrudan bağımlı olmak yerine, arayüzleri kullanarak iletişim kurar. Bu sayede modüllerin değiştirilmesi ve yeniden kullanılması kolaylaşır.

2.	📦 **Bağımlılık enjeksiyonu (Dependency Injection):** DIP'yi uygulamak için yaygın olarak kullanılan bir yöntemdir. Bağımlılık enjeksiyonu, modüllerin ihtiyaç duyduğu bağımlılıkları harici olarak almasını sağlar. Bu sayede modüller, bağımlılıkları ile doğrudan etkileşime geçmez ve soyutlamalara dayalı bir şekilde çalışır.

3.	📦 **Soyutlama ve arayüz tasarımı:** DIP, uygun soyutlamaların ve arayüzlerin tasarlanmasını gerektirir. Modüller, soyutlamalara ve arayüzlere bağımlı olmalı ve somut implementasyonlarla doğrudan bağlantılı olmamalıdır. Böylece, modüllerin daha genel ve esnek bir şekilde kullanılması sağlanır.

➕ **DIP'nin faydaları şunlardır:**

•	**Esneklik:** DIP, yazılımın esnekliğini artırır. Modüller arasındaki bağımlılıklar soyutlama düzeyinde gerçekleştiği için, bir modülde yapılacak değişiklikler diğer modülleri etkilemez.

•	**Test edilebilirlik:** DIP, bileşenlerin izole edilmiş bir şekilde test edilmesini kolaylaştırır. Bağımlılıkların enjekte edilmesi sayesinde, modüllerin testlerde taklit edilebilir ve kontrol edilebilir hale gelir.

•	**Daha az bağımlılık:** DIP, düşük seviyeli modüllerin yüksek seviyeli modüllere doğrudan bağımlı olmasını önler. Bu, bir bileşenin diğer bileşenler üzerindeki bağımlılığını azaltır ve kodun bakımını kolaylaştırır.

•	**Modülerlik:** DIP, modüler bir yapı oluşturmayı teşvik eder. Modüller arasındaki bağımlılıklar soyutlamalar üzerinden gerçekleştiği için, her bir modülün görevi ve sorumluluğu daha net ve bağımsız hale gelir.

•	**Yeniden kullanılabilirlik:** DIP, bileşenlerin bağımsızlığını ve soyutlamalara dayalı olmasını sağlar. Bu da bileşenlerin daha genel ve yeniden kullanılabilir olmasını sağlar.

Bağımlılık Tersine Çevirme Prensibi (Dependency Inversion Principle - DIP), yazılım tasarımında bağımlılıkların yüksek seviyeli bileşenlere doğru tersine çevrilmesini vurgular. Bu prensip, yazılımın daha esnek, genişletilebilir ve sürdürülebilir olmasını sağlar.

➕ **DIP'nin temel prensipleri şunlardır:**

1.	📦 **Üst düzey modüller, alt düzey modüllere bağımlı olmamalıdır:** Yüksek seviyeli bileşenler, düşük seviyeli ayrıntılara doğrudan bağımlı olmamalıdır. Bunun yerine, soyutlamalara ve arayüzlere bağımlı olmalıdır. Yüksek seviyeli modüller, düşük seviyeli modüllerin nasıl uygulandığından bağımsız olmalıdır.

2.	📦 **Soyutlamalara bağımlı olunmalıdır:** Modüller, soyutlamalara ve arayüzlere bağımlı olmalı, somut implementasyonlara değil. Böylece, modüller arasındaki bağımlılıklar soyutlamalar üzerinden gerçekleşir ve bileşenler arasındaki bağımlılık azaltılır.
DIP'nin temel amacı, yüksek seviyeli bileşenlerin alt seviye ayrıntılardan izole edilmesini sağlamaktır. Bunun için aşağıdaki stratejiler kullanılabilir:

2.1.	📦 **Bağımlılık enjeksiyonu (Dependency Injection):** Bu strateji, bir bileşene gereken diğer bileşenlerin dışarıdan sağlanmasını sağlar. Bağımlılık enjeksiyonu, bağımlılıkların bileşenin yapıcı metodunda veya özellikler aracılığıyla sağlandığı enjeksiyon noktalarını kullanır. Bu sayede bileşen, bağımlılıkları üzerinden doğrudan etkileşim kurmaz ve soyutlamalar üzerinden çalışır.

2.2.	📦 **Soyutlamaların kullanımı:** DIP'nin sağladığı esnekliği elde etmek için soyutlamalar kullanılır. Bir bileşenin somut bir sınıfa değil, soyut bir arayüze bağımlı olması, bileşenin değiştirilebilir ve yeniden kullanılabilir olmasını sağlar.

➕ **DIP prensibinin faydaları şunlardır:**

•	**Esneklik:** DIP, yazılımın daha esnek olmasını sağlar. Yüksek seviyeli bileşenlerin düşük seviyeli ayrıntılara bağımlı olmaması, değişikliklerin daha az etkilenmesini ve bileşenlerin daha bağımsız çalışmasını sağlar.

•	**Genişletilebilirlik:** DIP, yazılımın genişletilebilir olmasını sağlar. Alt seviyedeki bileşenlerin değiştirilmesi veya yeni bileşenlerin eklenmesi durumunda, yüksek seviyeli bileşenlere dokunulmadan değişiklik yapılabilir. Bu, yazılımın daha modüler ve genişletilebilir olmasını sağlar.

•	**Test edilebilirlik:** DIP, bileşenlerin test edilebilirliğini artırır. Bağımlılıkların enjekte edilmesi sayesinde, bir bileşenin test edilmesi sırasında bağımlı bileşenlerin yerine taklit edilebilen veya kontrol edilebilen sahte nesneler (mock) kullanılabilir. Bu, bileşenlerin izole edilmiş bir şekilde test edilmesini kolaylaştırır.

•	**Bileşenler arasındaki gevşek bağlantı:** DIP, bileşenler arasındaki bağımlılıkların azaltılmasını sağlar. Bileşenler, soyutlamalara ve arayüzlere bağımlı olduğu için, farklı bileşenlerin farklı somut implementasyonlarıyla çalışabilir. Böylece, bir bileşenin değiştirilmesi veya yeni bir bileşenin eklenmesi diğer bileşenleri etkilemez.

•	**Tekrar kullanılabilirlik:** DIP, bileşenlerin daha tekrar kullanılabilir hale gelmesini sağlar. Soyutlamalara dayalı bağımlılıklar, farklı senaryolarda bileşenlerin yeniden kullanılmasını kolaylaştırır. Aynı arayüzü uygulayan farklı bileşenler, aynı şekilde kullanılabilir ve değiştirilebilir.

•	**Bağımlılık yönetimi:** DIP, bağımlılıkların yönetimini kolaylaştırır. Bileşenler arasındaki bağımlılıklar, genellikle enjeksiyon noktaları aracılığıyla yönetilir. Bu, bileşenlerin oluşturulması, konfigürasyonu ve yaşam döngüsünün kontrolünü daha esnek hale getirir.

Bağımlılıkları Tersine Çevirme Prensibi, SOLID prensiplerinin bir parçası olarak yazılımın daha esnek, genişletilebilir ve sürdürülebilir olmasını sağlar. Bileşenlerin somut implementasyonlara değil, soyutlamalara ve arayüzlere bağımlı olması, yazılımın daha modüler bir yapıya sahip olmasını ve değişikliklere daha dirençli olmasını sağlar.


## ⌨️ Kullanım/Örnek 

```c#
using System;

// Veritabanı işlemlerini gerçekleştiren arabirim
public interface IDatabase
{
    void SaveData(string data);
}

// Veritabanı işlemlerini gerçekleştiren sınıf
public class Database : IDatabase
{
    public void SaveData(string data)
    {
        Console.WriteLine("Veri kaydedildi: " + data);
    }
}

// Veri işleme işlemlerini gerçekleştiren sınıf
public class DataProcessor
{
    private IDatabase database;

    public DataProcessor(IDatabase database)
    {
        this.database = database;
    }

    public void ProcessData(string data)
    {
        // Veri işleme işlemleri
        Console.WriteLine("Veri işlendi: " + data);
        database.SaveData(data);
    }
}

// Ana uygulama sınıfı
public class Program
{
    static void Main(string[] args)
    {
        string rawData = "Örnek veri";

        IDatabase database = new Database();
        DataProcessor processor = new DataProcessor(database);

        processor.ProcessData(rawData);

        Console.ReadLine();
    }
}




```
