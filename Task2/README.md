# Task 2. Архитектурное видение и выбор архитектурного стиля

**Решение:** модульный монолит на Go, платежи и логистика через партнёров, один управляемый PostgreSQL, контейнеры в Kubernetes. Переход к сервисам — по триггерам, вариант CTO отклонён по цифрам (ADR-001).

| Файл | Что внутри |
| --- | --- |
| [options-comparison.md](options-comparison.md) | Сравнение трёх вариантов (монолит / сервисы / вариант CTO) по срокам, деньгам, команде и TCO; проверка ставки \$12 000 за минуту простоя |
| [tco-model.xlsx](tco-model.xlsx) | Модель TCO на 5 лет: лист «Сравнение» + по листу на вариант |
| [adr-001-architecture-style.md](adr-001-architecture-style.md) | ADR №1: выбор стиля, отклонённые альтернативы, триггеры пересмотра |
| [architecture-vision.md](architecture-vision.md) | Architecture Vision: цели, принципы, целевое решение, интересы стейкхолдеров, дорожная карта |
| [c4-context.puml](c4-context.puml) · [.png](c4-context.png) | C4 Context: роли и 7 внешних систем с подписями связей |
| [use-cases.puml](use-cases.puml) · [.png](use-cases.png) | Use Case: 16 сценариев MVP |
| [nairobi-slide.pptx](nairobi-slide.pptx) | Один слайд для встречи в Найроби |
| [nairobi-script.md](nairobi-script.md) | Транскрипт выступления, 10 минут |
| `monolith.png`, `microservices.png`, `arch_draft.excalidraw` | Рабочие черновики вариантов A и B (не сдаточные артефакты) |

**Ключевые цифры:** TCO 5 лет (архитектурная часть) — \$6,70 / \$8,13 / \$13,89 млн; стоимость заказа — \$1,25 / \$1,29 / \$1,44; облако и SaaS в Год 1 — 51% / 83% / 154% лимита CFO; цена ошибки — \$1,0 млн против \$120 тыс. (8,4 : 1).

**Шаблон ADR:** [../templates/adr-template.md](../templates/adr-template.md), нумерация сквозная через Task2–Task5.
