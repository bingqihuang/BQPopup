# BQPopup
A PopupController which can scroll when contains a lot of subviews.

BQPopup支持ARC，Autolayout。

## 声明
本项目是在carsonperrotti大神的项目基础上修改的，当时是为了满足项目需求，实现了可滚动浏览。

附：
carsonperrotti项目地址：
[https://github.com/carsonperrotti/CNPPopupController](https://github.com/carsonperrotti/CNPPopupController)

## 项目效果图
### 图比较大，耐心等待...
![BQPopup](./BQPopupController/BQPopup.gif)

## 属性列表

```bash
/* View title */
@property (nonatomic, strong) NSAttributedString *title;

/**
 *  BQPopupHeight, when popupStyle is BQPopupStyleActionSheet,if popupHeight less than or equal keyWindow.frame.size.height/2, the final popupHeight is popupHeight, or it will be setted as keyWindow.frame.size.height/2.
 */
@property (nonatomic, assign) CGFloat popupHeight;

/**
 *  popupWidth，normally is screenWidth.
 */
@property (nonatomic, assign) CGFloat popupWidth;

/* content view array */
@property (nonatomic, strong) NSArray *contentsArray;

/* buttons in content views */
@property (nonatomic, strong) NSArray *buttonArray;

/* final button in content views, There's a margin to previous view */
@property (nonatomic, strong) BQButton *finalButton;

/* Controller delegate, it will controle the presentation and dismiss of the controller */
@property (nonatomic, weak) id <BQPopupControllerDelegate> delegate;

/*************************************/

/**
 *  The way to show PopupController, default is BQPopupStyleAlert.
 */
@property (nonatomic, assign) BQPopupStyle popupStyle;

/**
 *   Controls whether controller dismiss when touch background. Default Yes.
 */
@property BOOL dismissOnTouchBackground;

/**
 *  Controls whether show scrollview's vertical indicator, default is NO.
 */
@property BOOL showVerticalScrollIndicator;

/**
 *  cornnerRadius of scrollview and contentview, default is 8.0f.
 */
@property (nonatomic, assign) CGFloat cornerRadius;

/**
 *  contentview background color, default is whiteColor
 */
@property (nonatomic, strong) UIColor *contentBackgroundColor;

/**
 *  default is (16.0f, 16.0f, 16.0f, 16.0f).
 */
@property (nonatomic, assign) UIEdgeInsets contentInsets;

/**
 *  padding for subviews in contentView, default 12.0f
 */
@property (nonatomic, assign) CGFloat paddingForSubviews;

/**
 *  default 16.0f;
 */
@property (nonatomic, assign) CGFloat finalButtonPadding;

```

## 欢迎Star
我正在iOS路上，追随大牛们的步伐。欢迎关注：

新浪微博：[http://www.weibo.com/2609034524/profile?rightmod=1&wvr=6&mod=personinfo](http://www.weibo.com/2609034524/profile?rightmod=1&wvr=6&mod=personinfo)

博客地址：[http://bingqihuang.github.io/](http://bingqihuang.github.io/)
