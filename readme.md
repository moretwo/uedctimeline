UEDC Timeline
=========
Version 0.1.9 ( *象征性写写的，可能就一个版本了* )

Website: 还没域名

Demo: <http://fed.hz.netease.com/design/demo/uedctimeline/>   _只有杭州本地可以预览_

###背景

+ 实验背景：以纵向时间轴的形式展示 UEDC内部活动记录，配合图文预览设计资料内容
		 视觉设计到前端页面的相关技术实践，写着玩

+ 版权：用了很多开源的东西，谈不上版权，都是修修改改的活儿

+ 设计资料：

	1. UEDC 视觉设计大赛 作品
	2. UEDC 运动会 活动花絮、照片
	3. UEDC 精选分享资料 （收集整理中）
	4. UEDC blog 关于我们文案

###工具
工具： sketch  PS  DW    Edge Code    Chrome    Safari    字体图标生成（在线）

####一、视觉设计

1. 响应式页面设计，sketch 页面视觉包括移动端显示效果

2. 完成页面框架设计，以画布为中心，timeline 平分页面，解决页面的基本布局问题

3. 图标，使用 ionicons-1.5.2 开源  icons 设计，

4. 精简页面元素，元素间规范间距、居中对齐方式

      配图 + 标题 -副标题  +icons

5. 模块化图片展示区域，便于复用

6. 色彩  标志标准色



####二、切图环节

>让很多前端哥哥们非常苦恼，因为那是像素级的苦逼体力活儿，不得不说，PS cc 14.2以上版本新推出的  从图层自动生成图片功能 非常实用 ；
>
>仅针对DEMO上的视觉效果，简单分析我只要将 LOGO 切出来即可（sketch 切图功能已经非常成熟好用可直接生成SVG），其它效果和图标都交给CSS3、 font icons 解决



1. uedc logo 以SVG 格式生成 ，ps 玩家 可以考虑  用AI 生成

2. fonticons 字体图标灰常的流行，实现流程  矢量图标 to SVG 》svg  to font  这里推荐在线生成 font icons的工具  https://icomoon.io/app/#/select
	以SVG 格式上传图标，import icons  > font ，下载，demo 中使用


####三、前端页面

1. DW cc   HTML +CSS +JS ，在实时视图中完成页面调试

2. adobe Edge  Code cc 更轻量级的纯文字网页编辑器 (有代码提示与调色盘)，前端哥哥们更喜欢 Sublime Text
>Co 视觉党的选择 有一个比较性感的功能可以通过CSS相对路径找到资源图片，在# 16进制 代码上可以快速预览颜色
3. 响应式 页面控制， NEC css @media ，在不同分辨率 下，页面宽度发生改变，CSS随之实现不同样式效果几个熟悉的尺寸，320，480，640，768，1000，1440，还要考虑是否是 devicePixelRatio
