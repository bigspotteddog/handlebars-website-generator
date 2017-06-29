# handlebars-website-generator

## Run the template server:

```
$ java -jar handlebars-proto-4.0.5.jar -sx .html -d <template folder>
```

## Generate the website to a folder:

```
wget --mirror --convert-links --adjust-extension --page-requisites --no-parent http://localhost:6780
```

## A simple example

### header.html
```
<!DOCTYPE html>
<html lang="en">
<body>
```

### index.html
```
{{> header}}
<h1>Sample Content</h1>
{{> footer}}
```

### footer.html
```
</body>
</html>
```

### Run the server
```
$ java -jar handlebars-proto-4.0.5.jar -sx .html -d simple
```

### Generate the website
```
wget --mirror --convert-links --adjust-extension --page-requisites --no-parent http://localhost:6780
```
