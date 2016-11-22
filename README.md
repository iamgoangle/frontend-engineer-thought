## CSS at the top inside `</head>`, JS at the bottom before `</body>`
We think about prevention browser rendering blocking resource. So the browser can execution and displaying without delay.
Because of if we place `<script>` at a top, rendering engine will be displayed until js resources has loaded. That's means we allow rendering engine displays
`<body>` as fast as it can, before execution JS

## Avoid inline / embedded code
CSS / JS inline or embedded code able to reduce HTTP request / DNS lookup, but it make large HTML file.
It useful when we have small asset and need to display some temporary campaign or notice banner.

Use external css is loaded from `<link>` and js loaded from `<script src="">` tag

## Try out async
`<script async src="example.js"></script>`
Load js assets with async (parallel download), HTML request has limitation load asset at the same time
[https://www.keycdn.com/blog/parallel-downloads-across-domains/](https://www.keycdn.com/blog/parallel-downloads-across-domains/)
