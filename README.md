# snoopy
snoopy php class

`GET`

 $snoopy = new \Snoopy\Snoopy();  
 $snoopy->fetch($url); //获取所有内容  
 echo $snoopy->results; //显示结果  
 //可选以下  
 $snoopy->fetchtext //获取文本内容（去掉html代码）  
 $snoopy->fetchlinks //获取链接  
 $snoopy->fetchform  //获取表单

`POST`

$snoopy = new \Snoopy\Snoopy();  
$data["username"] = "admin";  
$data["pwd"] = "admin";  
$snoopy->submit($url,$data);//$data为提交的数组  
echo $snoopy->results; //获取表单提交后的 返回的结果 