Panduan Instalasi
1. Clone Project git clone https://github.com/jikipadila-alt/utsjiki.git

2. composer install

4. Konfigurasi File Environment (env)
cp env .env
app.baseURL = 'http://localhost:8080/'

database.default.hostname = localhost
database.default.database = db_census
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi

JWT_SECRET_KEY = 'secret key'
JWT_EXPIRE_DAYS = 5



5. Jalankan Database Migration & Seeder
Untuk mengisi data dummy secara otomatis

php spark migrate
php spark db:seed DatabaseSeeder
6. Jalankan Server
php spark serve
DONE
