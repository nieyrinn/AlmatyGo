# AlmatyGo — iOS Application
<img src="https://github.com/user-attachments/assets/20749ee4-340a-431b-9ef8-257c27a512a4" width="120" />


## Project Overview

**AlmatyGo** — iOS-приложение для жителей и гостей Алматы, предназначенное для поиска подходящих мест для отдыха, развлечений, прогулок на природе и других активностей.

Приложение помогает пользователю быстро найти оптимальное место по категории, средней цене и личным предпочтениям, а также сохранить понравившиеся места в избранное.

Проект реализован с использованием **UIKit** и **Storyboards**.

---

## Features

### Places Browsing
- Список из **50 популярных мест Алматы**
- Данные загружаются из сети
- Используется `UITableView` с кастомными ячейками

### Categories Filter
- Фильтрация по **5 категориям**
- Реализована через `UISegmentedControl`

### Search
- Поиск по названию, типу и адресу
- Реализован с помощью `UISearchController`

### Favorites
- Добавление и удаление мест в избранное
- Отдельный экран Favorites
- Сохранение избранных мест через `UserDefaults`

### User Profile & Settings
- Профиль пользователя (имя и описание)
- Настройки:
  - максимальная средняя цена
  - флаг `Only open`
- Максимальная цена выбирается через `UISlider` с шагом
- Все настройки сохраняются локально

### Price Filtering
- Фильтрация мест по максимальной средней цене
- Применяется автоматически при возврате на экран списка или можно через кнопку Refresh

### Refresh Data
- Кнопка обновления данных
- Повторный сетевой запрос по нажатию пользователя

### User Feedback
- Alert при сетевой ошибке

### Animations
- Анимация при добавлении/удалении из избранного
- Плавная анимация смены изображений на экране деталей

---

## Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/7ad22332-80e7-49b4-8960-ba16bd0e3260" width="200" />
  <img src="https://github.com/user-attachments/assets/86768d14-fd8b-4e3f-86ee-fc269dd20f54" width="200" />
  <img src="https://github.com/user-attachments/assets/d6c43aa2-d4ca-4cb0-8fbf-34cf6b511490" width="200" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/94a01be7-8d14-4d9c-a9c1-f88ec91ca1bd" width="200" />
  <img src="https://github.com/user-attachments/assets/89725d1e-dac9-4007-8318-3936ddf9af2d" width="200" />
</p>

---

## Technical Details

- **Platform:** iOS
- **Language:** Swift
- **UI Framework:** UIKit
- **Layout:** Storyboards + Auto Layout
- **Networking:** URLSession
- **Data Parsing:** Codable + JSONDecoder
- **Local Storage:** UserDefaults
