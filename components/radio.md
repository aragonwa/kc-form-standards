---
name: Radio
category: Form Controls
---

**When to use**

* Radio buttons allow users to see all available choices at once and select exactly one option.
* When the number of available options can fit onto a mobile screen.

**When to consider something else**

* Consider checkboxes if users need to select more than one option or if there is only one item to select.
* Consider a dropdown if you don’t have enough space to list out all available options.
* If users should be able to select zero of the options.

**Guidance**

* Users should be able to tap on or click on either the text “label” or the radio button to select or deselect an option.
* Options that are listed vertically are easier to read than those that are listed horizontally. Horizontal listings can make it difficult to tell which label pertains to which radio button.
* If you customize, make sure selections are adequately spaced for touch screens.
* Use caution if you decide to set a default value. Setting a default value can discourage users from making conscious decisions, seem pushy, or alienate users who don’t fit into your assumptions. If you are unsure, leave nothing selected by default.

**Accessibility**

* Group related radio buttons together with `<fieldset>` and describe the group with `<legend>`.
* Each radio button should have a `<label>`. Associate the two by matching the `<label>`’s for attribute to the `<input>`’s id attribute.
* The title attribute can replace `<label>`.

```example.html
<fieldset>
  <legend class="sr-only">Radio button example</legend>
  <div class="radio">
    <label for="option1">
      <input id="option1" type="radio" checked name="radiooptions" value="option1">
      Option 1
    </label>
  </div>
  <div class="radio">
    <label for="option2">
      <input id="option2" type="radio" name="radiooptions" value="option2">
      Option 2
    </label>
  </div>
  <div class="radio">
    <label for="option3">
      <input id="option3" type="radio" name="radiooptions" value="option3">
      Option 3
    </label>
  </div>
  <div class="radio disabled">
    <label for="option4">
      <input id="option4" type="radio" name="radiooptions" value="option4" disabled />
      Option 4 (is disabled)
    </label>
  </div>
</fieldset>
```
