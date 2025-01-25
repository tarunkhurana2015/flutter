# flutter

Flutter build system is consisted of 3 pillars
1. Widget
2. RenderObject
3. Element

`No matter how aggressively you compose your widget tree, the widgets that are ac‐
tually responsible for the rendering will always extend the RenderObjectWidget
class. Even if you, as a developer, don’t do it explicitly, you should know that this is
what is happening deeper in the widget tree. You can always verify this by following
the nesting of the build methods.
`
![image](https://github.com/user-attachments/assets/ccade6ee-2120-4831-948b-323dd813b11c)

