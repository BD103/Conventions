# Front End / CSS

This standard is for pure CSS which you are actively editing. Compiled CSS does not apply.

## Speed

Try to put all your styling inside a single CSS file. This increases load time. If you cannot do this, then see if you can enable file-caching for your server.

## Body First

Always have your global CSS first. Place the body selector first.

```css
body {
  background-color: black;
  color: white;
}
```

## Single Modifier

If there is only a single modifier, then do not add indentation. Make it shorthand.

```css
.content {padding: 1rem;}
```

## Specific

Always be as specific as possible. Ex: If you are changing the background color, use `background-color` instead of `background`.
