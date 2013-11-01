drawer_nav
==========

Drawer Navigation View Controller

1 Usage （使用说明）
Please refer to the demo. (请参照项目demo)

2 Description of Properties and methods (一些属性的说明)

/* Properties */
leftViewVisibleWidth        // Width of left view  (左边view的宽度)

rightViewVisibleWidth       // Width of right view（右边view的宽度）

leftViewCenterX             // The minimum point of x to trigger show center view that you dragging left view back when the left view is shown
                           （当左边view显示的时候，往回拖松开的时候的这个坐标，如果大于设置的值就显示center view,如果小于就还是显示left view)
                           
rightViewCenterX            //

showDrawerMaxTrasitionX     // The minimum width to trigger show left of right view that you dragging center view when center view is shown 
                            (当center view 在最中间的时候，你拖动center view松手时，如果拖动的距离大于这个值就显示left 或者right view,如果小于这个值还是显示center view)

/*  Methods  */
- (void)showRightView;                 
- (void)showCenterView:(BOOL)animate;
- (void)showLeftView;

- (void)disableGestureForDrawerView;
- (void)enableGestureForDrawerView;

- (void)initialDrawerViewController;


showRightView
showLeftView
