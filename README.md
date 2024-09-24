<h1 id="home">Homework :clipboard:</h1>

## react-hw-02-feedback

- 🇺🇸 [English](#en)
- 🇺🇦 [Ukrainian](#uk)
- 🇷🇺 [Russian](#ru)

---

<h3 id="en">📚 EN 📚</h3>

# Acceptance criteria

- Repository `react-hw-02-feedback` created
- When submitting homework, there are two links: to the source files and working

pages of each task on `GitHub Pages`.

- When running the task code, there are no errors or warnings in the console.
- Each component has a separate file in the `src/components` folder.
- `propTypes` are described for the components.
- Everything that the component expects as props is passed to it when called.
- JS code is clean and clear, `Prettier` is used.
- Styling is done by `CSS modules` or `Styled Components`.

# Feedback widget

Like most companies, Expresso Cafe collects feedback from its customers. Your
task is to create an application for collecting statistics. There are only three
options for feedback: good, neutral and bad.

## Step 1

The application should display the number of reviews collected for each
category. The application should not save review statistics between different
sessions (page refresh).

The application state must be of the following type, new properties cannot be
added.

```bash
state = {
good: 0,
neutral: 0,
bad: 0
}
```

The interface may look like this.

![preview](./hw/step-1.png)

## Step 2

Expand the functionality of the application so that the interface displays more
statistics about the collected reviews. Add a display of the total number of
reviews collected from all categories and the percentage of positive reviews. To
do this, create helper methods `countTotalFeedback()` and
`countPositiveFeedbackPercentage()`, which calculate these values ​​​​based on
the data in the state (calculated data).

![preview](./hw/step-2.png)

## Step 3

Refactor the application. The application state should remain in the root
component `<App>`.

- Move the statistics display to a separate component

`<Statistics good={} neutral={} bad={} total={} positivePercentage={}>`.

- Move the button block to the

`<FeedbackOptions options={} onLeaveFeedback={}>` component.

- Create a `<Section title="">` component that renders a section with a title
  and

children. Wrap each of `<Statistics>` and `<FeedbackOptions>` in

the created section component.

## Step 4

Extend the functionality of the application so that the statistics block is
rendered only after at least one review has been collected. Message about
absence of statistics move to the component
`<Notification message="There is no feedback">`.

![preview](./hw/preview.gif)

---

---

<h3 id="uk">📚 UK 📚 <a href="#home">⬆ Home ⬆</a></h3>

---

---

<h3 id="ru">📚 RU 📚 <a href="#home">⬆ Home ⬆</a></h3>

# Критерии приема

- Создан репозиторий `react-hw-02-feedback`
- При сдаче домашней работы есть две ссылки: на исходные файлы и рабочие
  страницы каждого задания на `GitHub Pages`.
- При запуске кода задания, в консоли нету ошибок и предупреждений.
- Для каждого компонента есть отдельный файл в папке `src/components`.
- Для компонентов описаны `propTypes`.
- Все что компонент ожидает в виде пропсов, передается ему при вызове.
- JS-код чистый и понятный, используется `Prettier`.
- Стилизация выполнена `CSS-модулями` или `Styled Components`.

# Виджет отзывов

Как и большинство компаний, кафе Expresso собирает отзывы от своих клиентов.
Твоя задача - создать приложение для сбора статистики. Есть всего три варианта
обратной связи: хорошо, нейтрально и плохо.

## Шаг 1

Приложение должно отображать количество собранных отзывов для каждой категории.
Приложение не должно сохранять статистику отзывов между разными сессиями
(обновление страницы).

Состояние приложения обязательно должно быть следующего вида, добавлять новые
свойства нельзя.

```bash
state = {
  good: 0,
  neutral: 0,
  bad: 0
}
```

Интерфейс может выглядеть так.

![preview](./hw/step-1.png)

## Шаг 2

Расширь функционал приложения так, чтобы в интерфейсе отображалось больше
статистики о собранных отзывах. Добавь отображение общего количества собранных
отзывов из всех категорий и процент положительных отзывов. Для этого создай
вспомогательные методы `countTotalFeedback()` и
`countPositiveFeedbackPercentage()`, подсчитывающие эти значения основываясь на
данных в состоянии (вычисляемые данные).

![preview](./hw/step-2.png)

## Шаг 3

Выполни рефакторинг приложения. Состояние приложения должно оставаться в
корневом компоненте `<App>`.

- Вынеси отображение статистики в отдельный компонент
  `<Statistics good={} neutral={} bad={} total={} positivePercentage={}>`.
- Вынеси блок кнопок в компонент
  `<FeedbackOptions options={} onLeaveFeedback={}>`.
- Создай компонент `<Section title="">`, который рендерит секцию с заголовком и
  детей (children). Оберни каждый из `<Statistics>` и `<FeedbackOptions>` в
  созданный компонент секции.

## Шаг 4

Расширь функционал приложения так, чтобы блок статистики рендерился только после
того, как был собран хотя бы один отзыв. Сообщение об отсутствиии статистики
вынеси в компонент `<Notification message="There is no feedback">`.

![preview](./hw/preview.gif)
