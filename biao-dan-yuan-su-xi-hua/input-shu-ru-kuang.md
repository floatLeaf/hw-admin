>常规表单输入框组， 默认display 属性是inline-block

```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">  
        <input type="text" readonly="" name="" id="goods-name">
    </div>
</div>
```
	
>浮动表单输入框组，父元素。form-row用于清除浮动, (每行最多三个)

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


>只能输入数字的input, 为input添加number 类名

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

>只读input 

```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">  
        <span class="text">阿莫西西</span>
        <input type="hidden" readonly="" name="" id="goods-name">
    </div>
</div>
```	

