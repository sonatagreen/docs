---
sort: 3
---

# `:bank, $:, "buccol", {$bank p/(list moss)}`

Form a mold which recognizes a tuple.

## Normalizes

The tuple the length of `p`, normalizing each item, defaulting
where the tuple does not match.

Void if `p` is empty.

## Defaults to

The tuple the length of `p`, defaulting each items.

Crashes if `p` is empty.

## Syntax

Regular: *running*.

Irregular: `{a b c}` is `:bank(a b c)`.

## Examples

```
~zod:dojo> =foo :bank(p/@ud q/@tas)

~zod:dojo> (foo 33 %foo)
[p=33 q=%foo]

~zod:dojo> `foo`[33 %foo]
[p=33 q=%foo]

~zod:dojo> $:foo
[p=0 q=%$]
```