# Product Requirements Document (PRD) - Todo App Upgrade

## 1. Overview

Upgrade the basic Todo app, which currently supports a task title and completed state, so users can organize tasks using due dates, priorities, and quick filters. The MVP must remain simple and teachable, use local storage, and require no backend changes.

---

## 2. MVP Scope

- Add an optional `dueDate` field to each task.
  - Use the ISO `YYYY-MM-DD` format.
  - Ignore invalid values and treat them as absent.
- Add a required `priority` field to each task.
  - Allow `P1`, `P2`, or `P3`.
  - Default to `P3`.
  - Display priorities as color-coded badges: red for `P1`, orange for `P2`, and gray for `P3`.
- Keep `title` required.
- Provide three filter tabs: **All**, **Today**, and **Overdue**.
  - **All** includes completed and incomplete tasks.
  - **Today** and **Overdue** show only incomplete tasks.
- Keep task storage local, with no backend changes or external storage.

---

## 3. Post-MVP Scope

- Visually highlight overdue tasks in red.
- Sort tasks in this order:
  1. Overdue tasks first.
  2. Priority from `P1` to `P3`.
  3. Due date in ascending order.
  4. Tasks without a due date last.

---

## 4. Out of Scope

- Notifications.
- Recurring tasks.
- Multi-user support.
- Keyboard navigation or special accessibility features.
- Backend changes.
- External storage.