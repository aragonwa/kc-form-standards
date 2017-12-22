---
name: Fieldset
category: Form Controls
---

**When to use**
- Use fieldsets to group related form controls. The first element inside a fieldset must be a legend element which describes the group.

```example.html
<form>
  <fieldset>
    <legend>
      <h3>Fieldset example</h3>

    </legend>
    <div class="form-group">
      <label for="usernameInput">User name</label>
      <input type="text" class="form-control" id="usernameInput" />
    </div>

    <p><strong>Select all that apply</strong></p>
     <div class="checkbox">
      <label for="option1">
        <input id="option1" type="checkbox" value="option1" checked>
        Option 1
      </label>
    </div>
    <div class="checkbox">
      <label for="option2">
        <input id="option2" type="checkbox" value="option2">
        Option 2
      </label>
    </div>
    <div class="checkbox">
      <label for="option3">
        <input id="option3" type="checkbox" value="option3">
        Option 3
      </label>
    </div>
  </fieldset>
</form>
```
