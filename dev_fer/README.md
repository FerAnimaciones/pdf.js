# NPM INSTLL

Verificar la cache si no permite instalar paquetes.
```
npm cache verify
```

Eliminar el archivo "package-lock.json" si continua sin poder instalar.

# Compilation

```
$ gulp minified
```


# viewer
[/web/viewer.html](/web/viewer.html)

```

<script type="text/javascript">
const urlParams = new URLSearchParams(window.location.search);
if(urlParams.get("print")=="false"){
  document.getElementById("print").hidden = true;
}
if(urlParams.get("download")=="false"){
  document.getElementById("download").hidden = true;
}
if(urlParams.get("editor")=="false"){
  document.getElementById("editorModeButtons").hidden = true;
}
document.getElementById("openFile").hidden = true;
window.addEventListener('load', function () {
  PDFViewerApplication.preferences.set('pdfBugEnabled', true);
})
</script>


```

# app_options.js
[/web/app_options.js](/web/app_options.js)

```
defaultOptions.locale = {
  /** @type {string} */
  value:  "es-MX", //typeof navigator !== "undefined" ? navigator.language :
  kind: OptionKind.VIEWER,
};

```
