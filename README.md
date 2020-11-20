#Cynet Widget Integration

### Adding the JavaScript
Add the following JavaScript snippet before the `</body>` on your page

`<script>!function(){var t,e,n;e=!1,(t=document.createElement("script")).type="text/javascript",t.src="https://cybersecurity-skill-tests.com/widget/frontend/dist/main.js",t.onload=t.onreadystatechange=function(){e||this.readyState&&"complete"!=this.readyState||(e=!0,window.cynetInit())},(n=document.getElementsByTagName("script")[0]).parentNode.insertBefore(t,n)}();</script>`

### Adding an embedded widget
To show an open, embedded widget on your page add the following HTML in the location you would like it shown and replace the values in `{}`

```
<div
    data-cynetwidget="true"
    data-cynetwidget-integration-id="{YOUR_INTEGRATION_ID}"
    data-cynetwidget-width="{OPTIONAL_WIDTH_IN_PIXELS}"
    data-cynetwidget-height="{OPTIONAL_HEIGHT_IN_PIXELS}"
></div>
```

### Adding a popup widget
Showing a widget in a popup is similar to the embedded version. Any HTML you add inside the widget's `<div></div>` will act as a link to open the popup.

```
<div
    data-cynetwidget="true"
    data-cynetwidget-type="modal"
    data-cynetwidget-integration-id="{YOUR_INTEGRATION_ID}"
    data-cynetwidget-width="{OPTIONAL_WIDTH_IN_PIXELS}"
    data-cynetwidget-height="{OPTIONAL_HEIGHT_IN_PIXELS}"
>
    <a href="#">Click Here</a>
</div>
```
