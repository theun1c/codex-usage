# Примеры подключения MCP-серверов

> Ниже — концептуальные примеры. Точные поля зависят от реализации клиента.

## 1) Локальный filesystem MCP
```toml
[mcp.servers.filesystem]
command = "npx"
args = ["-y", "@modelcontextprotocol/server-filesystem", "/workspace"]
```

## 2) GitHub MCP
```toml
[mcp.servers.github]
command = "npx"
args = ["-y", "@modelcontextprotocol/server-github"]

[mcp.servers.github.env]
GITHUB_TOKEN = "${GITHUB_TOKEN}"
```

## 3) Postgres MCP (read-only)
```toml
[mcp.servers.postgres]
command = "npx"
args = ["-y", "@modelcontextprotocol/server-postgres", "${DATABASE_URL}"]

[mcp.servers.postgres.policies]
mode = "read-only"
```

## Минимальный процесс валидации
1. Поднять MCP-сервер.
2. Проверить, что агент видит ресурсы (`list_mcp_resources`).
3. Прочитать тестовый ресурс.
4. Проверить логи на ошибки авторизации/прав.

## Рекомендации по безопасности
- Выдавайте токены с минимально необходимыми scope.
- Для БД используйте read-only роли по умолчанию.
- Логируйте действия с чувствительными источниками.
- Явно документируйте, кто владелец секрета и срок ротации.
