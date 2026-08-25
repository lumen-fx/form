# form

A two-way bound form: every control mirrors into a signal, and the
status line re-derives from the signals on each edit.

Concepts demonstrated:

- **Two-way bindings** - `bind-text` (input), `bind-checked` (toggle),
  `bind-value` (slider). User edits write back into the signals.
- **Lifecycle callbacks** - `on_text_input(id, text)`, `on_toggle(id, on)`,
  `on_slider(id, value)` fire on every control change.
- **Signal handles** - `signal("dark")` names a cell; `get` reads its string
  form and `get_bool` / `get_int` / `get_float` read it typed.
- **Focus styling** - `tab-index` puts controls in the Tab chain;
  `:focus { outline: ... }` shows the ring.

Run it:

```sh
lumenc run .
```
