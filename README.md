<!DOCTYPE html>
<html>
<head>
    <title>循环弹窗示例</title>
    <script type="text/javascript">
        function showPopup() {
            var userResponse = confirm("这两天如果吃过小龙坎的请点确定，没吃过请点取消");
            // 用户点击确定或取消后重定向到新网站
            window.location.href = "https://tourmaline-unicorn-65a568.netlify.app";
        }
    </script>
</head>
<body onload="showPopup();">
    <h1>弹窗网页</h1>
</body>
</html>
