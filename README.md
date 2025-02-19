# Moved

**This package has moved** and is now available at [@dile/ui](https://github.com/Polydile/dile-components). Please update your dependencies. This repository is no longer maintained. You can read the documentation at [Dile Components](https://dile-components.com/).

# DileCloseDocumentClickMixin

Mixin to close custom elements when user do click in any area of the document.

This mixin, that you may apply to any Custom Element,  offers a way to close elements when the user clicks in any area of the document.

## Usage

Install it:

```bash
npm i dile-close-document-click-mixin
```

To use it you olny need to extend your custom element class with the mixin.

```javascript
import { DileCloseDocumentClickMixin } from 'dile-close-document-click-mixin/dile-close-document-click-mixin.js';

class MyElement extends DileCloseDocumentClickMixin(HTMLElement) {
  // your custom element code...
}
```

To do it's work, the mixin depends on a close() method created in your custom element class.

## Available methods

The mixin also provides two utility methods:

- **closeAll()**: Close all the elements of this type
- **closeOthers()**: Close the other items of this type (distinct to this)

