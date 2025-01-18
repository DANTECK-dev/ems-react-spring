# EMS Frontend

Это фронтенд-приложение для управления сотрудниками, реализованное с использованием React. Оно взаимодействует с серверной частью, построенной на Spring Boot, и базой данных MySQL. Приложение позволяет добавлять, изменять и удалять информацию о сотрудниках.
>Ссылка на [BackEnd](https://github.com/DANTECK-dev/ems-springboot-react-backend) 

## Стек технологий

- **React**: Основной фреймворк для разработки пользовательского интерфейса.
- **Axios**: Библиотека для выполнения HTTP-запросов к API.
- **React Router DOM**: Для управления маршрутизацией в приложении.
- **Bootstrap**: Для стилизации компонентов и создания адаптивного дизайна.

## Основные возможности

1. **Добавление сотрудников**:
   - Форма для ввода имени, фамилии и email сотрудника.
   - Отправка данных на сервер через API.

2. **Редактирование сотрудников**:
   - Возможность выбора сотрудника из списка.
   - Обновление данных через соответствующую форму.

3. **Удаление сотрудников**:
   - Кнопка для удаления сотрудника из базы данных.
   - Отправка DELETE-запроса на сервер.

4. **Список сотрудников**:
   - Отображение всех сотрудников, полученных из базы данных MySQL.
   - Адаптивный интерфейс для удобной работы на различных устройствах.

## Установка и запуск

### 1. Клонирование репозитория

```bash
git clone https://github.com/your-repository/ems-frontend.git
cd ems-frontend
```

### 2. Установка зависимостей

Убедитесь, что у вас установлен Node.js. Затем выполните команду:

```bash
npm install
```

### 3. Запуск приложения

```bash
npm start
```

Приложение будет доступно по адресу [http://localhost:3000](http://localhost:3000).

## Конфигурация

Для взаимодействия с сервером необходимо указать базовый URL API. Это можно сделать в файле `src/services/EmployeeService.js`:

```javascript
import axios from "axios";

const EMPLOYEE_API_BASE_URL = 'http://localhost:8080/api/v1/employees';

const  EmployeeService = {
    //////////////////////////////
};

export default EmployeeService;
```

## Структура проекта

- **`src/components`**: Компоненты React.
- **`src/services`**: Конфигурация API и взаимодействие с сервером.

## Скрипты

- `npm start` — Запуск приложения в режиме разработки.
- `npm run build` — Сборка приложения для продакшена.
- `npm test` — Запуск тестов.

## Зависимости

- `axios` — Для выполнения HTTP-запросов.
- `react-router-dom` — Для маршрутизации.
- `bootstrap` — Для стилизации.
- `react` и `react-dom` — Основные библиотеки React.

## Лицензия

Этот проект распространяется под лицензией MIT. Подробности смотрите в файле [LICENSE](LICENSE).

## Связь

Если у вас возникли вопросы или предложения, свяжитесь с нами по адресу: **[lol@kek-work.ru](mailto:lol@kek-work.ru)**.
