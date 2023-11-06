# postgres-initsql

# "bulutdb" adında bir veritabanı oluştur
su - postgres -c "psql -U postgres -c 'CREATE DATABASE bulutdb;'"

# "bulutdb" veritabanına bağlan ve init.sql dosyasını çalıştır
su - postgres -c 'psql -U postgres -d bulutdb -f /tmp/postgres-initsql/init.sql'