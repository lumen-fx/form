# form

A two-way bound form: every control mirrors into a signal, and the
status line re-derives from the signals on each edit.

Concepts demonstrated:

- **Two-way bindings** - `bind-text` (input), `bind-checked` (toggle),
  `bind-value` (slider). User edits write back into the signals.
- **Lifecycle callbacks** - `on_text_input(id, text)`, `on_toggle(id, on)`,
  `on_slider(id, value)` fire on every control change.
- **Signal handles** - `signal<bool>("dark")` names a cell and says what it
  holds; one `get` / `set` pair reads and writes it as that type, and
  `signal<int>` / `signal<float>` / `signal<string>` do the same for theirs.
- **Focus styling** - `tab-index` puts controls in the Tab chain;
  `:focus { outline: ... }` shows the ring.

Run it:

```sh
lumenc run .
```
