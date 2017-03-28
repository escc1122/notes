# String "中"

2進位   : 100111000101101

8進位   : 47055

10進位 ： 20013

16進位  ：4E2D

##unicode

java  : \u4e2d

String g ="中";
char[] b = g.toCharArray();
for (char c :b){
	System.out.println(c+"===>"+Integer.toHexString(c));
}

//輸出    中===>4e2d



javascript  : \u4e2d

var g = '中';
for (var i=0;i<g.length;i++){
	options.response.write(username.charCodeAt(i)+"======="+username.charAt(i)+"<br>");
}
//輸出    20013=======中
