<iframe width="100%" height="300" src="//jsrun.net/4FqKp/embedded/all/light/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

>所有的搜索条件包裹在类名为table-search-wrap的div中

####单个input框

![](http://jc519.oss-cn-beijing.aliyuncs.com/642a2152d763952be7132f4ce77f2b53.jpg)
···
<div class="content-group">
    <label class="input-lable">联系人</label>
    <div class="input-wrap">
        <input class="x-input" type="text" name="actualName" value="" placeholder="请输入联系人">
    </div>  
</div> 
···

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
``