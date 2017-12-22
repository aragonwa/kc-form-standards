---
name: Help text
category: Form Controls
---
**When to use**
- Block level help text for form controls
- Avoid using placeholder text in form fields, as this will disappear once content is entered into the form field
- Instead use hint text for supporting contextual help, this will always be shown
- Hint text should sit above or below a form field
- Ensure hint text can be read correctly by screen readers

```example.html
<label for="inputHelpBlock">Input with help text</label>
<input type="text" id="inputHelpBlock" class="form-control" aria-describedby="helpBlock">
<span id="helpBlock" class="help-block">A block of help text.</span>
```