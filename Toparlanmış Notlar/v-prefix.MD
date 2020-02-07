# **v-html**
- herhangi bir html elementi içinde vue instance için tanımlanmış data değerinde html içerik gösterilebilir.
- dikkat edilmesi gereken bu data değişkeni içindeki bilgi kullanıcı tarafından oluşturulan bir içerik ise cross-site scripting yapılabileceği için kullanılmamalıdır.

# **v-bind**
- Vue instance içindeki bir data değerinin verildiği html attribute değerine bind edilmesini sağlar.
- property önüne ":" konularak kullanım yapılabilir. okunabilirliği daha iyidir.

# **v-on**
- Vue instance içindeki bir method'un verildiği html attribute değeri ile tetiklenmesini sağlar.
- property önüne "@" konularak kullanım yapılabilir. okunabilirliği daha iyidir.

# **v-model**
- Data değerine set edilen verilerin html component için model tanımıdır.
- Set edilen değer her değiştiğinde ilgili html DOM güncellenmektedir.

# **v-if**(attaches or detaches an element)
- Bir html elementinin belirtilen koşula göre görüntülenme durumudur. 
- Enable, disable değil browser üzerinde render etme durumunu belirler.
- Belirtilen state false ise tamamen html element oluşturulmaz ilgili sayfa için silinir.
- F12 ile bakıldığında ilgili component için satatement false ise sadece <!----> şeklinde yorum satırı koymaktadır.
- v-if konulmuş bir html component içindeki tüm nested componentler false durum için silinir.

# **v-else-if**
- vue js 2.1.0+ versiyonlar için kullanılır.
- Birden fazla if statement için kullanılır.

# **v-else**
- if else yapısı ile aynıdır veriln statement'ın false oludğu durumi için görüntülenir. Aynı if gibi çalışır.s
- v-else-if ile kullanılıyor ise tüm statement'ların dışındaki durum için girecektir.
- herhangi bir attribute değeri almamaktadır.
- <div v-else> gibi kullanılmaktadır.
- hiyerarşik olarak aynı seviyerde bulunan html elementi için kullanılan v-if için else ifadesi oluşturur.

# **v-show**
- html dom elementi kaynak html de kalmaya devam edecek şekilde show-hide durumunu yönetir.
- Bu işlemi style="style="display: none;"" ekleyerek yapar.
- Kaynak kod içinde bu bilginin görüntülendiği unutulmamalıdır.
- Özel durumlar için bir grup html elementin oluşturulup silinmesi yapılmadan show-hide yapılması içini kullanılabilir.
- performans olarak kesinlikler v-if daha başarılıdır.

# **v-for**
- bir veri veya kritere göre döngü olarak html dom oluşturmak için kullanılır.
- v-for içinde index almak için index tutacak değişken ile liste verilmelidir. `v-for="(value_of_the_element, index) in list_of_element">`
- object v-for verildiğinde "." kullanılarak properties yazdırılabidiği gibi obje verilerini de döngü ile kullanarak yazdırabiliriz.
- object fields yazdırılırken key ihtiyacı var ise  (field_value, field_name) olarak verilmelidir.
- belirli bir sayı kadar döngü oluşturmak için v`-for="n in 10"` kullanılır.
- vue içinde kullanılan array ler için sağlanan fonksiyonalite
   - push()
   - pop()
   - shift()
   - unshift()
   - splice()
   - sort()
   - reverse()
   
# **v-model**
- Data alanında tutulan bir bilginin input field üzerinden alınmasını sağlar.