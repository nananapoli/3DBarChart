# 3DBarChart
an animated 3d bar chart which have several option to change its shape and color

功能：改变方块的长度，颜色以及内容块的百分比

选择器的运用 + 元素结构
        1.利用伪类选择器（即透明的input标签的checked）配合input和label来改变状态，
        2.以相邻选择器改变紧邻着的label标签的样式，
        3.以兄弟选择器和伪类选择器（nth-child)选中3D bar（ul标签内的li标签）进行样式改变，用到了transition

利用伪元素呈现立体效果
      key:一个div里放两个div作为前后两个面，子div里利用before和after两个伪元素制造两个面，经过transform和移动到达指定位置，呈现立体效果

响应式布局
       简单地改变字体的大小
兼容性
一些css3属性需要注意，transition，transform，liner


Tips:
  ● label标签和input控件配合使用，lable的for属性的值应该是对应的控件的id,这样，点击label标签便会触发控件
  ● 可以利用伪元素来做补丁，遮挡不想被看到的部分
