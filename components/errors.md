---
name: Errors in forms
category: Validation
---

**Guidance**
- Recovering from errors can be hard for users, especially if a page contains multiple errors.

- Simplify forms by rewriting and where possible, splitting long forms across multiple pages.

- Add a symbol, asterisk for example, to lable to indicate a field is required. Make sure to include a way to alert screen readers to the required field.

- If possible, summarise errors at the top of the page. Include a link to each of the issues.

- Only show error validation messages or stylings after a user has interacted with a particular field.

```example.html
<div class="panel panel-danger">
  <div class="panel-heading">Your form contains errors</div>
  <div class="panel-body">
    <ul class="list-unstyled">
      <li><a href="#example-username">Link to error</a></li>
    </ul>
  </div>
</div>

<div class="form-group has-error has-feedback">
  <label class="control-label" for="example-username">Enter a username</label>
  <span class="text-danger"><span class="fa fa-asterisk"></span><span class="sr-only">Required field</span></span>
  <input type="text" class="form-control" id="example-username" aria-describedby="example-usernameStatus">
  <span id="example-usernameStatus" class="sr-only">(error)</span>
</div>

```