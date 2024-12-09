# React Add TODO Form

Implemented the ability to add TODOs to the `TodoList` implemented in the **Static List of TODOs**

1. Created an `App` component storing the `todos` array and displaying it using the `TodoList`.
1. Created a form to add new TODOs:
    - there should be a text input for the `title` with `data-cy="titleInput"` attribute;
    - add a `<select>` with `data-cy="userSelect"` attribute showing all the given users;
    - add labels and placeholders where they are needed;
    - add a new todo to the list after clicking the `Add` button;
    - each TODO should have `id`, `title`, `userId`, and `completed` (`false` by default);
    - `id` is the largest `id` in the array + 1 (add `data-id={todo.id}` attribute to each `.TodoInfo`).
1. Added validation to the form:
    - add a default empty option `Choose a user` to the select;
    - before creating a todo, check if a `user` was selected; if not, show an error message next to the `select` (`Please choose a user`);
    - if the `title` is empty, show an error message next to the `title` field (`Please enter a title`);
    - errors should appear only after clicking the `Add` button;
    - hide the message immediately after any change of the field with an error;
1. If the form is valid, add a todo to the list and clear the form.
1. Allow entering only letters (`ua` and `en`), digits, and `spaces` in the `title` field. Just remove any other characters from the `title`.

## Demo Links

- [DEMO LINK](https://AndriiZakharenko.github.io/react_add-todo-form/)
