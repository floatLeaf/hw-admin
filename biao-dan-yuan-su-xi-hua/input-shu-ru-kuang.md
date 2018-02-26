>常规表单输入框组， 默认display 属性是inline-block

```
<div class="form-input-wrap">
    <label class="input-lable"><span>*</span>商品名称</label>
    <div class="input-wrap text-only">  
        <input type="text" readonly="" name="" id="goods-name">
    </div>
</div>
```
	
>浮动表单输入框组，父元素。form-row用于清除浮动

```
<div class="form-row">
    <div class="form-input-wrap">
        <label class="input-lable"><span>*</span>通用名称</label>
        <div class="input-wrap">
            <input type="text" class="number" autocomplete="off">
            <div class="result-list hide"> </div>
        </div>
    </div>
    
    <div class="form-input-wrap">
        <label class="input-lable"><span>*</span>通用名称</label>
        <div class="input-wrap">
            <input type="text" class="number" autocomplete="off">
            <div class="result-list hide"> </div>
        </div>
    </div>
    
    <div class="form-input-wrap">
        <label class="input-lable"><span>*</span>通用名称</label>
        <div class="input-wrap">
            <input type="text" class="number" autocomplete="off">
    	<div class="result-list hide"> </div>
        </div>
    </div>
</div>
```