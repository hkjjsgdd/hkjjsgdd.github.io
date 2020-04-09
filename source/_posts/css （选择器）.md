p{
   font-size:12px;
   color:red;
   font-weight:bold;
}

类选择器


1、英文圆点开头

2、其中类选器名称可以任意起名（但不要起中文噢）

使用方法：

第一步：使用合适的标签把要修饰的内容标记起来，如下：

<span>胆小如鼠</span>
第二步：使用class="类选择器名称"为标签设置一个类，如下：

<span class="stress">胆小如鼠</span>
第三步：设置类选器css样式，如下：

.stress{color:red;}/*类前面要加入一个英文圆点*/




ID选择器



#setGreen{
   color:green;
}

<span id="setGreen">公开课</span>


子选择器
.food>li{border:1px solid red;}   即大于符号>


后代选择器
.first  span{color:red;}


子选择器和后代选择器的区别就是   >作用于元素的第一代后，空格作用于元素的所有后代

通用选择器

通用选择器是功能最强大的选择器，它使用一个（*）号指定，
它的作用是匹配html中所有标签元素，如下使用下面代码使用html中任意标签元素字体颜色全部设置为红色：

（）{color:red;}