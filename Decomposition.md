# Decomposition (Ayrıştırma)

Problem alanındaki ilgili varlıkların tespit edilip, doğru nesneler biçiminde ifade edilmesidir. Bir yöntem olarak da nitelendirilebilecek ayrıştırma, sistemdeki karmaşıklıkla (complexity) başa çıkabilmek için yapılır. Buna kısaca böl ve fethet (divide and conquer) denilmektedir.  

## Nesneye Yönelik Analiz Ve Nesneye Yönelik Tasarım  

Problem birbirinden bağımsız nesneler olarak ifade edilmelidir. İlgi alanı nesnelere göre ayrılmalı ve her nesnenin belirli nitelikleri ve davranışları olmalıdır.  

Nesneye yönelik analiz soyutlama, miras alma ilkelerinin üzerine kuruludur. Bu ilkelerden soyutlama karmaşık bir problemi, sistemi, fikri ya da durumu daha iyi anlayabilmek belirli yönleri ile ele almayı ifade eder. Analistin bakış açısı, sistem nesnelerinin en belirgin olan benzer nitelikleri üzerine odaklanır. Sistem böylece basit bir şekilde ifade edilebilmektedir.  

## Yapısal Analiz Ve Yapısal Tasarım  
 
Kullanılan çeşitli yapısal analiz ve tasarım yöntemleri arasında en popüler olanlardan birisi İşlevsel ayrıştırma (Functional decomposition)’dır.   

İşlevsel ayrıştırma, sistemin yerine getirmesi gereken işlevler, alt işlevler ve bu işlevlerin arasındaki ara yüzlerle ilgilenir. Problemi, daha kolay ele alınabilecek alt problemlere bölme ve bu alt problemlerin çözümlerinden esas problemi çözmeye yarayan tekniktir. İşlevsel ayrıştırma yukarıdan aşağıya geliştirme yöntemidir.   

Soyut ürünle başlayıp, somut ürüne doğru çalışır. Süreç, işlevin alt adımlara bölünmesiyle başlar.
Daha sonra her bir alt adım kendi içinde alt adımlara bölünerek devam edilir. Alt adımlara bölme daha fazla alt adıma bölünemeyecek bir alt adıma ulaşıldığında son bulur.

