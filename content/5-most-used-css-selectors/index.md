---
title: "5 Most Used CSS Selectors"
description: "1. * (Universal Selector)"
date: "2020-01-31T03:37:29.523Z"
categories: []
published: true
canonical_link: https://medium.com/@tiwari.apoorv1316/5-most-used-css-selectors-79cb84550cec
redirect_from:
  - /5-most-used-css-selectors-79cb84550cec
---

### 1\. \* (Universal Selector)

```
* {
 margin: 0;
 padding: 0;
 box-sizing : border-box;

}
```

The star symbol will target every single element on the page. Many developers will use this trick to zero out the margin and padding. While this is certainly fine for quick tests, I'd advise you to never use this in production code.

### 2\. # (ID Selector)

```
#container {
   width: 960px;
   margin: auto;
}


```

Prefixing the hash symbol to a selector allows us to target by id. This is easily the most common usage, however, be cautious when using id selectors. id selectors are rigid and don't allow for reuse.

### 3 .X (Class Selector)

```
.paragraph {
  color: blue;
}
```

This is a `class` selector. The difference between id’s and classes is that, with the latter, you can target multiple elements. Use classes when you want your styling to apply to a group of elements.

### 4\. X Y (Descendant selector)

```
li a {
  text-decoration: none;
}
```

The next most comment selector is the descendant selector. When you need to be more specific with your selectors, you use these. For example, what if, rather than targeting _all_ anchor tags, you only need to target the anchors which are within an unordered list? This is specifically when you'd use a descendant selector.

### **5 X (Type Selector)**

```
a { color: red; }
ul { margin-left: 0; }
```

What if you want to target all elements on a page, according to their type, rather than an id or class name? Keep it simple, and use a type selector. If you need to target all unordered lists, use ul{}.
