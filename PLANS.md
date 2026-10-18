# PLANS.md — Master Development Plan

## Статус фаз
- PHASE 0 — PROJECT ORIENTATION — ✅ DONE (2026-10-18)
- PHASE 1 — PRODUCT & CONTENT AUDIT — ✅ DONE (2026-10-18; docs/PRODUCT_AUDIT.md; commit «PHASE 1 — PRODUCT MASTER AUDIT FINALIZED»)
- PHASE 2 — COMPETITOR RESEARCH — ✅ DONE (2026-10-18; docs/COMPETITOR_RESEARCH.md + docs/COMPETITORS.md; commit «PHASE 2 — COMPETITOR RESEARCH COMPLETED»)
- PHASE 3 — BRAND STRATEGY — ✅ DONE (2026-10-18; docs/BRAND.md v2 + docs/AUDIENCE.md v2; commit «PHASE 3 — BRAND STRATEGY COMPLETED»)
- PHASE 4 — INFORMATION ARCHITECTURE — ✅ DONE (2026-10-18; docs/INFORMATION_ARCHITECTURE.md + docs/UX.md; commit «PHASE 4 — INFORMATION ARCHITECTURE COMPLETED»)
- PHASE 5 — DESIGN DIRECTION — ✅ APPROVED (2026-10-18; направление A + эмоциональный слой B; commit «PHASE 5 — DESIGN DIRECTION APPROVED»)
- PHASE 6 — WIREFRAMES — ✅ DONE (2026-10-18; docs/PHASE_6_WIREFRAMES.md + docs/PHASE_6_VISUAL_PROTOTYPE_REVIEW.md; commits «PHASE 6 — WIREFRAMES COMPLETED», «PHASE 6 — VISUAL PROTOTYPE REVIEW COMPLETED»)
- PHASE 7 — PROTOTYPE — ⛔ GATE
- PHASE 8 — FRONTEND IMPLEMENTATION — ⛔ GATE
- PHASE 9 — CONTENT INTEGRATION — ⛔ GATE
- PHASE 10 — QA — (внутри каждой фазы)
- PHASE 11 — UX / CONVERSION AUDIT — ⛔ GATE
- PHASE 12 — FINAL REVIEW — ⛔ GATE

---

