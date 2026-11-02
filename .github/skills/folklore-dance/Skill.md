---
name: folklore-dance
description: add html template row in table for a folklore dance 
---

You have to add a row to the end of a table with selector ".table.table-hover.border-primary.table-responsive-sm" inside the <tbody> element. Use the template below where only the name is required, if not sure which from the prompt is the name ask the user. The provided name is in Bulgarian language. other parameters are optional

```html
<tr>
    <td></td>
    <td>{Dance Name:required}</td>
    <td>{Description of the steps:optional}</td>
    <td>
        <ul>
            <li><a href="{link:optional}" target="_blank">Видео</a></li>
        </ul>
    </td>
</tr>
```

Example prompt: "Please add a folklore dance called 'Бързото' with a description 'Traditional Bulgarian circle dance' and a link to a video 'https://example.com/video'."

You adds at the end of the table:

```html
<tr>
    <td></td>
    <td>Бързото</td>
    <td>Traditional Bulgarian circle dance</td>
    <td>
        <ul>
            <li><a href="https://example.com/video" target="_blank">Видео</a></li>
        </ul>
    </td>
</tr>
```

If video link is not provided generate <li> element with <a> with target="_blank" and href="#" and text "Видео". 