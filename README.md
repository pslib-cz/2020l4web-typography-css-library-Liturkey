# Litography
Simple CSS library for creating text pages with abnormal speeds.

**Author:** [*Lukáš Pánek*](https://github.com/Liturkey)

## Demo site
Link to **[demo](http://liturkey.github.io/litography)** site for preview.
## Dependecies
It is recommended to use [normalize.css](https://github.com/necolas/normalize.css) with this library. But it is optional.
## Implementation
```html
<!DOCTYPE html>
<html lang="en">
<head>
    ...
    <link rel="stylesheet" href="normalize.css">
    <link rel="stylesheet" href="typography.css">
    ...
</head>
```
## Usage
This library edits some basic elements for better readability. This includes elements like:
* h1 - h6
* p
* section

They don't need the `.lit` class to work.
## Components
Litography also includes some stylized components to make your pages stand out.

### Container
The basic feature of Litography. Creates responsive container with fixed width. It has a width of 1200px.

```html
<div class="lit container">
    ...
    Your content
    ...
</div>
```

### Meta
Basic summary of meta data like author, date of creation atc.
```html
<div class="lit meta">
    <ul>
        <li>Author: Lukáš Pánek</li>
        <li>Date: 28. 9. 2020</li>
    </ul>
</div>
```
### Perex
Short summary of content of the page.

```html
<p class="lit perex">This is perex.</p>
```

### Images
You can include small images or full width images that break the container.

```html
<img class="lit responsive margins" src="./link/to/image.jpg" alt="">
<img class="lit full width margins" src="./link/to/image.jpg" alt="">
```

You can also use figure and figcaption for images with description.
```html
<figure class="lit small">
    <img src="./link/to/image.jpg" alt="" class="lit">
    <figcaption>Your description</figcaption>
</figure>
```

### Tables
Simple but powerful table system. You can create stripped tables, tables with different backgrounds and other.

```html
<table class="lit margins stripped">
    <thead>
    <tr>
        <th>Jméno</th>
        <th>Přijmení</th>
        <th>Věk</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <th>Francesco</th>
        <td>Sanvito</td>
        <td>92</td>
    </tr>
    <tr>
        <th>Daniel</th>
        <td>Cvejn</td>
        <td>18</td>
    </tr>
    <tr>
        <th>Jan</th>
        <td>Novák</td>
        <td>20</td>
    </tr>
    </tbody>
</table>
```

## License

This library was created with the GNU GENERAL PUBLIC license. You can use and edit this library however you want.