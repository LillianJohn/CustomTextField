# CustomTextField
在我们平时开发的时候，避免不了要封装控件，提高复用性，下面小demo时对textfield进行简单封装
简单用法：
1、textfield左视图文字，图片
[self.leftTextField setLeftViewImage:@"leftImage"];
[self.leftTextField setLeftViewText:@"左信息："];
2、textfield右视图
[self.rightImageField setRightViewImage:@"rightImage"];
3、textfield阴影
[self.leftTextField setInnerShadow];

属性说明：
/**占位字符*/
@property (nonatomic, copy) NSString *placeHolder;
/**字体大小*/
@property (nonatomic, assign) CGFloat fontSize;
/**字体颜色*/
@property (nonatomic, copy) id textColors;
/**对齐方式*/
@property (nonatomic, assign) NSTextAlignment textAlignments;

方法说明：
/**
 设置左视图文字

 @param leftStr 文字
 */
- (void)setLeftViewText:(NSString *)leftStr;
/**
 设置左视图image

 @param imageStr 图片名称
 */
- (void)setLeftViewImage:(NSString *)imageStr;
/**
 设置右视图image

 @param imageStr 图片名称
 */
- (void)setRightViewImage:(NSString *)imageStr;
/**设置内阴影*/
- (void)setInnerShadow;
