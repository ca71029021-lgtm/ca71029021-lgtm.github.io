# PLANS.md — Master Development Plan

## Статус фаз
- PHASE 0 — PROJECT ORIENTATION — ✅ DONE (2026-10-18)
- PHASE 1 — PRODUCT & CONTENT AUDIT — ✅ DONE (2026-10-18; docs/PRODUCT_AUDIT.md; commit «PHASE 1 — PRODUCT MASTER AUDIT FINALIZED»)
- PHASE 2 — COMPETITOR RESEARCH — ✅ DONE (2026-10-18; docs/COMPETITOR_RESEARCH.md + docs/COMPETITORS.md; commit «PHASE 2 — COMPETITOR RESEARCH COMPLETED»)
- PHASE 3 — BRAND STRATEGY — ✅ DONE (2026-10-18; docs/BRAND.md v2 + docs/AUDIENCE.md v2; commit «PHASE 3 — BRAND STRATEGY COMPLETED»)
- PHASE 4 — INFORMATION ARCHITECTURE — ✅ DONE (2026-10-18; docs/INFORMATION_ARCHITECTURE.md + docs/UX.md; commit «PHASE 4 — INFORMATION ARCHITECTURE COMPLETED»)
- PHASE 5 — DESIGN DIRECTION — ✅ APPROVED (2026-10-18; направление A + эмоциональный слой B; commit «PHASE 5 — DESIGN DIRECTION APPROVED»)
- PHASE 6 — WIREFRAMES + VISUAL PROTOTYPE + PHOTO AUDIT — ✅ APPROVED (2026-10-19; docs/PHASE_6_WIREFRAMES.md + docs/PHASE_6_VISUAL_PROTOTYPE_REVIEW.md + docs/PHOTO_AUDIT.md + docs/PHASE_6_APPROVAL.md; commits «PHASE 6 — WIREFRAMES COMPLETED», «PHASE 6 — VISUAL PROTOTYPE REVIEW COMPLETED», «PHOTO AUDIT — COMPLETED», «PHASE 6 — VISUAL PROTOTYPE AND PHOTO AUDIT APPROVED», «PROJECT CONTACTS AND INQUIRY RULES — APPROVED»)
- PHASE 7 — PROTOTYPE — ▶ APPROVED FOR START (2026-10-19; initial version; форма prototype-only; после первой версии — остановка на утверждение; commit «PROJECT CONTACTS AND INQUIRY RULES — APPROVED»)
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

## PHASE 6 — PHOTO AUDIT (контрольный подэтап) — ✅ DONE 2026-10-19
- OBJECTIVE: проанализировать реальную фототеку (33 папки изделий, 333 изображения) и выбрать рекомендованные фото по назначениям ДО PHASE 7. Только анализ; фото не изменялись/не удалялись/не переименовывались; AI-генерация не использовалась.
- ФАКТ: docs/PHOTO_AUDIT.md. Главные фото рекомендованы для 32 из 33 изделий; SNS028 — критический разрыв (нет студийного кадра, только уличные фото на газоне и листы каталога со встроенным баннером). Выбраны: 5 кандидатов HERO, рабочий набор Selected, Featured, макро Материала, тайлы категорий. Полностью отсутствуют: фото процесса/мастерской, интерьерные кадры, портрет мастера (TO PRODUCE). HTML/CSS/JS, фото и Product Master не тронуты.

## PHASE 6 — APPROVAL (итоговое утверждение фазы) — ✅ APPROVED 2026-10-19
- OBJECTIVE: зафиксировать все решения владельца перед PHASE 7 в одном документе.
- ФАКТ: docs/PHASE_6_APPROVAL.md. Принято: HERO B — основной hero, HERO A — атмосферный блок; HERO PHOTO = SNS033/_156.jpg (PROVISIONAL / APPROVED FOR PROTOTYPE, замена допускается без изменения архитектуры сайта); SELECTED PRODUCTS = S002/SN008/SNS033 (PROVISIONAL / APPROVED FOR PROTOTYPE); SNS028 — сохранён в каталоге, исключён из HERO/Featured/editorial/первого экрана (PHOTO GAP / NEEDS RESHOOT, не удалять); PHOTO TO PRODUCE не блокирует PHASE 7 (placeholder ≠ реальное фото); Photography Rule — только реальные фото, AI-generated запрещены; Google Drive не блокирует проект. HTML/CSS/JS, фото и Product Master не тронуты.

