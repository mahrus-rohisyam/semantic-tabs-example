# jQuery Semantic Tabs v1.0.0

jQuery SemanticTabs is a jQuery plugin that can convert semantic HTML tags to tabs.

## Options

componentClass:
String. `semantic-tabs-component` by default. A CSS class to group elements of heads and components.

## head:

String. `h3` by default. An HTML tag or element as a head.

## headsID:

String. `semantic-tabs-heads` by default. A CSS ID for a group of heads.

## Demo

See the demo section for the usage.

### HTML File

```
  <!DOCTYPE html>
<html>
  <head>
    <title>jQuery Semantic Tabs</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div id="semantic-tabs">
      <h3>Title 1</h3>
      <p>This is the content of 1.</p>
      <p>This is the content of 1.</p>
      <p>This is the content of 1.</p>
      <h3>Title 2</h3>
      <p>This is the content of 2.</p>
      <p>This is the content of 2.</p>
      <p>This is the content of 2.</p>
      <h3>Title 3</h3>
      <p>This is the content of 3.</p>
      <p>This is the content of 3.</p>
      <p>This is the content of 3.</p>
    </div>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="../jquery-semantic-tabs.js"></script>
    <script src="main.js"></script>
  </body>
</html>
```

### CSS File

```
#semantic-tabs {
  border: 2px solid #555;
  border-radius: 4px;
  font-family: Helvetica, Arial, sans-serif;
}

#semantic-tabs-heads {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

#semantic-tabs-heads {
  background: #555;
}

#semantic-tabs-heads li {
  color: #fff;
  cursor: pointer;
  padding: 10px 15px;
}

#semantic-tabs-heads li.active {
  color: #000;
  background: #fff;
}

```

### JS File
```
$('#semantic-tabs').semanticTabs({
	head: 'h3'
});
```
> Ini menunjukkan plugin akan mengambil ID `#semantic-tabs` pada code di bagian HTML dan memberikan konfigurasi `head: h3` pada semanticTabs