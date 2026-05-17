# opendk_docker
opendk docker compose
docker/README.md
markdown
# OpenDK Docker Setup

## Struktur
- `project/` → source code OpenDK
- `docker/` → konfigurasi Docker

## Cara Menjalankan
1. Clone OpenDK ke folder `project/`
   ```bash
   git clone https://github.com/OpenSID/OpenDK.git project
2. Jalankan Docker
docker-compose up -d --build

3. Generate APP_KEY
docker exec -it opendk-app php artisan key:generate

4. Migrasi database
docker exec -it opendk-app php artisan migrate --seed

5. Akses aplikasi di browser: http://localhost:9011

Akun Default
Email: admin@mail.com
Password: password

