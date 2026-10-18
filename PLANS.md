# PLANS.md — Master Development Plan

## Статус фаз
- PHASE 0 — PROJECT ORIENTATION — ✅ DONE (2026-10-18)
- PHASE 1 — PRODUCT & CONTENT AUDIT — ✅ DONE (2026-10-18; docs/PRODUCT_AUDIT.md; commit «PHASE 1 — PRODUCT MASTER AUDIT FINALIZED»)
- PHASE 2 — COMPETITOR RESEARCH — ✅ DONE (2026-10-18; docs/COMPETITOR_RESEARCH.md + docs/COMPETITORS.md; commit «PHASE 2 — COMPETITOR RESEARCH COMPLETED»)
- PHASE 3 — BRAND STRATEGY — ✅ DONE (2026-10-18; docs/BRAND.md v2 + docs/AUDIENCE.md v2; commit «PHASE 3 — BRAND STRATEGY COMPLETED»)
- PHASE 4 — INFORMATION ARCHITECTURE — ⛔ GATE (следующая; ждёт подтверждения владельца)
- PHASE 5 — DESIGN DIRECTION — ⛔ GATE
- PHASE 6 — WIREFRAMES — (внутри PHASE 5/7)
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

## PHASE 4 — INFORMATION ARCHITECTURE (GATE)
- OBJECTIVE: решает: остаёмся one-page или переходим на многостраничный (каталог → карточка изделия).
- INPUTS: PHASE 2–3. OUTPUTS: схема страниц/якорей.

## PHASE 5 — DESIGN DIRECTION (GATE)
- OBJECTIVE: визуальное направление v2 (типографика, сетка, фотоподача).
- OUTPUTS: docs/DESIGN-SYSTEM.md v2, wireframes ключевых экранов.

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
| Цены/размеры: 33 из 36 VERIFIED (owner, «Каталог всех изделий.docx» 2026-10-18); UNKNOWN — 3 полки | частично закрыт (2026-10-18) |
| Две параллельные системы ID (старая/новая) без подтверждённой привязки | открыт |
| Фото изделий не отобраны вручную (главное фото = первое по алфавиту) | открыт |
| Публикация на служебном GitHub-аккаунте | открыт |
| Контакты: телефон UNKNOWN; e-mail altaywoodslab@gmail.com — NEEDS CONFIRMATION | открыт |
| Непроверенные цифры на сайте (450–500 лет, 3100 мм, 40–90 мм) — UNVERIFIED | открыт |
| Факты бренда UNKNOWN: история мастерской, имена мастеров, гарантия, статусы изделий | открыт (gaps G3–G6 в BRAND.md) |
