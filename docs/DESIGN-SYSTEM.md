# DESIGN SYSTEM — основа (PHASE 5)

Дата: 2026-10-18
Статус: ✅ УТВЕРЖДЕНА проектная база (решение владельца 2026-10-18: направление A + слой B); допускается уточнение токенов на следующих этапах без изменения утверждённого характера.
Это НЕ техническая реализация: CSS-код не писался, сайт не изменялся.

---

## 1. Design Tokens

### Colors
| Токен | HEX | Роль |
|---|---|---|
| `--bg` | `#F7F4EE` | основной фон (warm paper) |
| `--surface` | `#FFFFFF` | карточки, плашки, формы |
| `--text` | `#211C15` | основной текст |
| `--muted` | `#6E665B` | вторичный текст, ID, подписи |
| `--border` | `#DCD5C8` | разделители 1 px |
| `--primary` | `#24352A` | cedar dark: тёмные секции, primary CTA, footer |
| `--primary-hover` | `#1B2820` | hover primary |
| `--accent` | `#8F6A3F` | ссылки-акценты, hover, inquiry CTA (≥4.5:1 на белом) |
| `--accent-tint` | `#E9DFCE` | подложки акцентов, focus ring |
| `--dark-bg` | `#1C2320` | hero-скрайм, full-bleed тёмные секции |

### Typography (утверждённая пара: Cormorant Garamond + Inter; альтернативы — см. DESIGN_DIRECTION §5)
| Токен | Шрифт / вес | Desktop | Mobile | Интерлиньяж | Трекинг |
|---|---|---|---|---|---|
| `--font-display` | Cormorant Garamond 500 | 72–96 | 40–52 | 1.02 | −0.5–1% |
| `--font-h1` | Cormorant Garamond 500 | 48–64 | 30–36 | 1.1 | −0.5% |
| `--font-h2` | Cormorant Garamond 500 | 32–40 | 24–28 | 1.15 | 0 |
| `--font-h3` | Inter 500 | 20–24 | 18–20 | 1.3 | +0.2% |
| `--font-body` | Inter 400 | 17–18 | 16 | 1.65 | 0 |
| `--font-caption` | Inter 400 | 12–13 | 12 | 1.5 | +0.5% |
| `--font-ui` | Inter 500 | 14–16 | 14–15 | 1.2 | +0.5–1% |

### Spacing (base 4)
`4 · 8 · 16 · 24 · 32 · 48 · 64 · 96 · 128 · 160` px.
Section rhythm: desktop 96–160; mobile 48–64.

### Grid
| Брейкпоинт | Колонки | Max-width | Gutters | Поля |
|---|---|---|---|---|
| ≥1200 px (desktop) | 12 | 1360 | 28–32 | 40–64 |
| 768–1199 (tablet) | 8 | — | 24 | 32 |
| ≤767 (mobile) | 4 | — | 16 | 20 |

### Image ratios
hero 21:9 (desktop) / 4:5 (mobile); карточка 4:5; PDP галерея 4:3, 3:2; макро 1:1 / 3:2.

### Motion tokens
| Токен | Значение |
|---|---|
| `--dur-fast` | 200 ms |
| `--dur-base` | 400 ms |
| `--dur-slow` | 600–900 ms |
| `--ease` | cubic-bezier(0.22, 1, 0.36, 1) (ease-out) |

---

## 2. Components (спецификация)

### Buttons
- **Primary:** filled `--primary`, текст `#F7F4EE`, радиус 2–4 px, padding 16/28, hover `--primary-hover`; без теней.
- **Secondary:** 1 px `--border`, фон прозрачный, текст `--text`, hover: border `--accent`, текст `--accent`.
- **States:** hover 250 ms; focus-visible кольцо 2 px `--accent-tint` + offset 2 px; disabled opacity 0.4.
- Не e-commerce: без негативных теней, без градиентов, без «кричащих» заливок.

### Links
- Текстовая ссылка: `--text`, стрелка →; hover `--accent` + underline.
- В тексте: underline только hover.

### Cards (product card)
- Фон `--surface` или прозрачный на `--bg`; рамки нет (либо 1 px `--border` в сетке каталога).
- Контент: изображение 4:5 → название (H3 антиква) → ID/категория (caption muted) → размеры (body) → цена (Inter 500).
- Hover: image scale 1.02–1.03 (`--dur-base`), название → `--accent`.
- Вся карточка кликабельна; на mobile hover нет.

### Image treatment
- Full-bleed для hero и тёмных секций; скрайм `--dark-bg` градиент 25–35% снизу для читаемости.
- Без тяжёлых фильтров; допустима лёгкая цветокоррекция к единому тёплому тону (реальные фото, конструкция изделий не меняется).

### Forms (заявка)
- Поля: фон `--surface`, border 1 px `--border`, радиус 2–4 px, label caption над полем.
- Focus: border `--accent` + кольцо `--accent-tint`.
- Submit — Primary CTA; рядом текстовая ссылка «Задать вопрос» (mailto).
- На карточке изделия форма предзаполняется ID.

### Navigation
- Header 72 px (mob 56): прозрачный над hero → `--bg` + border при скролле; меню `--font-ui`.
- Mobile menu: полноэкранный overlay `--primary`, пункты display-антиквой, CTA внизу.
- Breadcrumbs: caption, `--muted`.
- Footer: фон `--primary`, текст off-white/muted.

### States (глобально)
hover / focus-visible / active / disabled для всех интерактивных элементов; touch targets ≥44 px; `prefers-reduced-motion` отключает анимации.

---

## 3. Принципы использования

1. Два шрифтовых семейства максимум; палитра только из токенов; отступы только из шкалы.
2. Акцент `--accent` — дозированно (ссылки, hover, мелкие элементы), не фонами больших площадей.
3. Фотография первична; декоративные элементы минимальны (рамки 1 px, скраймы).
4. Компонент не добавляется без NEED; не создаём UI ради количества.
5. Любое отклонение от токенов — только с обоснованием и фиксацией в этом документе.
