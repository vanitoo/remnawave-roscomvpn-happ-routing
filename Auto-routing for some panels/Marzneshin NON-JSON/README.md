# Добавление роутинга `RoscomVPN` в Marzneshin для пользователей обычных подписок (не JSON)
- Положите файл subscription.py в `/var/lib/marzneshin`
- Прилинкуйте файл строкой `- /var/lib/marzneshin/subscription.py:/app/app/routes/subscription.py` в конец файла `/etc/opt/marzneshin/docker-compose.yml`
- Перезагрузите Marzneshin - `marzneshin restart`
- Готово! Теперь в Happ вместе с подписками поставляется всегда свежий роутинг `RoscomVPN`
