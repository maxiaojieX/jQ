
# jQ使用储备库

<hr>
<br>
<h3>文本域textarea限制行数</h2>
以下代码只替换textarea id 和 行数即可。

```jqery
$("#your textarea id").on('input',function(e){
            <!--限制的行数-->
            var len = 20;
            var tx = $("#orderIdTx").val();
            var mycars=new Array();
            mycars = tx.split("\n");
            if(mycars.length>len) {
                var test = "";
                for(var i=0;i<len;i++){
                    if(i < len-1) {
                        var te  = mycars[i]+"\n";
                        test +=te;
                    }else {
                        test += mycars[i];
                    }
                }
                $("#your textarea id").val(test)
            }
        });
```



