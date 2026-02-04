# Effective Mobile — DevOps Test Task

## Описание

Данный проект представляет собой решение тестового задания на позицию DevOps.

Развёртывается простое backend-приложение, доступное пользователю через nginx.
Все компоненты запускаются в Docker-контейнерах и управляются с помощью Docker Compose.

Архитектура решения:

client - nginx (порт 80) - backend (Python HTTP server, порт 8080)

---

## Структура проекта

├── backend/
│ ├── Dockerfile
│ └── app.py
├── nginx/
│ └── nginx.conf
├── docker-compose.yml
└── README.md

---

## Запуск проекта

docker compose up --build

# Проверка
curl http://localhost

Ответ: Hello from Effective Mobile!


