### 说说children() find() parents() parent()区别
1. 今天在看jQuery的时候突然因为children()被拦住了，感觉不是很理解，就学习了一下，其实我的理解是children()之会向下取他的直属子元素;w3c上有一个关于children方法的demo，我觉得很能说明问题:函数只在当前jQuery对象匹配元素的所有子元素中查找，不会查找"孙子"以及更后代的元素。
2.  这样他就跟parent()的方法类似，只不过一个是向下一级找子元素，而parent方法是向上一级找父元素，这样closest()与parent()方法的作用相似；closest()从元素本身开始，逐级向上级元素匹配，并返回最先匹配的祖先元素。
3.  find()方法是会遍历当前选择器中所有匹配与之匹配的元素，而parents()是一直向上找自己的父级，直到DOM的根节点，parents(element),参数可以限制朝上找的范围；