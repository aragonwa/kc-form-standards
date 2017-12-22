---
name: Table
category: Components
---

**When to use**
- Tables show tabular data in columns and rows

**When to consider something else**
- Depending on the type of content, consider using other presentation formats such as definition lists or hierarchical lists.

**Guidance**
- When comparing rows of numbers, align numbers to the right in table cells
- Use a caption to describe the table in the same way you would use a heading. It can help users find, navigate and understand tables.

**Accessibility**
- Simple tables can have two levels of headers. Each header cell should have `scope="col"` or `scope="row"`.
- Complex tables are tables with more than two levels of headers. Each header should be given a unique id and each data cell should have a headers attribute with each related header cell’s id listed.
- When adding a title to a table, include it in a `<caption>` tag inside of the `<table>` element.

```example.html
<table class="table">
<caption class="heading-small">Customer accounts</caption>
  <thead>
    <tr>
      <th scope="col">Name</th>
      <th scope="col">ID</th>
      <th class="text-right" scope="col">Amount</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Bob</th>
      <td>1234</td>
      <td class="text-right">$7,000</td>
    </tr>
    <tr>
      <th scope="row">Ralph</th>
      <td>3423</td>
      <td class="text-right">$1,000</td>
    </tr>
    <tr>
      <th scope="row">Cher</th>
      <td>1222</td>
      <td class="text-right">$9,000</td>
    </tr>
    <tr>
      <th scope="row">Simon</th>
      <td>3333</td>
      <td class="text-right">$8,000</td>
    </tr>
    <tr>
      <th scope="row">Lisa</th>
      <td>5656</td>
      <td class="text-right">$2,000</td>
    </tr>
  </tbody>
</table>
```