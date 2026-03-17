# AI Development Workflow (Personal)

## Общая философия

Современная разработка с AI делится на два основных этапа:

```
Planning → Implementation
```

* **Planning** — требования, архитектура, декомпозиция задач
* **Implementation** — написание кода, тесты, исправление ошибок

AI используется как **ассистент и junior-разработчик**, а человек выступает как:

* архитектор
* ревьюер
* интегратор
* декомпозитор задач

---

# Основные инструменты

## 1. Kiro — Planning / Specification

**Назначение**

Используется для:

* генерации требований
* архитектуры
* декомпозиции задач
* проектной документации

**Типичный workflow**

```
Idea
↓
requirements.md
↓
design.md
↓
tasks.md
```

**Когда использовать**

* новый проект
* сложная архитектура
* микросервисы
* backend системы
* SaaS проекты

**Что генерирует**

```
/spec
   requirements.md
   design.md
   tasks.md
```

---

## 2. Windsurf — основная IDE

**Назначение**

IDE для работы с кодом и интеграции AI.

Используется для:

* редактирования кода
* просмотра diff
* навигации по репозиторию
* интеграции AI-агентов

**Почему используется**

* удобная работа с большими codebase
* хороший AI-контекст проекта
* подходит для AI pair programming

---

## 3. Codex — AI coding agent

**Назначение**

Основной AI для:

* написания кода
* refactor
* генерации тестов
* объяснения кода
* code review

**Роли Codex**

```
junior developer
code generator
review assistant
mentor
```

**Примеры использования**

```
Implement task 1 from tasks.md
Explain this code
Refactor this module
Generate tests for this file
```

---

# Персональный workflow

## Planning этап

Используется **Kiro**

```
idea
↓
requirements
↓
architecture
↓
tasks
```

Результат:

```
requirements.md
design.md
tasks.md
```

---

## Implementation этап

Используется **Windsurf + Codex**

```
open repo
↓
read spec
↓
implement feature
↓
fix bugs
↓
next feature
```

---

# Основной стиль разработки

Используется комбинация двух подходов:

## 1. Feature-driven development

```
feature
↓
implement
↓
fix
↓
next feature
```

---

## 2. AI pair programming

```
developer writes code
↓
Codex reviews
```

или

```
Codex writes code
↓
developer reviews
```

---

# Правило работы с AI

**Никогда не использовать код, который не понимаешь.**

Перед использованием:

* прочитать код
* понять архитектуру
* проверить логику
* при необходимости попросить объяснение

---

# Полезные запросы для Codex

### Понимание кода

```
Explain this code step by step
Why did you choose this pattern?
```

### Улучшение кода

```
Refactor this code
Optimize this function
Improve readability
```

### Архитектура

```
Suggest better architecture for this module
```

### Тесты

```
Generate tests for this module
```

---

# Цель использования AI

AI используется для удаления рутины:

* boilerplate код
* документация
* генерация тестов
* поиск ошибок

Человек отвечает за:

```
architecture
system design
problem solving
integration
code review
```

---

# Итоговый стек

```
Planning
   Kiro

IDE
   Windsurf

AI
   Codex
```

Workflow:

```
Kiro → specification
↓
Windsurf → development
↓
Codex → coding + mentoring
```

---

# Главная идея

AI — это не замена разработчика.

Это **ускоритель разработки**.

Разработчик остаётся ответственным за:

* архитектуру
* качество кода
* системное мышление
* интеграцию компонентов

```
```
