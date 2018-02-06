###基于恒宇方舟项目后台风格

#####注意事项
1. 所有的页面布局代码统一包在类名为.x-main-content的元素中， 做统一的宽度样式限制
```
<!DOCTYPE html>
<html>
<head>
     <title></title>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <link rel="stylesheet" type="text/css" href="/static/Admin/css/Index/testAdd.css">
     <!--[if lt IE 9]>
     <script src="/static/lib/respond.min.js" type="text/javascript"></script>
     <script src="/static/lib/html5shiv.min.js" type="text/javascript"></script>
     <script src="/static/lib/selectivizr.min.js" type="text/javascript"></script>
     <![endif]-->
 </head>
 <body>
    <div class="x-main-content">
        ...
    </div>
 </body>
 <script type="text/javascript" src="/static/Admin/js/vendor.js"></script>
 <script type="text/javascript" src="/static/Admin/js/Index/testAdd.js"></script> 
</html>
```




