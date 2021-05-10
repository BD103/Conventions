# Front End / HTML

HTML is the most used programming language. Note how I didn't say popular, just used.

Web development is a really popular frontier in the programming community. The client needs an HTML file to render.

## Base File

All HTML files should have this at least:

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>Title Here</title>
  <!-- Stylesheets and scripts -->
</head>

<body>
  <!-- Content -->
</body>

</html>
```

Note some important elements:

1. `<!DOCTYPE html>` You need this for HTML5
2. `<html lang="en">` Specifies the language
3. `charset="utf-8"` Compatability
4. `<meta name="viewport" content="width=device-width">` Sets width of page, necessary
5. Everything that is not seen by the client (excluding comments) is lowercase.

## Head

You should always have a header. This will include meta info, stylesheets, and JS libraries.

By JS libraries, I mean any Javascript file that doesn't run anything. It just includes functions / variables. This rule excludes libraries with the event listener `onload`. If the script runs something outside of a function or event handler, then put it at the bottom of the body tag.

## Body

The body tag can be exluded if nothing is included inside it. (_You wouldn't include the `<body>` tags in the [Base Files](#base-files) example._)

You may insert nodes inside this parent however you like, but non-library JS must be inserted at the very bottom. Here is an example:

```html
<body>
  <nav></nav>

  <div class="content">
    <h1>Hello, world!</h1>

    <p>Lorem ipsum...</p>
  </div>

  <script src="run.js"></script>
  <script>
    console.log('test');
  </script>
</body>
```

Do not put anything outside of the body and head tags. This is not to standard, and may not render properly.

## Classes and IDs

All classes and id names must be lowercase. Never use an underscore, instead use a dash.

> Eg. instead of `my_class` use `my-class`

## Indentation

Indents are two spaces, not 1 tab, not 4 spaces. Just 2.

`<!DOCTYPE>`, html, body, and head tags are not indented. Everything inside body and head tags are indented as normal.

```html
<!DOCTYPE html>
<html>

<head></head>

<body></body>

</html>
```
