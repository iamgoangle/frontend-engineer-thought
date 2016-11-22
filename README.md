# Just a notes

## CSS at the top inside </head>, JS at the bottom before </body>
We think about prevention browser rendering blocking resources. To prevent displaying a page with delayed (white page) we should be placed <script> at a bottom, since rendering engine can be displayed until resources has loaded. That's means we allows rendering engine displays <body> as fast as it can, before execution JS.
