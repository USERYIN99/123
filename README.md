<!DOCTYPE html>
<html>
<head>
    <title>循环弹窗示例</title>
    <script type="text/javascript">
        function showPopup() {
            var userResponse = confirm("这两天如果吃过小龙坎的请点确定，没吃过请点取消");
            // 这里可以根据用户响应执行一些操作
            // ...

            // 使用 setTimeout 来调用 showPopup 函数，而不是无限循环
            setTimeout(showPopup, 100); // 这里的 100 毫秒可以根据需要调整
        }
    </script>
</head>
<body onload="showPopup();">
    <h1>循环弹窗网页</h1>
</body>
</html>
