# Updating to "nxblu" CSS

Major OE CSS version change: 5.x.x to 6.x.x

## Overview

1. Replace the 2 light and dark CSS files with a single new CSS file
2. Update OE panel with the new UI buttons to change themes
3. Manage theme classes on `<html>`

> iDG is setup to demo the following setup

### 1) CSS and `<head>` changes

Replace the 2 light and dark CSS files:

```
<link rel="stylesheet" type="text/css" data-theme="dark" href="/assets/2ab3e0f0/dist/css/style_oe_dark.3.css" media="none">
<link rel="stylesheet" type="text/css" data-theme="light" href="/assets/2ab3e0f0/dist/css/style_oe_light.3.css>
```

With the update CSS files from nxblue/dist



---
#### note: `style_eyedraw_doodles.css`

This is unchanged, and is still in 'newblue', as it only provides the CSS for the Eyedraw doodle icons in edit mode. _(btw. it only needs loading when a User is editing an Eyedraw)_


`<link rel="stylesheet" type="text/css" href="/assets/2ab3e0f0/dist/css/style_eyedraw_doodles.css">`

---





