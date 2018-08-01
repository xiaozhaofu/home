```
<dt>QQ技术咨询</dt>
<dd>
    <span id="tecQQ">
        <a href="http://wpa.qq.com/msgrd?v=3&uin=3268338747&site=qq&menu=no"          target="_blank">3268338747
        </a>
    </span>
</dd>


<dt>售后服务电话</dt>
<dd>
    <span id="saled">
        <a href="javascript:;">400-6688-779</a>
    </span> 
</dd>

```
###### 默认为pc端执行程序,经过下边js判断,如果为移动端,则按移动端执行程序
```
<script type="text/javascript">
    //    判断pc端和手机端
    function browserRedirect() {
        var sUserAgent = navigator.userAgent.toLowerCase();
        var bIsIpad = sUserAgent.match(/ipad/i) == "ipad";
        var bIsIphoneOs = sUserAgent.match(/iphone os/i) == "iphone os";
        var bIsMidp = sUserAgent.match(/midp/i) == "midp";
        var bIsUc7 = sUserAgent.match(/rv:1.2.3.4/i) == "rv:1.2.3.4";
        var bIsUc = sUserAgent.match(/ucweb/i) == "ucweb";
        var bIsAndroid = sUserAgent.match(/android/i) == "android";
        var bIsCE = sUserAgent.match(/windows ce/i) == "windows ce";
        var bIsWM = sUserAgent.match(/windows mobile/i) == "windows mobile";

        if (bIsIpad || bIsIphoneOs || bIsMidp || bIsUc7 || bIsUc || bIsAndroid || bIsCE || bIsWM) {
            //电话
            $('#saled a').attr('href','tel:400-6688-779') ;
            // QQ技术咨询
            $('#tecQQ a').attr('href','mqqwpa://im/chat?chat_type=wpa&uin=3268338747&version=1&src_type=web&web_src=oicqzone.com') ;
            
        }
    }

    browserRedirect();
</script>
```