Откройте docs/workflow.md и внесите правила как часть артефактов сопровождения. Текст можно взять готовым и вставить без изменений:

Ветка main является основной. Прямые коммиты в main запрещены. Любое изменение выполняется в отдельной ветке и попадает в main через Pull Request.

Формат имени ветки: type/short-topic, где type принимает значения feature, fix, docs, chore, test. Примеры: docs/workflow-rules, feature/add-parser, fix/date-format.

Правило коммитов: один коммит фиксирует одну законченную мысль. Сообщение коммита задаётся в формате <type>: <действие>, где <type> принимает значения feat, fix, docs, chore, test, refactor. Примеры: docs: add workflow rules, feat: add app entrypoint, chore: add gitignore.

Правила Pull Request: в описании указываются цель изменения, что сделано и как проверить. Pull Request должен проходить локальные проверки ruff check . и запуск проекта. Если добавлены тесты, они должны запускаться командой pytest.