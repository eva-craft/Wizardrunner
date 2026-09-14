# 🧙‍♂️ Wizardrunner / Волшебный Бегун

---

## 🇷🇺 Русское описание

### Общая концепция
**Wizardrunner** — это бесконечный раннер с голосовым управлением заклинаниями. Вы играете за волшебника, который бежит по семи магическим мирам, уворачивается от препятствий, собирает монеты и произносит заклинания голосом, чтобы выжить и пройти все уровни.

### Управление
| Действие | Как выполнить |
|---|---|
| Прыжок | Тап по экрану / Пробел / Стрелка вверх |
| Двойной прыжок | Двойной тап по экрану |
| Заклинания | Голосовые команды через микрофон |

### Заклинания (голосовые команды)
| Фраза | Эффект | Длительность |
|---|---|---|
| **«Фокус Покус»** | Бесплотность — неуязвимость ко всем препятствиям | 15 сек |
| **«Абракадабра»** | Уничтожает ближайшее препятствие впереди | Мгновенно |
| **«Магнифико»** | Притягивает все монеты в радиусе | 10 сек |
| **«Темпус»** | Откат во времени на 7 секунд назад (позиция, здоровье, монеты) | Мгновенно |
| **«Торнадо»** | Ураган, уничтожающий до 3 препятствий впереди | ~2.5 сек |
| **«Левитация»** | Полёт над землёй, неуязвимость | 10 сек |
| **«Сангуис»** | Самоисцеление: +1 сердце | Мгновенно |

### Здоровье и урон
- У волшебника **5 сердец**.
- При столкновении с препятствием (не в режиме неуязвимости):
  - Теряется 1 сердце.
  - Наложен эффект **конфузии** на 2 секунды — маг двигается хаотично, не может прыгать, управление затруднено.
  - Даётся **неуязвимость на 2.5 секунды** (мигание).
- При 0 сердцах — игра окончена.

### Уровни (7 миров)
| № | Название | Цель (метры) | Особенности |
|---|---|---|---|
| 1 | 🌙 Волшебная Ночь | 1500 | Ночной лес, камни, шипы, кристаллы |
| 2 | 🏜 Пустыня Кудесников | 2100 | Кактусы, песчаные башни, быстрее |
| 3 | 🏰 Академия Волшебства | 2700 | Книжные полки, котлы, кристаллы |
| 4 | 🌋 Вулкан Колдунов | 3300 | Лавовые озёра, магмовые валуны, шипы |
| 5 | 💀 Храм Некромантов | 3900 | Костяные алтари, черепа-башни, колонны |
| 6 | 🌲 Чародейский Лес | 4800 | Грибы, шипастые лозы, мшистые камни |
| 7 | 🌌 Мир Магии | 6000 | Порталы, призмы, кристаллы — максимальная сложность |

С каждым уровнем:
- Скорость увеличивается.
- Интервал между препятствиями сокращается.
- Шанс двойного спавна растёт.
- Меняется визуальный стиль: небо, земля, фоновые объекты, цвета препятствий.

### Визуальные и звуковые эффекты
- Динамическое небо с луной, звёздами, градиентами.
- Уникальные фоны для каждого уровня (пирамиды, замок, вулкан, храм, лес, порталы).
- Частицы: искры при заклинаниях, взрывы при уничтожении, звёзды при конфузии, лечебное сияние.
- Экранные эффекты: вспышки, тряска, замедление, откат времени.
- Вибрация (на мобильных устройствах).

### Технические особенности
- Canvas 2D, адаптивный под любые экраны.
- Голосовое управление через Web Speech API (русский язык).
- Распознавание как промежуточных, так и финальных результатов речи.
- Защита от повторного срабатывания (кулдаун 450 мс).
- Поддержка клавиатуры для тестирования (G, D, M, T, R, L, H).
- Сохранение истории для отката времени (12 секунд).

---

## 🇬🇧 English Description

### Overview
**Wizardrunner** is an endless runner with voice-controlled spells. You play as a wizard running through seven magical worlds, dodging obstacles, collecting coins, and casting spells by voice to survive and complete all levels.

### Controls
| Action | How to perform |
|---|---|
| Jump | Tap screen / Space / Arrow Up |
| Double jump | Double tap screen |
| Spells | Voice commands via microphone |

### Spells (voice commands)
| Phrase | Effect | Duration |
|---|---|---|
| **"Focus Pocus"** | Ghost form — invulnerability to all obstacles | 15 sec |
| **"Abracadabra"** | Destroys the nearest obstacle ahead | Instant |
| **"Magnifico"** | Attracts all coins within radius | 10 sec |
| **"Tempus"** | Rewinds time 7 seconds back (position, health, coins) | Instant |
| **"Tornado"** | Hurricane destroying up to 3 obstacles ahead | ~2.5 sec |
| **"Levitation"** | Flight above ground, invulnerability | 10 sec |
| **"Sanguis"** | Self-heal: +1 heart | Instant |

### Health & Damage
- The wizard has **5 hearts**.
- On collision with an obstacle (not invulnerable):
  - Loses 1 heart.
  - **Confusion** effect for 2 seconds — chaotic movement, cannot jump, controls impaired.
  - **Invulnerability for 2.5 seconds** (flashing).
- At 0 hearts — game over.

### Levels (7 Worlds)
| # | Name | Goal (meters) | Features |
|---|---|---|---|
| 1 | 🌙 Magic Night | 1500 | Night forest, rocks, spikes, crystals |
| 2 | 🏜 Sorcerers' Desert | 2100 | Cacti, sand towers, faster |
| 3 | 🏰 Academy of Magic | 2700 | Bookshelves, cauldrons, crystals |
| 4 | 🌋 Volcano of Warlocks | 3300 | Lava pools, magma boulders, spikes |
| 5 | 💀 Temple of Necromancers | 3900 | Bone altars, skull towers, pillars |
| 6 | 🌲 Enchanted Forest | 4800 | Mushrooms, thorn vines, mossy rocks |
| 7 | 🌌 World of Magic | 6000 | Portals, prisms, crystals — max difficulty |

With each level:
- Speed increases.
- Obstacle spawn interval decreases.
- Double spawn chance increases.
- Visual style changes: sky, ground, background objects, obstacle colors.

### Visual & Sound Effects
- Dynamic sky with moon, stars, gradients.
- Unique backdrops per level (pyramids, castle, volcano, temple, forest, portals).
- Particles: spell sparks, destruction explosions, confusion stars, healing glow.
- Screen effects: flashes, shake, slowdown, time rewind.
- Vibration (on mobile devices).

### Technical Features
- Canvas 2D, responsive to any screen.
- Voice control via Web Speech API (Russian language).
- Recognition of both interim and final speech results.
- Anti-repeat protection (450 ms cooldown).
- Keyboard support for testing (G, D, M, T, R, L, H).
- History saving for time rewind (12 seconds).

---
