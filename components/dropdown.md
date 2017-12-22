---
name: Dropdown
category: Components
---
**When to use**
- A dropdown allows users to select one option from a list.
- Use sparingly — only when a user needs to choose from about seven to 15 possible options and you have limited space to display the options.

**When to consider something else**
- If the list of options is very short. Use radio buttons instead.
- If the list of options is very long. Let users type the same information into a text input that suggests possible options instead.
- If you need to allow users to select more than one option at once. Users often don’t understand how to select multiple items from dropdowns. Use checkboxes instead.
- For site navigation (use the navigation components instead).

**Guidance**
- Test dropdowns thoroughly with members of your target audience. Several usability experts suggest they should be the “UI of last resort.” Many users find them confusing and difficult to use.
- Avoid making options in one dropdown menu change based on the input to another. Users often don’t understand how selecting an item in one impacts another.
- When most users will (or should) pick a particular option, make it the default: `<option selected="selected">Default</option>`
- Don’t use JavaScript to automatically submit the form (or do anything else) when an option is selected. Offer a “submit” button at the end of the form instead. Users often change their choices multiple times. Auto-submission is also less accessible.

**Accessibility**
- If you customize the dropdown, ensure it continues to meet the the accessibility requirements that apply to all form controls.
- Make sure your dropdown has a label. Don’t replace it with the default menu option (for example, removing the “Select list:” label and just having the dropdown read “Select an item" by default).
- Don’t use JavaScript to automatically submit the form (or do anything else) when an option is selected. Auto-submission disrupts screen readers because they select each option as they read them.

```example.html
<div class="form-group">
  <label for="sel1">Select list:</label>
  <select class="form-control" id="sel1">
    <option>1</option>
    <option>2</option>
    <option>3</option>
    <option>4</option>
  </select>
</div>
```