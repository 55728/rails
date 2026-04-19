*   Fix `collection_radio_buttons` and `collection_check_boxes` generating
    a label `for` attribute that does not match the input `id` when a
    collection value is `nil`.

    *Kenta Ishizaki*

*   Skip blank attribute names in tag helpers to avoid generating invalid HTML.

    *Mike Dalessio*

*   Fix tag parameter content being overwritten instead of combined with tag block content.
    Before `tag.div("Hello ") { "World" }` would just return `<div>World</div>`, now it returns `<div>Hello World</div>`.

    *DHH*

*   Add ability to pass a block when rendering collection. The block will be executed for each rendered element in the collection.

    *Vincent Robert*

*   Add `key:` and `expires_in:` options under `cached:` to `render` when used with `collection:`

    *Jarrett Lusso*

Please check [8-1-stable](https://github.com/rails/rails/blob/8-1-stable/actionview/CHANGELOG.md) for previous changes.