## PHASE 1 — PRODUCT & CONTENT AUDIT
- OBJECTIVE: зафиксировать документацию и подтверждённую базу 36 изделий.
- SCOPE: AGENTS/GOALS/PLANS/PROMPTS.md, docs/*.md, PRODUCT-база.
- NON-GOALS: изменение дизайна/кода сайта.
- INPUTS: структура `ВСЕ ИЗДЕЛИЯ/`, фото, ранее собранный лендинг.
- OUTPUTS: файлы документации; реестр UNKNOWN.
- ACCEPTANCE: документы созданы, изделия занесены со статусами.

## PHASE 2 — COMPETITOR RESEARCH (GATE) — ✅ DONE 2026-10-18
- OBJECTIVE: 5–8 референсов premium handcrafted furniture; извлечь transferable patterns.
- ФАКТ: исследовано 13 сайтов (IT/DK/UK/US/JP/FR). OUTPUTS: docs/COMPETITOR_RESEARCH.md (полный анализ), docs/COMPETITORS.md (сводка). NON-GOALS: копирование — соблюдено.

## PHASE 3 — BRAND STRATEGY (GATE) — ✅ DONE 2026-10-18
- OBJECTIVE: позиционирование, essence, аудитория, journey, дифференциация, коммуникация.
- ФАКТ: docs/BRAND.md v2 (позиционирование «материал первичен», ToV, brand story без выдумок, 8 gaps G1–G8, вопросы Q1–Q4), docs/AUDIENCE.md v2 (5 сегментов, приоритет 1–2). Открытые решения владельца: CTA, гарантия, публикация цен, месседж «единственный экземпляр».

## PHASE 4 — INFORMATION ARCHITECTURE (GATE) — ✅ DONE 2026-10-18
- OBJECTIVE: решает: остаёмся one-page или переходим на многостраничный (каталог → карточка изделия).
- ФАКТ: одобрена гибридная многостраничная архитектура. OUTPUTS: docs/INFORMATION_ARCHITECTURE.md (sitemap, 2 сценария A/B + прямой вход, структура карточки, mobile IA, URL-структура, CTA-логика, спорные решения S1–S7), docs/UX.md. Каталог: 3 категории / 33 изделия (полки исключены решением владельца).

## PHASE 5 — DESIGN DIRECTION (GATE) — ✅ APPROVED 2026-10-18
- OBJECTIVE: визуальное направление v2 (типографика, сетка, фотоподача).
- ФАКТ: разработаны 3 Art Direction (A — Editorial/Architectural, B — Natural/Tactile, C — Contemporary Luxury), сравнительная таблица 13 критериев. OUTPUTS: docs/DESIGN_DIRECTION.md (hero-концепции, типографика, палитра HEX, сетка, photography direction, карточка/PDP, навигация, CTA, motion, mobile, a11y, premium-аудит, дифференциация), docs/DESIGN-SYSTEM.md (токены + компоненты). HTML/CSS/JS и фото не тронуты.
- УТВЕРЖДЕНИЕ: направление A — основа визуальной системы + эмоционально-тактильный слой B; C не используется. Кедр — визуальный герой. Типографика (Cormorant Garamond + Inter), цвета, grid, photography direction, motion — утверждены как проектная база с допуском уточнения. Открытыми остаются: публикация цен (S2), состав «избранных» (S7), формулировки CTA (Q1).

## PHASE 6 — WIREFRAMES (GATE) — ✅ DONE 2026-10-18
- OBJECTIVE: структура всех ключевых экранов до вёрстки: главная, hero ×2, каталог → категория → карточка, PDP, mobile, CTA-flow, фото-система, interaction, QC.
- ФАКТ: docs/PHASE_6_WIREFRAMES.md. Порядок блоков главной уточнён (HERO → Материал → Craftsmanship → Избранные → Категории → Featured → Trust → CTA → Footer); два варианта hero (рекомендация B, A — под A/B-тест); карточка IMAGE→NAME→ID→SIZE→PRICE→CTA; PDP 10 обязательных блоков; mobile-first 9 элементов; фото-система TO SELECT/TO PRODUCE; interaction 10 эффектов; QC 8 критериев (2 предупреждения). Спорные: W1–W5. Требуют решения владельца: hero-вариант, избранные/featured (S7), публикация цен (S2), формулировки CTA (Q1), способ приёма заявок. HTML/CSS/JS, фото и Product Master не тронуты.

## PHASE 6 — VISUAL PROTOTYPE REVIEW (контрольный подэтап) — ✅ DONE 2026-10-18
- OBJECTIVE: показать визуально, как утверждённая IA + Design Direction выглядят ДО production. PROTOTYPE — NOT PRODUCTION.
- ФАКТ: docs/PHASE_6_VISUAL_PROTOTYPE_REVIEW.md. Собрано 8 экранов на реальных фото: Home Desktop/Mobile, Catalog, Category (кухонные), PDP Desktop/Mobile (SN008), Hero A и Hero B. Только реальные фото проекта + утверждённый hero-ассет; недостающие кадры помечены PHOTO TO SELECT. Сравнение HERO A vs B (8 критериев, 1–10): A = 7.25, B = 8.25; рекомендация B (без выбора за владельца). Final review: 8/8 критериев. HTML/CSS/JS, фото и Product Master не тронуты; мокапы — локальные артефакты workspace (в репозиторий бинарники не передаются).

## PHASE 7 — PROTOTYPE (GATE)
- OBJECTIVE: кликабельный прототип новой IA/дизайна (до внедрения в код).

## PHASE 8 — FRONTEND IMPLEMENTATION (GATE)
- OBJECTIVE: внедрение поэтапно (по секциям), без переписывания всего сразу.

## PHASE 9 — CONTENT INTEGRATION (GATE)
- OBJECTIVE: реальные цены/размеры/фото по мере получения от пользователя.

## PHASE 11 — UX / CONVERSION AUDIT (GATE)
- OBJECTIVE: критический разбор: friction, CTA, мобильный опыт; список улучшений по приоритету.

## PHASE 12 — FINAL REVIEW (GATE)
- OBJECTIVE: полный аудит перед «сдачей»; чек-лист GOALS.md.

---

## Реестр рисков (поддерживаемый)
| Риск | Статус |
|---|---|
| Цены/размеры: 33 публикуемых изделия VERIFIED (owner, «Каталог всех изделий.docx» 2026-10-18); полки исключены из публикации; высота не используется | закрыт (2026-10-18) |
| Две параллельные системы ID (старая/новая) без подтверждённой привязки | открыт |
| Фото изделий не отобраны вручную (главное фото = первое по алфавиту) | открыт |
| Публикация на служебном GitHub-аккаунте | открыт |
| Контакты: телефон UNKNOWN; e-mail altaywoodslab@gmail.com — NEEDS CONFIRMATION | открыт |
| Непроверенные цифры на сайте (450–500 лет, 3100 мм, 40–90 мм) — UNVERIFIED | открыт |
| Факты бренда UNKNOWN: история мастерской, имена мастеров, гарантия, статусы изделий | открыт (gaps G3–G6 в BRAND.md) |