---
name: Button
category: Components
---
**When to use**
-  Use buttons for the most important actions you want users to take on your site, such as “download,” “sign up,” or “log out.”

**When to consider something else**
- If you want to lead users between pages of a website, use links instead.
- Less popular or less important actions may be visually styled as links.

**Guidance**
- Generally, use primary buttons for actions that go to the next step and use secondary buttons for actions that happen on the current page.
- Style the button most users should click in a way that distinguishes from other buttons on the page. Try using the “large button” or the most visually distinct fill color.
- Make sure buttons should look clickable—use color variations to distinguish static, hover and active states.
- Avoid using too many buttons on a page.
- Use sentence case for button labels.
- Button labels should be as short as possible with “trigger words” that your users will recognize to clearly explain what will happen when the button is clicked (for example, “download,” “view” or “sign up”).
- Make the first word of the button’s label a verb. For example, instead of “Complaint Filing” label the button “File a complaint.”
- At times, consider adding an icon to signal specific actions (“download”, “open in a new window”, etc).

**Accessibility**
- Buttons should display a visible focus state when users tab to them.
- When styling links to look like buttons, remember that screen readers handle links slightly differently than they do buttons. Pressing the Space key triggers a button, but pressing the Enter key triggers a link.

**States**
- Default 
- Hover
- Active
- Focus
- Disabled

```states.html
<button class="btn btn-default">Default</button>
<button class="btn btn-default active">Hover</button>
<button class="btn btn-default active">Active</button>
<button class="btn btn-default focus">Focus</button>
<button class="btn btn-default disabled">Disabled</button>
```