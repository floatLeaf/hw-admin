####常规表单输入框组， 默认display 属性是inline-block

![](http://jc519.oss-cn-beijing.aliyuncs.com/060b4c946e47256221fc857bec78d9e7.jpg)
```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">  
        <input type="text" readonly="" name="" id="goods-name">
    </div>
</div>
``` 
	
####浮动表单输入框组，父元素。form-row用于清除浮动, (每行最多三个)

![](http://jc519.oss-cn-beijing.aliyuncs.com/2c69acb0dca0b5f0c7b0ff4a9a30fce5.jpg)

```
<div class="form-row">
    <div class="form-input-wrap">
        <label class="input-lable"><span>*</span>通用名称</label>
        <div class="input-wrap">
            <input type="text" class="number">
        </div>
    </div>
    
    <div class="form-input-wrap">
        <label class="input-lable"><span>*</span>通用名称</label>
        <div class="input-wrap">
            <input type="text" class="number">
            <div class="result-list hide"> </div>
        </div>
    </div>
</div>
```



####只能输入数字的input, 为input添加number 类名

```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">  
        <input type="text" readonly="" name="" id="goods-name">
    </div>
</div>

<script type="text/javascript">
    var elem = $('input.number'),
        preNum = 0;
    elem.on('input propertychange', function() {
      preNum = $(this).data('pre') || '';
      var num = $(this).val();
      
      if (!/^(?:|[1-9]{1,}\d*)$/.test(num)) {
        $(this).val(preNum);
      } else {
        $(this).data('pre', num);
      }  
    });
    
    elem.on('change', function() {
      if ($(this).val() === '') {
        $(this).val(0);
      }
    });
</script>
```
####带单位input
![](http://jc519.oss-cn-beijing.aliyuncs.com/003a6c4fddf865cb90ecdb9cc794d0c7.jpg)

```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>入库数量</label>
    <div class="input-wrap text-icon">
        <input type="number" min="0" required="" name="number" id="number">
        <span class="unit">盒</span>
    </div>
</div>
```


####只读input 

![](http://jc519.oss-cn-beijing.aliyuncs.com/a4f580d8717c07c09aebafd5c2617dfe.jpg)
```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">   
        <input type="text" readonly name="" id="goods-name" value="阿拉蕾">
    </div>
</div>

<!-- 纯文字展示 -->
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">   
        <span class="text">阿拉蕾</span>
    </div>
</div>

```	

####带单位只读的input

![](http://jc519.oss-cn-beijing.aliyuncs.com/feda3d1cd900befaad0c82168d826521.jpg)
```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>有效期</label>
    <div class="input-wrap text-icon text-only ">
        <input type="text" readonly name="" id="goods-name" value="12"> 
        <span class="unit">个月</span>
    </div>
</div>
```
