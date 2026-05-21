# 💅 Beauty Studio — Сайт-визитка салона красоты

Учебный проект многостраничного сайта для салона красоты. Чистый HTML/CSS/JS, без фреймворков — идеально для практики и деплоя на GitHub Pages.

## 📁 Структура проекта

```
beauty-studio/
├── index.html          # Главная страница
├── price.html          # Прайс-лист
├── gallery.html        # Галерея с каруселью
├── css/
│   └── style.css       # Все стили (тёмная тема + золото)
├── js/
│   └── script.js       # Карусель, фильтр, lightbox, анимации
├── images/             # Папка для локальных изображений (опционально)
└── README.md
```

## ✨ Функциональность

- **3 страницы:** Главная, Прайс, Галерея
- **Адаптивная вёрстка** — корректно отображается на мобильных, планшетах и десктопе
- **Фиксированный navbar** с эффектом прокрутки и мобильным burger-меню
- **Карусель** — автоплей, стрелки, точки-навигаторы, swipe на тач-устройствах
- **Фильтр галереи** по категориям (все / волосы / ногти / макияж / уход)
- **Lightbox** — полноэкранный просмотр фото по клику
- **Scroll-анимации** через Intersection Observer API
- **Плавная прокрутка** для якорных ссылок
- **CSS-переменные** — легко менять цвета и шрифты

## 🚀 Деплой на GitHub Pages

### 1. Создайте репозиторий

```bash
cd beauty-studio
git init
git add .
git commit -m "Initial commit: Beauty Studio website"
```

### 2. Создайте репозиторий на GitHub

- Зайдите на [github.com](https://github.com) → **New repository**
- Назовите, например, `beauty-studio`
- Не добавляйте README (он уже есть)

### 3. Отправьте код

```bash
git remote add origin https://github.com/ВАШ_ЛОГИН/beauty-studio.git
git branch -M main
git push -u origin main
```

### 4. Включите GitHub Pages

- Репозиторий → **Settings** → **Pages**
- Source: `Deploy from a branch`
- Branch: `main` / `/ (root)`
- Сохраните — через ~1 минуту сайт будет доступен по адресу:  
  `https://ВАШ_ЛОГИН.github.io/beauty-studio/`

## 🎨 Кастомизация

### Смена цветов (css/style.css)
```css
:root {
  --gold:         #c9a84c;   /* Основной золотой акцент */
  --bg-primary:   #0d0d0d;   /* Фон страницы */
  --text-primary: #f0ece4;   /* Цвет основного текста */
}
```

### Добавление реальных фотографий

1. Поместите фото в папку `images/`
2. Замените ссылки на Unsplash в HTML на локальные пути:
   ```html
   <!-- Было -->
   <img src="https://images.unsplash.com/..." />
   <!-- Стало -->
   <img src="images/my-photo.jpg" />
   ```

### Изменение цен (price.html)

Найдите нужный `.price-item` и отредактируйте `.price-value`:
```html
<span class="price-value">від 450 ₴</span>
```

## 🛠 Технологии

| Технология | Использование |
|---|---|
| HTML5 | Семантическая разметка |
| CSS3 | Переменные, Grid, Flexbox, анимации |
| JavaScript (ES6+) | Карусель, фильтр, lightbox, IntersectionObserver |
| Google Fonts | Playfair Display + Cormorant Garamond |
| Unsplash | Placeholder-изображения |

## 📝 Идеи для развития

- [ ] Форма записи с валидацией
- [ ] Страница "Мастера"
- [ ] Анимация при загрузке (preloader)
- [ ] Тёмная/светлая тема (toggle)
- [ ] Интеграция с Google Maps
- [ ] PWA (service worker, manifest.json)

---

Создано для практики веб-разработки ✨
