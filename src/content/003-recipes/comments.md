---
title: "Comments"
description: Recipes for interacting with WordPress comments using WPGraphQL
path: recipes/comments
---

## Query Comments

Comments in WordPress are typically used for user to user interactions. Comments are a really exciting part of WordPress and have many use cases. Let's look at some basic comment examples.

### Querying a list of Comments

```
{
  comments { 
    edges {
      node {
        id
        content
        date
      }
    }
  }
}
```

This will return a list of comments with each comment's id, content and date.