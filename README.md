<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>IFE JavaScript Task 01</title>
</head>
<body>

<label>请输入北京今天空气质量：<input id="aqi-input" type="text"></label>
<button id="button">确认填写</button>

<div>您输入的值是：<span id="aqi-display">尚无录入</span></div>

<script type="text/javascript">
//参考以下示例代码，补充其中的JavaScript功能，完成一个JavaScript代码的编写
//本任务完成的功能为：用户可以在输入框中输入任何内容，点击“确认填写”按钮后，用户输入的内容会显示在“您输入的值是”文字的右边
    (function() {
        /*
         在注释下方写下代码
         给按钮button绑定一个点击事件
         在事件处理函数中
         获取aqi-input输入的值，并显示在aqi-display中
         */
        var btn = document.getElementById("button");
        btn.onclick = function(){
            //addEventListener与on的区别是：on只触发一次事件，前边同样的事件（如click）会被覆盖掉，addEventListener不会，
            // 还有一个对应的移除事件removeEventListener
            document.getElementById("aqi-display").innerText = document.getElementById("aqi-input").value;
        }
    })();

</script>
</body>
</html>
