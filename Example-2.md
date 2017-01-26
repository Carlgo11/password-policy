# Example 2

In these examples I'll go over some of the possible solutions to link-specific password policies.

## Example 2:1

In this example the policy is specific to a link to the current site.

```yaml
# YAML example
site: /login.php
 minimum: 6
 maximum: 100
 characters: [a-Z, 0-9, U+0021-U002F,U+003A-U+0040]
```

```xml
<!--- XML example ---->
<policy>
 <site>/login.php</site>
 <minimum>6</minimum>
 <maximum>100</maximum>
 <characters>
  a-Z,
  0-9,
  U+0021-U002F,
  U+003A-U+0040
 </characters>
</policy>
```

## Example 2:2

In this example the policy is specific to a full URL. Therefor the site ownership would have to be validated somehow. One way of doing that would be to see if the hash of the current file is the same for that domain.

```yaml
# YAML example
site: http://example.org/login.php
 minimum: 6
 maximum: 100
 characters: [a-Z, 0-9, U+0021-U002F,U+003A-U+0040]
```

```xml
<!--- XML example ---->
<policy>
 <site>http://example.org/login.php</site>
 <minimum>6</minimum>
 <maximum>100</maximum>
 <characters>
  a-Z,
  0-9,
  U+0021-U002F,
  U+003A-U+0040
 </characters>
</policy>
```
