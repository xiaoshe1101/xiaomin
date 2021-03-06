## jQuery 使用过滤器方法缩小选择范围

###### first()
^除了所选元素的第一个元素之外，first方法会过滤掉所有其他元素；^
###### last()
^除了所选元素的最后一个元素之外，last方法会过滤掉所有其他元素；^

^**注意**：first和last方法都会去遍历整个DOM结构，找到符合的元素，然后只返回与之匹配的第一个或最后一个元素；（将匹配元素集合缩减为集合中的第一个（或最后一个）元素。）^

* * *

###### eq()
^除了所选元素中的索引号等于括号中内容的元素之外，eq方法会过滤掉所有其他元素；^
###### slice()
^slice()这个元素比较有意思，看headfirst差点把我误导了，slice（start，end），有这两个参数，除了索引介于括号中指定索引号之间的元素之外，slice方法会过滤掉所有其他元素；其实这段话是不严谨的^==slice方法过滤时，其实包含开始的下标的索引，比如slice（1,4），表示选择的是括号中选择器的索引值1到3的元素；那么又一个思考来了问题来了，如果slice（）只写了一个参数，那么如何处理，这时默认这个值是开始的下标索引值，他的结束选择在这个选择器的最后一个元素，后面我有demo介绍==
###### filter()
^除了与括号中指定选择器匹配的元素外，filter方法会过滤掉所有其他元素^
注意：filter方法也会遍历整个DOM结构，将满足条件的元素创建一个新的子集；
###### not()
^not()方法和filter方法选取元素的方法正好相反，not方法会过滤掉与括号中指定选择器匹配的所有元素；同样not方法也会遍历整个DOM结构，将满足条件的元素创建一个新的子集；^