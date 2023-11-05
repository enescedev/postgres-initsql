# postgres-initsql

# Veri tabanına erişebilmek için postgres kullanıcısının şifresini değiştir.
su - postgres -c "psql -U postgres -c \"ALTER USER postgres WITH PASSWORD 'postgres';\""

# "bulutdb" adında bir veritabanı oluştur
su - postgres -c "psql -U postgres -c 'CREATE DATABASE bulutdb;'"

# "bulutdb" veritabanına bağlan ve init.sql dosyasını çalıştır
su - postgres -c 'psql -U postgres -d bulutdb -f /home/mock/init.sql'