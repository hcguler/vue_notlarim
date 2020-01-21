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