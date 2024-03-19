<h1 align="center">Проектный практикум</h1>

## Содержание

<details>
<summary>Открыть содержание</summary>

-   [Матрица ответственности](#Матрица-ответственности)
-   [Examples](#examples)
-   [Release](#release)
-   [Related projects](#related-projects)
-   [Contributors](#contributors---)
-   [Security and safe diagrams](#security-and-safe-diagrams)
-   [Reporting vulnerabilities](#reporting-vulnerabilities)
-   [Appreciation](#appreciation)

</details>

## Матрица заинтересованных лиц

![matrix of interest](./matrix.jpg)

<table>
    <tr>
        <th>Результаты проекта</th>
        <th>Роль в проекте / должность</th>
    </tr>
    <tr>
    </tr>
</table>

<p align="right">
<a href="./ResponsibilityMatrix.md">more</a>
</p>

|               | 1   | 2   | 3   | 4   |
| ------------- | --- | --- | --- | --- |
| Documentation | 25  | 10  | 5   | 25  |
| Programming   | 0   | 15  | 20  | 0   |

Pandoc

**ERP Студента**

```mermaid
flowchart TD
    A{{Вход/Регистрация}} --> B{{Выбор науч.рука}}
    B --> C{Подтверждение\n науч.рука}
    C -->|Yes| D{{Выбор темы}}
    C -->|No| B
    D --> E{Утверждение\n темы}
    E -->|Yes| status
    E -->|No| D
    subgraph status
        direction TB
        a[Выбор темы] --> b[Изучение теоретических аспектов темы]
        b --> c[Сбор и анализ данных]
        c --> d[Написание основной части / Разработка]
        d --> e[Оформление ВКР]
        e --> f[Завершено]
    end
```

**ERP Преподавателя**

```mermaid
flowchart TD
    A{{Вход/Регистрация}} --> B{{Подтверждение\n студентов}}
    B --> C{{Подтверждение тем}}
    C -->D{{Выбор темы}}
    D --> E(Наблюдение за\n продвижением студентов)
    E --> status
    subgraph status
        direction TB
        a[Выбор темы] --> b[Изучение теоретических аспектов темы]
        b --> c[Сбор и анализ данных]
        c --> d[Написание основной части / Разработка]
        d --> e[Оформление ВКР]
        e --> f[Завершено]
    end
```

![](tfwzqvpD6W16jVC_ezWZQsK3baTgH5gZbeDE3_n1QLDbCQ92tmdm7SL0_7cyHBjsHcXsZYx3WoTY1MgMzxBryDZhdraBXPbhYsX3k6bf37T82Gdy0QSAmmBQVWAjZMzEvOLBUfvz)