## PHASE 6 — OPEN QUESTIONS RESOLVED (контрольный подэтап) — ✅ DONE 2026-10-19
- OBJECTIVE: закрыть открытые вопросы проекта перед стартом PHASE 7.
- ФАКТ: решения владельца зафиксированы в docs/PHASE_6_APPROVAL.md §14 и docs/CONTENT-RULES.md (новый файл), обновлены docs/UX.md. Итоги: (1) приём заявок — основной: форма на сайте; доп.: e-mail; messenger — NEEDS CONFIRMATION (не фиксировать канал); форма минимальная: имя/телефон/e-mail/изделие/сообщение. (2) «Единственный экземпляр» — не под изделиями и не badge; один отдельный смысловой раздел. (3) Контакты: e-mail ЗАМЕНЁН на Siberian.slab@gmail.com (во всех новых элементах; старый — только исторический); телефон — PHONE NEEDS CONFIRMATION (подтверждённый номер в материалах проекта не найден, не выдумывать). (4) Текущие фото временные, замена на студийные позже (этап PHOTO REPLACEMENT / PHOTO FINALIZATION); не удалять/не редактировать/не генерировать. (5) Путь HOME→CATALOG→PRODUCT→INQUIRY (+ HOME→CONTACT); CTA: hero «Смотреть коллекцию», каталог «Смотреть изделие», PDP «Оставить заявку на это изделие»; e-mail в Footer и Contact. (6) Запрет придумывать коммерческие/юридические утверждения. (7) PHASE 7 разрешён: initial version, форма prototype-only, после первой версии — остановка на утверждение.

## PHASE 7 — PROTOTYPE (GATE) — ▶ APPROVED FOR START 2026-10-19
- OBJECTIVE: кликабельный прототип новой IA/дизайна (до внедрения в код).
- УСЛОВИЯ СТАРТА (владелец): новый e-mail; телефон не публиковать выдуманный (NEEDS CONFIRMATION); форма заявки prototype-only; messenger — NEEDS CONFIRMATION; «единственный экземпляр» — отдельный раздел, не под изделиями; текущие фото временные с предусмотренной заменой.
- СТОП-ПРАВИЛО: после завершения первой версии — остановка и представление результата владельцем; автоматический переход к production development запрещён.

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
| Фото изделий не отобраны вручную (главное фото = первое по алфавиту) | закрыт как риск (2026-10-19): рекомендованные главные фото — docs/PHOTO_AUDIT.md §3; финальное утверждение — за владельцем |
| SNS028: нет пригодных фото | решение принято (2026-10-19): сохранён в каталоге, исключён из HERO/Featured/editorial/первого экрана; NEEDS RESHOOT; изделие и фото не удалять (PHASE_6_APPROVAL.md §8) |
| Публикация на служебном GitHub-аккаунте | открыт |
| Контакты | частично закрыт (2026-10-19): e-mail VERIFIED = Siberian.slab@gmail.com (заменил прежний; прежний — только исторический); телефон — PHONE NEEDS CONFIRMATION (подтверждённый номер в материалах проекта не найден; не выдумывать); messenger — NEEDS CONFIRMATION |
| Непроверенные цифры на сайте (450–500 лет, 3100 мм, 40–90 мм) — UNVERIFIED | открыт |
| Факты бренда UNKNOWN: история мастерской, имена мастеров, гарантия, статусы изделий | открыт (gaps G3–G6 в BRAND.md) |
| Нет фото процесса/мастерской, интерьерных кадров, портрета мастера (блоки Craftsmanship/История/Доверие) | открыт — TO PRODUCE; PHASE 7 НЕ блокирует (PHOTO_AUDIT.md §5, PHASE_6_APPROVAL.md §9) |