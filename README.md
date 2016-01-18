# SimpleExplorer
已经实现html解析和渲染功能

解析分为标记识别和DOM树构建两步, 标记识别利用状态机实现(HtmlToken, HtmlTag), DOM树构建利用栈实现(HtmlDomTree), 

DOM树遍历样例见HtmlParser.walkDomTree, 仅仅渲染了文本和图片(HtmlRendorTree, HtmlNode), HtmlParser是主控类

运行: java -jar simple_explorer.jar
输出
1.以深度优先打印DOM树里的可视化文本标记
2.输出渲染的位图,和jar包在同一个目录下,名称为rendor.bmp
