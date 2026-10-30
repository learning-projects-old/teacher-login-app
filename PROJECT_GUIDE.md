# Путеводитель: login_app

Автономная инструкция: достаточно этой папки, исходников и перечисленных защищённых копий. История чатов и центральный каталог не требуются.

[Восстановление](RECOVERY.md) · [Карта файлов и зависимостей](PROJECT_MAP.json)

## Назначение

Достоверное описание назначения в изученных документах не найдено. Ниже приведены проверенные файлы; не определяйте назначение только по имени папки.

Обнаруженные языки: JavaScript, Vue SFC.

## Порядок чтения

1. Локальные AGENTS.md / CLAUDE.md и документы ниже.
2. Манифесты: версии среды, зависимости, команды.
3. Кандидаты точек входа; фактический запуск проверить по манифесту.
4. PROJECT_MAP.json: imports_local от источника к импортируемому файлу; входящие рёбра — потребители модуля.
5. RECOVERY.md: независимые данные, восстановление среды, запуск и критерии приёмки.

- [client/README.md](client/README.md)
- [vuex-app/README.md](vuex-app/README.md)

## Манифесты

- [client/package.json](client/package.json)
- [server/package.json](server/package.json)
- [vuex-app/package.json](vuex-app/package.json)

## Кандидаты точек входа

- [client/src/main.js](client/src/main.js)
- [server/server.js](server/server.js)
- [vuex-app/src/main.js](vuex-app/src/main.js)

## Основные файлы по локальным импортам

| Файл | Входящих импортов |
|---|---:|
| [client/src/views/AboutView.vue](client/src/views/AboutView.vue) | 1 |
| [client/src/App.vue](client/src/App.vue) | 1 |
| [client/src/router.js](client/src/router.js) | 1 |
| [client/src/views/HomeView.vue](client/src/views/HomeView.vue) | 1 |
| [client/src/views/LoginView.vue](client/src/views/LoginView.vue) | 1 |
| [client/src/views/NotFoundView.vue](client/src/views/NotFoundView.vue) | 1 |
| [vuex-app/src/components/Counter.vue](vuex-app/src/components/Counter.vue) | 1 |
| [vuex-app/src/components/CounterButtons.vue](vuex-app/src/components/CounterButtons.vue) | 1 |
| [vuex-app/src/components/TodoInput.vue](vuex-app/src/components/TodoInput.vue) | 1 |
| [vuex-app/src/components/TodoList.vue](vuex-app/src/components/TodoList.vue) | 1 |
| [vuex-app/src/style.css](vuex-app/src/style.css) | 1 |
| [vuex-app/src/App.vue](vuex-app/src/App.vue) | 1 |

## Проверки


## Чтение карты без специальных плагинов

PROJECT_MAP.json — UTF-8 JSON: nodes и edges. Пути файлов относительные. contains обозначает наличие файла; imports_local — статически распознанный импорт; declares_dependency — объявление пакета в манифесте. evidence содержит источник и, где доступно, строку. Карта не исполняет код.

Статус исходного анализа: static-scan-complete; ограничений чтения: 0. Исходный снимок: 2026-10-30T14:47:11.360Z.

После изменения кода перечитайте затронутые файлы: карта является снимком. Отсутствие ребра не доказывает отсутствие зависимости.
