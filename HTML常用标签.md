# 1.a 标签的用法 
html a标签是定义网页的超链接，是用在从一个页面往另一个页面的超链接.

>作用有:可跳转外部页面,内部锚点,邮箱与电话等.

## a 标签的属性
* href
* target
* download
* rel=noopener

属性href的取值
* 网址   
          https://.....  
          http://...   
          //google.com
* 路径   /a/b/c以及a/b/c
        index.html以及./index.html
* 伪协议 javascript:代码(或为空白);代码为空白页面不发生任何改变
        mailto:邮箱
        tel:手机号
* id
        href=#xxx
## target的取值
* _blank 跳转至新窗口
* _self 在当前页面打开
* _top 在当前的整个浏览器窗口中打开所链接的文档，因而会删除所有框架.
* _parent 将链接的文件载入含有该链接框架的父框架集或父窗口中。如果
含有该链接的框架不是嵌套的，则在浏览器全屏窗口中载入链接的文件.
# 2.img标签的用法
* 作用:发送get请求,展示一张图片
* 属性:alt/height/width/src/
* 事件:onload/onerror
* 响应式:max-width:100%;
* 可替换元素
  >转化官方的话来说意思为：一个 内容 不受CSS视觉格式化模型控制（关于视觉格式化模型控制的问题，视觉格式化模型中的各种框），CSS渲染模型并不考虑对此内容的渲染，且元素本身一般拥有固有尺寸（宽度，高度，宽高比）的元素，被称之为置换元素。即置换元素就是浏览器根据元素的标签和属性，来决定元素的具体显示内容。

  >如img|input|select|textarea|button|label等，他们被称为可置换元素（Replaced element）。他们区别一般inline元素（相对而言，称non-replaced element）是：这些元素拥有内在尺寸(intrinsic dimensions),他们可以设置width/height属性。他们的性质同设置了display:inline-block的元素一致。
  来自https://blog.csdn.net/Syleapn/article/details/79583598
  # table 标签的用法
  ## 1.table的标签
  * table
  * thead
  * tbody
  * tfoot
  * tr
  * th
  * td
    
    [写法html](/a-href.html)
  ## 2.相关的样式
  * table-layout:auto/fixed
  * border-collapse:collapse;
  * border-spacing:0;
 
# form标签
 > 作用:发送get或post请求，然后刷新页面
## 属性
* action 请求的哪个页面
* autocomplete 自动完成属性取值有"on/off","on"输入框内显示储存先前输入历史,"off"则不显示
* method get或post请求方式
* target 在当前页面提交，还是新开一个页面提交.

### Input的submit和button的submit有什么区别？
1. input标签内不能加入新的标签
2. button可以随意加入新的标签
### 注意:
> form表单必须带有type="submit"才能提交表单,不写则为默认,不管input或button的type="submit"  

> form里的Input都要有Name

# input标签
作用:让用户输入内容
## 属性
* button  
* checkbox  多选  
  【同一组类型的多选】：令多个input的name都是同一个字符串，这样浏览器提取值会自动归为同一数组
* radio  单选  
   【单选实现二选一效果】：令两个input的name都是同一个字符串，就能实现二选一效果.
* email
* file 若需要上传多个添加"multiple"
* color
* hidden
* search
* textarea 生成一个文本框,可是设置样式--style="resize:none;width:;height:;"
* select 选择 子标签为 option ：value
```
<select>
        <option value="">-請選擇-</option>
        <option value="1">週一</option>
        <option value="2">週二</option>
        <option value="3">週三</option>
</select>
```
## JS事件
onchange 当用户输入改变的时候触发   
onblur 当用户鼠标从对象移开时触发  
onfocus 当用户把鼠标集中在对象上时触发
