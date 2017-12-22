---
name: Checkbox
category: Form Controls
---
**When to use**
- When a user can select any number of choices from a set list.
- When a user needs to choose “yes” or “no” on only one option (use a stand-alone checkbox). For example, to toggle a setting on or off.
- When users need to see all the available options at a glance.

**When to consider something else**
- If there are too many options to display on a mobile screen.
- If a user can only select one option from a list (use radio buttons instead).

**Guidance**
- Users should be able to tap on or click on either the text label or the checkbox to select or deselect an option.
- List options vertically if possible; horizontal listings can make it difficult to tell which label pertains to which checkbox.
- Avoid using negative language in labels as they can be counterintuitive. For example, “I want to receive a promotional email” instead of “I don’t want to receive promotional email.”
- If you customize, make sure selections are adequately spaced for touch screens.

**Accessibility**
- Surround a related set of checkboxes with a `<fieldset>`. The `<legend>` provides context for the grouping. Do not use fieldset and legend for a single check.
-Each input should have a semantic id attribute, and its corresponding label should have the same value in it’s for attribute.
- The title attribute can replace `<label>`.

```example.html
 <fieldset>
    <legend class="sr-only">Checkbox example</legend>
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
    <div class="checkbox disabled">
      <label for="option4">
        <input id="option4" type="checkbox" value="" disabled>
        Option two is disabled
      </label>
    </div>
</fieldset>
```
