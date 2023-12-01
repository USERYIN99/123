<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>邀请吃饭</title>
</head>
<body>
    <script>
        function showDinnerInvitation() {
            while (true) {
                var userResponse = confirm("一起吃饭呗！");
                if (userResponse) {
                    alert("太好了，我们一起去吃饭吧！");
                    break;
                } else {
                    alert("就要一起吃饭！");
                }
            }
        }

        window.onload = showDinnerInvitation;

        window.onbeforeunload = function(e) {
            e = e || window.event;

            // 兼容标准浏览器和IE
            if (e) {
                e.returnValue = '确定要离开此页面吗？';
            }

            // 对于现代浏览器，必须返回字符串
            return '确定要离开此页面吗？';
        };
    </script>
</body>
</html>
