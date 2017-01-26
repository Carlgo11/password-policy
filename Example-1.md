# Example 1

This is just a basic example of how a password policy file could look like. For a more in depth look of specific site-requirements see the other examples.

```yaml
# YAML example
minimum: 6
maximum: 100
characters: [a-Z, 0-9, U+0021-U002F,U+003A-U+0040]
```

```xml
<!--- XML example ---->
<minimum>6</minimum>
<maximum>100</maximum>
<characters>
 a-Z,
 0-9,
 U+0021-U002F,
 U+003A-U+0040
</characters>
```
