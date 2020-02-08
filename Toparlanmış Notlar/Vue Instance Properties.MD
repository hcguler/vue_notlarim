# **el** (Connect to DOM)
- Vue instance'ın yöneteceği html DOM elementini içerir.

# **data** (Store Data to be used)
- Vue instance içinde verileri kullanmak için tanımlanan alan.

# **methods** (Methods of this Vue instance )
- Vue instance içinde kullanılacak fonksiyonların tanımlandığı alan.

# **computed** (Dpendent properties)
- Vue instance'a ait bağımlı özelliklerin tanımlandığı alandır.
- Değişken değerin yanı sıra fonksiyon da alabilir.
- Computed değerlerini metod çağırımı gibi değil değişken kullanımı gibi çağırıyoruz. Return etse dahi parantez koymaya gerek yok.
- computed içine yazılan bir fonksiyonun çalışma önceliği fonksiyondan sonradır.
- computed içinde değer veya fonksiyonun tetiklenmesi için içinde kullanılan bir değeri etkiliyor olması gerek. Eğer içinde bulunan değer dışında bir tetikleme gerçekleşirse computed metod çağrımı yapılmaz.
- Render işlemi tamamlandıkan sonraki yaşam döngüsü anına işaret eder.
- Computed property ile template içerisinde normal property işlemlerinde olduğu gibi data-bind işlemleri yapmak mümkün.
- Vue instance computed içinde kullanılan değişkenlerin bağlı olduğu data değerlerinin bilincinde olduğu için güncellemeyi ve method çağırımını yönetebiliyor.
- computed property ön tanımlı olarak getter tanımlıdır. Ancak, ihtiyaç halinde setter tanımlanabilmektedir.
- computed property bağlı olduğu değişkeni ekranda sunarken **ön belleğe (cache)** de alır ve bu değişken değişmediği sürece tekrar hesaplama yapmaz.
- Computed properties her zaman bir değer döndürmek (return) ve eş zamanlı olmak durumundadır.
- **computed properties diğer verilerden türetilmiş yeni veriler oluşturmak istendiğinde öne çıkmaktadır. Bu verileri dönüştürmek (transform), filtrelemek (filter) ya da değiştirmek (manipulate) istediğimizde rahatlıkla kullanabiliriz.**
- synchronous işlemler için kullanılan cachable işlemleri içerir.

# **watch** (Execute code upon data changes)
- Data değişikliğini gözlemlemek ve bunlara tepki vermek için kullanılan property'dir.
- Componenti içeren data değerleri her değişikliğe uğradığında yakalanır ve tetiklenir.
- Bir data farklı bir dataya bağlı ise `this.fullName=this.name+" "+this.surName` gibi name veya surName değişikliklerini handle etmek için watch kullanılmalıdır.
- **asynchronous ve bütçeli operasyonlardaki veri değişikliklerinin takibinde watch değerlendirilebilir bir seçenektir**

# **template** (insert html block in vue instance)
- Vue instance içeriğini ezerek verilmiş html değerlerin render edilmesini sağlarız.
- el değerine specific html component id bilgisi verilmeden bir isimlendirme yapılarak oluşturulmuş temlate ile yeni bir component oluşturulabilir.

# **beforeCreate**
- Instance create edilmeden önce yapılacak işlemleri tetikleyen fonksiyondur.

# **created** 
- Instance create edilirken yapılacak işlemleri tetikleyen fonksiyondur.

# **beforeMount**
- Mount edilmeden yani bir html element için atama yapılmadan önce yapılacak işlemleri tetikleyen fonkisyondur.

# **mounted**
- Mount edilirken yapılacak işlemleri tetikleyen fonksiyondur.

# **beforeDestroy**
- Instance yıkıma uğramadan önce yapılacakları tetikleyen fonksiyondur.

# **destroyed**
- Instance yıkıma ugrarken yapılacakları tetikleyen fonksiyondur.

# **components**
- Vue instance içinde kullanılacak local vue componentlerin isim ve defination şeklinde değerini tutar.

# **props**
- Hazırlanmış vue component için dışarıdan alınacak property değerlerini dizi olarak sunar.

# **deacticated**
- Dinamik olarak gösterilen componentlerde keep-alive olarak aktif yaşamı devam ettiriliyorsa, gösterimden kalktığı durumda işlem yapmak için kullanılır.

# **directives**
- local olarak vue instance içerisinde tüm html domlarında kullanılabilir v- prefix ile başlayan directives tanımı yapılmasını sağlar.






