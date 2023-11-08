## Aşağıdaki işlemleri sırasıyla terminal kullanarak gerçekleştirin.

### Aşağıdaki komut postgres kullanıcısına bağlanıp "bulutdb" adında bir veritabanı oluşturmaya yarar.
su - postgres -c "psql -U postgres -c 'CREATE DATABASE bulutdb;'"

### Bu komut ise postgres kullanıcısına ve oluşturulan bulutdb veritabanına bağlanıp içerisinde init.sql dosyasını çalıştırır.
su - postgres -c 'psql -U postgres -d bulutdb -f /tmp/postgres-initsql/init.sql'
