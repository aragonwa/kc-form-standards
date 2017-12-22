---
name: Text Input
category: Form Controls
---

**When to use**
- Text inputs allow people to enter any combination of letters, numbers, or symbols of their choosing (unless otherwise restricted). Text input boxes can span single or multiple lines.
-  If you can’t reasonably predict a user’s answer to a prompt and there might be wide variability in users’ answers.
- When using another type of input will make answering more difficult. For example, birthdays and other known dates are easier to type in than they are to select from a calendar picker.
- When users want to be able to paste in a response.

**When to consider something else**
- When users are choosing from a specific set of options.

**Guidance**
- The length of the text input provides a hint to users as to how much text to write. Do not require users to write paragraphs of text into a single-line input box; use a text area instead.
- Text inputs are among the easiest type of input for desktop users but are more difficult for mobile users.
- Only show error validation messages or stylings after a user has interacted with a particular field.
- Avoid using placeholder text that appears within a text field before a user starts typing. If placeholder text is no longer visible after a user clicks into the field, users will no longer have that text available when they need to review their entries. (People who have cognitive or visual disabilities have additional problems with placeholder text.)

**Accessibility**
- Avoid placeholder text for accessibility reasons. Most browsers’ default rendering of placeholder text does not provide a high enough contrast ratio.
- Avoid breaking numbers with distinct sections (such as phone numbers, Social Security Numbers, or credit card numbers) into separate input fields. For example, use one input for phone number, not three (one for area code, one for local code, and one for number). Each field needs to be labeled for a screen reader and the labels for fields broken into segments are often not meaningful.

**States**
- Default 
- Focus
- Error
- Success

```states.html
<div class="form-group">
  <label for="exampleInput">Default text label</label>
  <input type="text" class="form-control" id="exampleInput"/>
</div>

<div class="form-group">
  <label for="exampleFocusInput">Focus text label</label>
  <input type="text" class="form-control" id="exampleFocusInput"  />
</div>

<div class="form-group has-error">
  <label for="exampleInputError">Error text label</label>
  <input type="text" class="form-control " id="exampleInputError"  />
</div>

<div class="form-group has-success">
  <label for="exampleInputSuccess">Success text label</label>
  <input type="text" class="form-control " id="exampleInputSuccess" />
</div>
```