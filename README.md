# quill-table-ui
A module for table UI in Quill

# Online Demo
[quill-table-ui Codepen Demo](https://codepen.io/volser/pen/QWWpOpr)

# Requirements
[quilljs](https://github.com/quilljs/quill) v2.0.0-dev.3

# Installation
```
npm install quill-table-ui
```

# Usage
Load quill and style dependencies
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/quill/2.0.0-dev.3/quill.min.js" type="text/javascript"></script>
<script src="https://unpkg.com/quill-table-ui@1.0.5/dist/umd/index.js" type="text/javascript"></script>
```
```
<link href="https://cdnjs.cloudflare.com/ajax/libs/quill/2.0.0-dev.3/quill.snow.min.css" rel="stylesheet">
<link href="https://unpkg.com/quill-table-ui@1.0.5/dist/index.css" rel="stylesheet">
```

ES6
```
import * as QuillTableUI from 'quill-table-ui'

Quill.register({
  'modules/tableUI': QuillTableUI
}, true)

window.onload = () => {
  const quill = new Quill('#editor-wrapper', {
    theme: 'snow',
    modules: {
      table: true,
      tableUI: true,
    }
  })
}
```
