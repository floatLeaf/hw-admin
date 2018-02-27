<iframe width="100%" height="300" src="//jsrun.net/4FqKp/embedded/all/light/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

>所有的搜索条件包裹在类名为table-search-wrap的div中

####单个input框

![](http://jc519.oss-cn-beijing.aliyuncs.com/642a2152d763952be7132f4ce77f2b53.jpg)
```
<div class="content-group">
    <label class="input-lable">联系人</label>
    <div class="input-wrap">
        <input class="x-input" type="text" name="actualName" value="" placeholder="请输入联系人">
    </div>  
</div> 
```


####单个select框

![](http://jc519.oss-cn-beijing.aliyuncs.com/ba265fe72e45a6beaeaef652a2d3ecc6.png)
```
<div class="content-group select">
    <label class="input-lable">地区</label>
    <div class="input-wrap "> 
    <input type="text" name="batchNumber" readonly required="" placeholder="请选择生产批号">

    <div class="select-down-lists">
        <div class="list" data-value="select-1">select-1</div>
        <div class="list" data-value="select-2">select-2</div>
        <div class="list">select-3</div>
        <div class="list">select-4</div>
        <div class="list">select-5</div> 
        <div class="list">select-6</div>
        <div class="list">select-6</div>
        <div class="list">select-6</div>
    </div>
</div>
```

####常规搜索 一行展示三个input
```
<div class="table-search-wrap">
    <h1 class="search-title"><i class="iconfont"></i>筛选查询<i class="iconfont arrow"></i></h1>
    <div class="content">
        <div class="form-row">
            <!--搜索的input框-->
        </div>
    </div>
</div>
```