# Flower Shop "Flowers by Sabi" - Торговая система цветочного магазина

## 1. Описание проекта

**Flower Shop "Flowers by Sabi"** - это полнофункциональная веб-приложение для управления цветочным магазином, построенное на современном стеке технологий. Система обеспечивает полный цикл управления торговыми операциями: от учета товаров и поставщиков до обработки продаж и анализа клиентской базы.

### Решаемые проблемы:
- Устранение ручного учета и бумажной работы
- Контроль за наличием цветов, букетов и сопутствующих товаров
- Ведение истории покупок, персональных скидок и предпочтений клиентов
- Мониторинг эффективности товаров и категорий
- Автоматическое отслеживание закупок и остатков

### Ценность проекта:
- Повышение эффективности управления, снижение ошибок при учете, увеличение продаж за счет анализа данных
- Упрощение процессов продаж, быстрый доступ к информации о товарах
- Улучшенный сервис, персональные предложения, прозрачность цен и наличия товаров

## 2. Инструкции по установке

### Предварительные требования
- Node.js (версия 14 или выше)
- PostgreSQL (версия 12 или выше)
- npm или yarn

#### Шаг 1: Клонирование репозитория
```bash
git clone https://github.com/sssabbe/flower
cd flower
Шаг 2: Установка зависимостей
bash
npm install
Шаг 3: Настройка базы данных
Создайте базу данных в PostgreSQL:

sql
CREATE DATABASE trade_app_db;
Настройте переменные окружения. Создайте файл .env в корне проекта:

text
DB_HOST=localhost
DB_USER=postgres
DB_PASSWORD=SaaaBee08642
DB_NAME=trade_app_db
DB_PORT=5432
NODE_LOCAL_PORT=8080
Шаг 4: Запуск сервера
bash
npm start
Шаг 5: Запуск приложения
bash
npm run dev
Приложение будет доступно по адресу: http://localhost:8080

3. Использование
Запуск приложения
bash
npm start
Структура проекта
text
flower-shop/
├── app/
│   ├── controllers/     # Контроллеры (бизнес-логика)
│   ├── models/         # Модели Sequelize
│   └── routes/         # Маршруты API
├── config/             # Конфигурация
├── public/             # Статические файлы
│   ├── index.html     # Главная страница
│   ├── style.css      # Стили
│   └── script.js      # Фронтенд скрипты
├── .env               # Переменные окружения
├── server.js          # Точка входа
└── package.json       # Зависимости
Пример работы с API
Получение всех товаров
javascript
fetch('/api/products')
  .then(response => response.json())
  .then(data => console.log(data));
Создание нового товара
javascript
fetch('/api/products', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
  },
  body: JSON.stringify({
    article: 'rose_red_01',
    product_name: 'Красная роза',
    category_code: 1,
    supplier_code: 1,
    price: 150.00
  })
});
4. Вклад
Процесс внесения изменений
Создайте ветку для вашей фичи:

bash
git checkout -b feature/AmazingFeature
Сделайте коммит изменений:

bash
git commit -m 'Add some AmazingFeature'
Запушьте в вашу ветку:

bash
git push origin feature/AmazingFeature
5. Документация
База данных: PostgreSQL с Sequelize ORM

Бэкенд: Express.js + Node.js

Фронтенд: HTML + CSS + JavaScript

ORM: Sequelize для работы с PostgreSQL

6. Лицензия
Разрешается:
Использование в коммерческих целях

Модификация и распространение

Частное использование

Требуется:
Сохранение уведомления об авторских правах и лицензии

Запрещается:
Ответственность автора

Гарантия работы

7. Контактная информация
Разработчик
Имя: Абибулаева Сабина

Email: sabi.abibulaeva@mail.ru

GitHub: @sssabbe

Телефон: +7 979 001-76-10

8. Благодарности
Express.js - Веб-фреймворк для Node.js

Sequelize - ORM для Node.js

PostgreSQL - Реляционная база данных

pgAdmin - Администрирование PostgreSQL
