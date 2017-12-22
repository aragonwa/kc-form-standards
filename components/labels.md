---
name: Labels
category: Form Controls
---
**When to use**
- All form fields should be given labels
- Don’t hide labels, unless the surrounding context makes them unnecessary
- Labels should be aligned above their fields
- Label text should be short, direct and in sentence case
- Avoid colons at the end of labels
- Labels should be associated with form fields using the for attribute

```example.html
<div class="form-group">
    <label for="exampleInputEmail1">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" />
  </div>
```