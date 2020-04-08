# Stacked

Add attributes to HTML and create complex layouts

# Live Demo

[View Live Demo](https://regularmemory.blog/Stacked/)

See `index.html` for the demo's markup

# Basic Usage

Let's say you have a collection of nested div elements. You want some to be vertical or horizontal containers:

```html
<head>
    <link rel="stylesheet" type="text/css" href="stacked.css">
</head>
<body>
    <div vstack root>
        <div>hello world</div>
    </div>
</body>
</html>
```

```html
<head>
    <link rel="stylesheet" type="text/css" href="stacked.css">
</head>
<body>
    <div vstack root>
        <div hstack>
            <div hstack>Space</div>
            <div space></div>
            <div>Between</div>
        </div>
        <div hstack>
            <div space></div>
            <div>Space</div>            
            <div>Around</div>
            <div space></div>
        </div>        
    </div>
</body>
</html>
```

# Attributes

- `vstack`: vertically align child contents
- `hstack`: horizontally align child contents
- `space`: Takes up vertical or horizontal space in a greedy fashion
- `shrink`: combine with hstack or vstack to "shrink wrap" the contents

# Notes

All `attributes` should be applied to `div elements`. Div elements by default will, horizontally and vertically `center` their contents.
