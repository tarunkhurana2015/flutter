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

## Performance 

The best performance practices in the preceding list are also the reason why it’s
better to decouple your widgets into other custom widgets rather than extract
them into helper methods such as Widget buildMyWidget(). The widgets ex‐
tracted into methods still access the same context or call setState, which causes
the whole encapsulating widget to rebuild, so it’s generally recommended to pre‐
fer widget classes rather than methods.
