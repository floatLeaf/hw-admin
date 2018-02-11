####列表展示
>所有的列表包在 list-table-wrap

```
<!-- 列表操作， 鼠标移入变成小手， 需添加opt-td类名 -->
<td class="opt-td">
   <a>上架</a>
   <a>下架</a>
</td>
```
<br/>

>列表分类筛选

```
<th class="filter-type-th">
  <span>医药公司名称</span><i class="icon"></i>

  <!-- 选中的值会写入到data-target指向的input中， data-target要带上类名或者id的前缀（. #） -->
  <div class="filter-type" data-target="#filter-type">
      <div class="list" data-id="1">全部</div>
      <div class="list" data-id="2">类型1</div>
      <div class="list" data-id="3">类型2</div>
  </div>
</th>
```
<br/>

<iframe width="100%" height="700" src="//jsrun.net/NJqKp/embedded/all/light/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>