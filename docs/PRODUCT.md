# PRODUCT.md — база продукции Siberian Nature Style

## Формат записи
PRODUCT ID · NAME · CATEGORY · PHOTOS (штук в папке) · DIMENSIONS · PRICE · STATUS
Статусы: VERIFIED / NEEDS CONFIRMATION / UNKNOWN.

## Общие факты (VERIFIED)
- Материал: алтайский кедр, цельные слэбы, живой край; часть изделий — с эпоксидной заливкой.
- Все изделия уникальны (единичный экземпляр).
- Фото на сайте: по 1 (первое по алфавиту) — требуется ручной отбор главного фото.

## Журнальные столы — 7 (VERIFIED)
| ID | Фото | Размеры | Цена | Статус |
|---|---|---|---|---|
| S001 | 17 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION (главное фото) |
| S002 | 17 | UNKNOWN | ~10 000 ₽ (старая карточка «S 2») | NEEDS CONFIRMATION |
| S003 | 14 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| S004 | 12 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| S005 | 14 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| S006 | 15 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| S007 | 8 | UNKNOWN | ~25 000 ₽ (старая карточка «S 7») | NEEDS CONFIRMATION |

## Кухонные столы — 19 (VERIFIED)
| ID | Фото | Размеры | Цена | Статус |
|---|---|---|---|---|
| SN008 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN009 | 13 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN010 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN011 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN012 | 21 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN013 | 9 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN014 | 9 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN015 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN016 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN017 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN018 | 12 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN019 | 13 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN020 | 12 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN021 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN022 | 12 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN023 | 13 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN024 | 14 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN025 | 15 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SN026 | 14 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |

## Эксклюзивные столы — 7 (VERIFIED)
| ID | Фото | Размеры | Цена | Статус |
|---|---|---|---|---|
| SNS027 | 19 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS028 | 8 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS029 | 22 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS030 | 20 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS031 | 12 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS032 | 16 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| SNS033 | 28 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |

## Полки — 3 (VERIFIED)
| ID | Фото | Размеры | Цена | Статус |
|---|---|---|---|---|
| Полка 1 500 | 3 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| Полка 1600 | 4 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |
| Полка 1700 | 6 | UNKNOWN | UNKNOWN | NEEDS CONFIRMATION |

## Старые данные (из первой версии лендинга) — NEEDS CONFIRMATION к сопоставлению
- «Эксклюзивный №69 (SNS 5)» 1980×1050×72 — 230 000 ₽
- «Эксклюзивный №70 (SNS 4)» 3000×(860–930)×75 — 220 000 ₽
- «Эксклюзивный SNS 1» 2020×(850–940)×76 — 140 000 ₽
- «Письменный SN 5» 1600×(820–880)×82 — 43 000 ₽
- Диапазоны: журнальные от 8 000 ₽, письменные от 28 000 ₽, эксклюзивные от 140 000 ₽.
⚠️ Старые фото (sns1/sns4/sns5, sn5) не сопоставлены с новыми ID — объединять автоматически запрещено.

## Реестр UNKNOWN (запросить у пользователя)
1. Размеры всех 36 изделий.
2. Цены всех изделий + диапазоны по категориям.
3. Главное фото для каждого изделия (сейчас — первое по алфавиту).
4. Статус каждого изделия: в наличии / под заказ / продано.

## Content pipeline
SOURCE (папки ВСЕ ИЗДЕЛИЯ) → фото на сайт (1200 px JPG) → PRODUCT.md (база) → Collection (каталог) → далее: карточки изделий, КП, маркетинг.

## UPDATE 2026-10-18 — «Каталог всех изделий.docx» (owner-provided, VERIFIED)
Текущий каталог владельца, привязанный к новым ID. Полная таблица (33/36) — в docs/PRODUCT_AUDIT.md,
раздел «UPDATE 2026-10-18». Кратко:
- Журнальные: 8 500–15 000 ₽ (S001 9 500; «S022»⚠️ 11 000 — вероятно S002; S003 8 500; S004 9 500; S005 11 000; S006 9 000; S007 15 000), размеры 650–800 × 450–500, толщ. 48.
- Кухонные: 28 000–120 000 ₽ (SN008–SN026; SN011 без высоты), размеры 1020–3000 мм.
- Эксклюзивные: 65 000–190 000 ₽ (SNS027–SNS033), размеры 1440–3000 мм.
- Полки: в файле отсутствуют — цены UNKNOWN.
- Статусы (в наличии/под заказ/продано): UNKNOWN для всех 36.
- Конфликты со старыми каталогами сохранены; для публикации приоритет — данные владельца.
