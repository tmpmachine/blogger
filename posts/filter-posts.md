# by Label
Filter posts by labels that __has any label__ with name __Music__ in it.
```xml
<b:loop values='data:posts where (post => post.labels any (label => label.name == "Music"))' var='post'>
   <a expr:href='data:post.url'><data:post.title/></a>
</b:loop>
```

Filter posts by labels that __has no label__ with name __Music__ in it.
```xml
<b:loop values='data:posts where (post => post.labels none (label => label.name == "Music"))' var='post'>
   <a expr:href='data:post.url'><data:post.title/></a>
</b:loop>
```
