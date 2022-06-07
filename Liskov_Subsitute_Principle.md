# Liskov Subsitute Principle

SOLID yazılım prensipleri diye adlandırılan ve dünya üzerinde, OOP nesne tabanlı yazılım geliştirirken kullanılan standartlaştırılmış 5 önemli tasarım ilkesi vardır. Bu ilkeler sayesinde yazılım tasarımlarını daha anlaşılır, esnek ve sürdürülebilir hale getirmek, düzgün hatasız temiz bir kod yazmak amaçlanır.  

Bu 5 tasarım ilkesi, Robert C. Martin tarafından Design Principles and Design Patterns kitabında tanıtılmıştır.  

Bu ilkelerin birlikte uygulanması sonucunda maliyet olarak çok zaman alan yazılım bakımları daha kolay hale gelmektedir.  

Bu ilkeler aşağıdaki gibidir;
1.	(S)ingle Responsibility Principle
2.	(O)pen/Closed Principle
3.	(L)iskov ‘s Substitution Principle
4.	(I)nterface Segregation Principle
5.	(D)ependency Inversion Principle    

Liskov’un yerine geçme prensibi alt sınıflardan oluşturulan nesnelerin üst sınıfların nesneleriyle yer değiştirdiklerinde aynı davranışı göstermek zorunda olduklarını söyler. Yani; türetilen sınıflar, türeyen sınıfların tüm özelliklerini kullanmak zorundadır. Eğer kullanmaz ise ortaya işlevsiz kod blokları oluşturulmuş olur.  

Türetilmiş sınıfların yazılımı geliştirilirken, türetilmiş sınıflar, temel sınıfların işlevselliğini değiştirmeden, bu sınıfların işlevselliğini genişletebilir.  

Bir üst sınıfta bulunan özellikler, kendisinden kalıtım alan alt sınıflarda kullanılmayacaksa bu durum LSP’ye aykırı bir durumdur. Yani kalıtım alınan ana sınıfın içindeki özellikler kalıtımı alan alt sınıflarda kullanılmalıdır.
Örneğin kuş isimli ana sınıfımız olsun ve bu sınıfta uç(), yürü() isimli 2 metot tanımlı olsun. Kuş ana sınıfından kalıtım alan güvercin alt sınıfını oluşturduğumuzda güvercin hem uçabilir hem de yürüyebilir hayvan olduğu için ana sınıfın özelliklerini kullanacaktır. Bu şekilde olan örnekler LSP’ye uygundur.  

Yine kuş isimli ana sınıftan kalıtım alan tavuk isimli alt sınıf olsun. Tavuk alt sınıfında yürü() metodu kullanıcaktır. Fakat tavuğun uçamadığı düşünüldüğünde uç() metodu alt sınıfta kullanılmayacaktır. İşte bu durum LSP’ye uygun değildir.
 