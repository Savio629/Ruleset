# AsyncAPI Error Ruleset

### asyncapi-info-version
**Type: Update**
Error message: The latest version is not used. You should update to the "2.5.0" version.

**Bad Example**

```yaml
asyncapi: "2.0.0"
```

**Good Example**

```yaml
asyncapi: "2.5.0"
```
**Recommended:** No

### asyncapi-info-description
**Type: Update**
Error message: Info "description" must be present and non-empty string.
**Before Fix**

```yaml
asyncapi: "2.5.0"
info:
  title: Awesome API
  version: "1.0"
```

**After Fix**

```yaml
asyncapi: "2.5.0"
info:
  title: Awesome API
  description: A very well-defined API
  version: "1.0"
```
**Recommended:** Yes

### asyncapi-schema
**Type: Insert**
Error message: "info" property must have required property "title"
**Bad Example**

```yaml
asyncapi: "2.5.0"
info:
  title: Awesome API
  version: "1.0"
```

**Good Example**

```yaml
asyncapi: "2.5.0"
info:
  title: Awesome API
  description: A very well-defined API
  version: "1.0"
```
**Recommended:** Yes
