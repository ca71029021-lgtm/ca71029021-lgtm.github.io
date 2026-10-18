# PROMPTS.md — библиотека команд проекта

## /ORIENT
- PURPOSE: быстро войти в контекст проекта.
- INSTRUCTIONS: прочитать AGENTS.md, GOALS.md, PLANS.md (статус фаз), docs/BRAND.md.
- OUTPUT: краткое резюме текущего состояния и следующего шага. STOP: резюме выдано.

## /PLAN
- PURPOSE: подготовить план следующей фазы.
- INPUT: номер фазы из PLANS.md.
- OUTPUT: OBJECTIVE/SCOPE/NON-GOALS/INPUTS/OUTPUTS/RISKS/ACCEPTANCE. STOP: план показан, ждёт APPROVAL.

## /DESIGN
- PURPOSE: предложить визуальное решение секции/экрана до внедрения в код.
- OUTPUT: мудборд словами (палитра, типографика, композиция) + wireframe текстом. STOP: согласование.

## /IMPLEMENT
- PURPOSE: внедрить согласованное изменение.
- INSTRUCTIONS: менять только согласованное; затем `npm run build` и проверка в браузере.
- OUTPUT: отчёт (FILES CHANGED / TESTS / ISSUES). STOP: отчёт выдан.

## /VISUAL-QA
- PURPOSE: независимая проверка визуала.
- INSTRUCTIONS: скриншоты ключевых экранов; проверить TYPOGRAPHY/COMPOSITION/SPACING/CONTRAST/RHYTHM/CTA.
- OUTPUT: список находок CRITICAL/HIGH/MEDIUM/LOW. STOP: список выдан.

## /UX-CRITIQUE
- PURPOSE: поиск friction в пути пользователя.
- OUTPUT: разбор по этапам DISCOVER→CONTACT, список проблем и быстрых побед.

## /CONVERSION-AUDIT
- PURPOSE: проверка CTA, формы, доверия.
- OUTPUT: рекомендации по приоритету, без выдуманных фактов.

## /MOBILE-AUDIT
- PURPOSE: проверка на 360–390 px: меню, карточки, форма, изображения.
- OUTPUT: список проблем + предложения. STOP: отчёт выдан.

## /CONTENT-AUDIT
- PURPOSE: проверка всех текстов на выдуманные факты.
- OUTPUT: список нарушений CONTENT-RULES + формулировки-замены с UNKNOWN.

## /PUBLISH
- PURPOSE: публикация на GitHub Pages.
- INSTRUCTIONS: пересобрать base64-чанки (≤750 КБ), версионировать URL (?v=N+1), обновить index/app/style с SHA, проверить raw → живой сайт, все 36 изображений грузятся.
- STOP: сайт обновлён и проверен; иначе честный статус «не завершено».

## /FINAL-AUDIT
- PURPOSE: прогон чек-листа GOALS.md + визуал + UX + мобильный + контент.
- OUTPUT: итоговый отчёт с зелёными/красными пунктами.

## /HANDOFF
- PURPOSE: передать проект: структура, как собирать/публиковать, что где лежит.
- OUTPUT: краткая инструкция + список открытых UNKNOWN.
