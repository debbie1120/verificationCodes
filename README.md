
##关于验证码

* 首先要先引入jquery，基于jq开发   http://code.jquery.com/jquery-1.8.0.min.js

* 使用 ：初始化
    * 添加到dom中
    * 成功后：onSuccess 
    * onError  (具备参数，可选) 



```javascript
   verificationCode.init({
            el:$('.code'),
                onSuccess: function () {
                document.getElementById('msg').innerHTML = '验证成功！'
            },
            onError: function (isError) {
                if(isError){
                    document.getElementById('msg').innerHTML = '验证失败'
                }else{
                     document.getElementById('msg').innerHTML = ''
                }
              
            }
        });
```

![image](https://github.com/debbie1120/verificationCodes/blob/c960df5caa18faf4ee9036bbf1c9f6b2732f1457/微信图片_20180706145727_看图王.png)

![image](https://github.com/debbie1120/verificationCodes/blob/c960df5caa18faf4ee9036bbf1c9f6b2732f1457/微信图片_20180706145723_看图王.png)







        
