# **Environment Variable**
- .env dosyası oluşturulur. Cli bu dosyayı tanır ve tüm vue instance için erişilebilir hale getirir.
- key=value şeklinde global variable eklemesi yapılır.
- process.env.key_name ile tüm vue instace içinde erişim sağlanabilir.
- Bu değer alınarak ilgili vue instance içinde bir veriye aktarılabilir.
- .env.development .env.production .env.test gibi ayrı dosyalar oluşturulup mode verilerek environment variable tanımı yapılabilir.
- Hangi dosyadan okuyacağını package.json içindeki scriptler ile `--mode development` belirtiyoruz. Default production olarak ele alınır.

# **Vue js Build Target**
- Vue App
    - vue build --target app
    - Normal Vue App Bundle
    - Includes your Code + Vue Framework
- Vue Library
    - vue build --target lib
    - A distributable Vue Library Bundle
    - Only includes your Code Not the Vue Framework
- Web Component
    - vue build --target wc
    - A distributable Web Component
    - Only include your Code.Not the vue framework
    - Can be dumped into any page where you import Vue
- Yapılan build output dizini dist dizini altındadır. Her build farklı dosya oluşturur.

# **Vue js Deployment**
- npm run build
- dist/build.js 
- deploy any server build.js (included all code)
- Sadece build.js ve index.html dosyası ile deploy edilebilecek platformlar var.
- webpack config içinde deployment ayarlamaları yapılıyor.
- deploy ederken build.js dosyasını index.html içinde nasıl referance verildi ise o şekilde dizin oluşturulmalı.


