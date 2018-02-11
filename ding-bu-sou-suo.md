####列表顶部搜索

>常规form
```
<div class="table-search-wrap">
    <h1 class="search-title"><i class="iconfont"></i>筛选查询<i class="iconfont arrow"></i></h1>
    <div class="content width-btn">   
        <div class="form-row">
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
	                            <div class="list">select-6</div>
	                        </div>
	                    </div> 
            </div> 

            <div class="content-group">
                <label class="input-lable">联系人</label>
                <div class="input-wrap">
                    <input class="x-input" type="text" name="actualName" value="" placeholder="请输入联系人">
                </div>  
            </div>  

            <div class="content-group">
                <label class="input-lable">医药公司</label>
                <div class="input-wrap">
                    <input class="x-input" type="text" name="companyName" value="" placeholder="请输入医药公司">
                </div>  
            </div>  

            <input type="hidden" value="" id="channel-type" name="roleId">
            <input type="hidden" value="" id="approval-type" name="auditStatus">
            <button class="x-btn-yellow" type="submit">查询</button> 

        </div>
    </div> 
</div>
```

<iframe width="100%" height="700" src="//jsrun.net/qJqKp/embedded/all/light/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>