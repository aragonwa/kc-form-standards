---
name: File upload
category: Form Controls
---
**When to use**
- A control that lets the user select a file.

**Accessibility**
- Use a native input using `type="file"`, rather than a custom implementation.

```example.html
<div class="form-group">
  <label for="exampleInputFile">Upload a file</label>
  <input type="file" id="exampleInputFile" />
</div>
```