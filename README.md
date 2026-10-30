### Алексей Русских — разработчик ИИ-агентов (Python, LLM)

Делаю ИИ-агентов, которые работают в реальных процессах: собирают данные из документов,
фото и голоса, сверяют их с правилами и сами вносят результат в корпоративные системы.
Человек подтверждает ключевые шаги. 15+ лет в IT, от администрирования серверов до
продакшена LLM-сервисов.

## Основные проекты

**[LibraCalc](https://github.com/AI-bot-service/libra-calc-showcase)** · [libracalc.ru](https://libracalc.ru)<br>
Дневник для семей с диабетом 1 типа. По фото тарелки, упаковки или меню столовой ИИ считает
углеводы и ХЕ, данные датчика глюкозы приходят через LibreLinkUp и Nightscout, врачу — PDF-отчёт.
Модель распознаёт только состав, углеводы считает код по справочникам. Две цепочки фолбэка —
моделей и провайдеров — с общим состоянием в Redis и алертами в Telegram.
`FastAPI` `Celery` `PostgreSQL` `Next.js` `Vision LLM` `JSON Schema` `aiogram`

**[ИИ-агент страхования имущества для СОГАЗ](https://github.com/AI-bot-service/sogaz-insurance-agent-showcase)**<br>
Бот в Telegram и MAX консультирует клиента по документам продукта (RAG), собирает данные
заявки по чек-листу текстом, голосом и фото (tool-calling), а Windows-агент на Playwright
сам заполняет форму в кабинете страховой в сессии агента. Заявка уходит сделкой в amoCRM,
менеджер получает уведомления на каждой передаче.
`FastAPI` `pgvector` `OpenAI` `Whisper` `Playwright` `amoCRM` `DaData`

## Другое

- [repair_bot_public](https://github.com/AI-bot-service/repair_bot_public) — бот приёма заявок на ремонт: голосовые с расшифровкой, чат клиента с мастером, защита от спама
- [efir](https://github.com/AI-bot-service/efir) — мобильный клиент видеоконференций на Jitsi (React Native)
- [AI-Agent-Tasks-Public](https://github.com/AI-bot-service/AI-Agent-Tasks-Public) — планировщик задач в Telegram
- [whisper-offline](https://github.com/AI-bot-service/whisper-offline) — локальное распознавание речи

## Стек

- **Backend:** Python, FastAPI, aiogram 3, Celery, SQLAlchemy 2 + Alembic, PostgreSQL + pgvector, Redis
- **ИИ:** LLM через OpenAI-совместимые API с фолбэком между провайдерами; RAG, vision/OCR, Whisper, структурированный вывод, tool calling, свои бенчмарки моделей
- **Frontend:** Next.js, React, TypeScript, Tailwind, PWA, Telegram Mini App
- **Автоматизация:** Playwright (RPA в веб-кабинетах), интеграции с CRM, боты Telegram и MAX
- **Инфраструктура:** Docker Compose, Traefik, Linux, GitHub Actions, non-root контейнеры, CVE-аудит (trivy, OSV, gitleaks)
- **Разработка:** Claude Code

## Связь

Telegram: [@Rubitco1](https://t.me/Rubitco1)
