---
title: My New Post
date: 2022-04-26 16:39:19
tags:
---
```
<div class="container">
  <h1>Works</h1>
  <ul class="row-fluid block-grid-4">
  {{#each model as |w index|}}
    <li>
      <h5>{{w.title}}</h5>
      <p>Owner: {{w.owner}}</p>
      <p>{{#link-to "work" w.id}}<img class="img-responsive img-rounded" src={{w.image}} alt={{w.title}}>{{/link-to}}</p>
    </li>
  {{/each}}
  </ul>
</div>
```