# verificationCodes
行为验证码


1.关于验证码
   a,首先要先引入jquery，基于jq开发   http://code.jquery.com/jquery-1.8.0.min.js
   b,使用 ：
            初始化：1，添加到dom中  2，成功后：onSuccess  3,onError  (具备参数，可选) 
   
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












        