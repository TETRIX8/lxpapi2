
# 📚 Дневник успеваемости Newlxp

<details>
<summary><strong>🔍 Описание проекта</strong></summary>

Скрипт для автоматизированного получения данных об успеваемости из системы Newlxp через GraphQL API с возможностью:
- Авторизации в системе
- Парсинга данных по всем дисциплинам
- Удобного отображения в консоли
- Сохранения полного дампа данных

</details>

<details>
<summary><strong>🛠 Технический стек</strong></summary>

- **Node.js** (v14+)
- **Axios** (для HTTP-запросов)
- **GraphQL** (для работы с API)
- **JSON** (формат хранения данных)

</details>

<details>
<summary><strong>📦 Установка</strong></summary>

```bash
# 1. Клонировать репозиторий
git clone [ваш-репозиторий]

# 2. Перейти в папку проекта
cd diary-tracker

# 3. Установить зависимости
npm install axios
```

</details>

<details>
<summary><strong>⚙️ Настройка</strong></summary>

1. Откройте файл `h.js`
2. Заполните свои учетные данные:

```javascript
const AUTH_DATA = {
  email: "ваш@email.ru",  // Ваш учебный email
  password: "ваш_пароль"  // Пароль от ЛК
};
```

3. Сохраните изменения

</details>

<details>
<summary><strong>🚀 Запуск</strong></summary>

```bash
node h.js
```

После успешного выполнения:
- В консоли появится отчет
- Полные данные сохранятся в `diary_full.json`

</details>

<details open>
<summary><strong>📊 Пример вывода</strong></summary>

```plaintext
=== УСПЕВАЕМОСТЬ ===

📚 Математический анализ (MATH-101)
👨‍🏫 Преподаватели: Иванов Иван Иванович
⭐ Оценка: 4 (85/100 баллов)
📊 Посещаемость: 12/15 (80%)

📚 Физика (PHYS-201)
👨‍🏫 Преподаватели: Петрова Мария Сергеевна
⭐ Оценка: 5 (92/100 баллов)
📊 Посещаемость: 14/15 (93%)
```

</details>

<details>
<summary><strong>🔐 Безопасность</strong></summary>

- Все данные авторизации хранятся только локально
- Файл `diary_full.json` содержит конфиденциальную информацию
- Рекомендуется:
  - Не коммитить файл с учетными данными
  - Использовать .gitignore
  - Хранить пароли в переменных окружения

</details>

<details>
<summary><strong>🔄 Возможные доработки</strong></summary>

- [ ] Добавить фильтрацию по семестрам
- [ ] Реализовать экспорт в Excel/Google Sheets
- [ ] Добавить расчет среднего балла
- [ ] Настроить автоматические уведомления
- [ ] Создать Telegram-бота для уведомлений

</details>

<details>
<summary><strong>❓ Частые вопросы</strong></summary>

**Q:** Получаю ошибку 400 при запросе  
**A:** Проверьте:
- Актуальность API-эндпоинта
- Корректность studentId
- Срок действия токена

**Q:** Как изменить формат вывода преподавателей?  
**A:** Отредактируйте функцию `formatTeachers()` в скрипте

</details>

<details>
<summary><strong>📜 Лицензия</strong></summary>

MIT License © 2024 [Ваше имя]

</details>


### Особенности реализации:
1. **Интерактивные элементы**:
   - Все основные разделы свернуты под `<details>`
   - Раздел с примером вывода открыт по умолчанию (`<details open>`)

2. **Улучшенная структура**:
   - Добавлены новые логические разделы
   - Четкое разделение на блоки
   - FAQ для быстрого решения проблем

3. **Визуальные улучшения**:
   - Эмодзи для лучшей навигации
   - Подсветка кода в блоках
   - Чекбоксы для списка доработок

4. **Безопасность**:
   - Выделенный раздел с рекомендациями
   - Предупреждения о конфиденциальных данных

Для использования просто сохраните этот код в файл `README.md` в корне вашего проекта. При просмотре через GitHub/GitLab все раскрывающиеся блоки будут работать автоматически.
