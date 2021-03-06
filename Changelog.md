Changelog
=====================

0.9.2
-------------
All attributes on sencha widgets (`<st:xxx>`) that do not contain a namespace (e.g. ng:controller, ...) are
now removed from the dom, as they only serve as input attributes to sencha touch. By this, the dom stays small.
The options that are used to create the sencha widget are appended as a comment within every sencha widget tag.

The application requires the meta tag `<meta name="auto-start" content="true">` to be present.
This is needed to prevent initialization during unit tests.

CSS-Bugfix for `<st:spacer>`, `<st:list>` and `<st:grouped-list>` (did not work before).

`st:event` now takes the handlers as json.

Added `$navigate` service and `$navigate` expression.
Removed `$show` and `$hide` services. Use `$navigate` for this.

Extended `$waitDialog` service.

Added paging support for arrays via `$paged`.

Added `st:shared-controller`.

Added `st:if`

Added `st:radiofield` support.

Added `st:enabled` support.

Added `<st:selectfield>` with special attribute `options` as angular expression, so that it can be used without stores.

Added `ng:validate` and `ng:format` support.

Added support for `<st:numberfield>`, `<st:emailfield>` and `<st:urlfield>`

Added `$groupBy` for arrays.

0.9.1
-------------
- Update the syntax to use elements instead of the st:xtype attribute


0.9.0
-------------
- Initial release, incomplete
