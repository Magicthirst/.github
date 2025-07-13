# Magicthirst

В данной организации представлена многопользовательская игровая платформа, построенная на микросервисной архитектуре. Платформа предназначена для поддержки многопользователських игр с синхронизацией сессий в реальном времени.
\
Изначальная курсовая для памяти сохранена здесь же [SysDesign.pdf](../SysDesign.pdf)

Репозитории (компоненты) системы:
- **[Dashboard](https://github.com/Magicthirst/host-dashboard)** — Клиентское веб-приложение для хостов игр: регистрация, настройка правил доступа, управление друзьями и бан-листами.
- **[Magicthirst - Green](https://github.com/Magicthirst/Magicthirst---Green)** — Игровой клиент на Unity, использующий инфраструктуру Magicthirst для сетевого взаимодействия.
- **[Gateway](https://github.com/Magicthirst/Service_Gateway_Py)** — Единая точка входа (API Gateway). Маршрутизирует запросы, валидирует токены, управляет сессиями.
- **[Sync](https://github.com/Magicthirst/Syncing-Battleship)** — Сервис синхронизации игровых сессий (Riptide/gRPC).
- **[Auth](https://github.com/Magicthirst/Service_Auth_Py)** — Аутентификация пользователей, выдача и проверка JWT/JWE токенов.
- **[Hosts](https://github.com/Magicthirst/Service_Hosts_Py)** — Управление настройками и списками доступа для игровых хостов.

Схема:

![Diagram Image Link](../puml/components.png)

## TODO

- [ ] Собрать всю документацию в репозиторий Magicthirst/Docs через Github Actions
- [ ] Перевести сервисы Auth и Hosts на C# для унификации стека.
- [ ] Поддержка refresh/access токенов с разными временами жизни.
- [ ] Улучшить автоматизацию деплоя и CI/CD.
