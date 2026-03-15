# AGENTS.md (пример для Node.js/TypeScript)

## Scope
Инструкции действуют для `frontend/`.

## Стек и стиль
- Node.js 20+
- Package manager: `pnpm`
- Линтинг: `pnpm lint`
- Тесты: `pnpm test`
- Typecheck: `pnpm typecheck`

## Ограничения
- Не использовать `any` без комментария, почему это необходимо.
- UI-изменения сопровождаются скриншотом.
- При правках UX обновлять `docs/changelog.md`.

## Команды перед коммитом
```bash
pnpm install --frozen-lockfile
pnpm lint
pnpm typecheck
pnpm test
pnpm build
```
