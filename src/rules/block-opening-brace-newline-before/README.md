# block-opening-brace-newline-before

Require or disallow a newline before the opening brace of blocks.

```css
    a 
      { color: pink; }
/**   ↑  
 * The newline before this brace */
```

## Options

`string`: `"always"|"never"`

### `"always"`

There *must always* be a single newline before the opening brace.

The following patterns are considered warnings:

```css
a{ color: pink; }
```

```css
a {color: pink;}
```

The following patterns are *not* considered warnings:

```css
a
{ color: pink; }
```

### `"never"`

There *must never* be whitespace before the opening brace.

The following patterns are considered warnings:

```css
a { color: pink; }
```

```css
a 
{color: pink;}
```

The following patterns are *not* considered warnings:

```css
a{ color: pink; }
```