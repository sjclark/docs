---
id: 2e700683-1fb1-4cde-a019-67770ceabadf
blueprint: modifiers
title: 'Is Tomorrow'
modifier_types:
  - date
  - conditions
---
Returns `true` if a given date is tomorrow, using the server's time.

```yaml
date: January 1, 2000
```

::tabs

::tab antlers
```antlers
{{ if date | is_tomorrow }}
```
::tab blade
```blade
@if (Statamic::modify($date)->isTomorrow()->fetch()) ... @endif
```
::

```html
false
```
