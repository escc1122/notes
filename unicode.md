# String "中"

2進位   : 100111000101101

8進位   : 47055

10進位 ： 20013

16進位  ：4E2D

##unicode

java  : 

    String g ="中二病";
    char[] b = g.toCharArray();
    for (char c :b){
        StringBuilder unicode = new StringBuilder(Integer.toHexString(c));
        while(unicode.length() < 4){
            unicode.insert(0,0);
        }
        unicode.insert(0,"\\u");
        System.out.println(c+"===>"+Integer.toHexString(c)+"===>"+unicode+"===>"+(int)c);
    }

	
    int[] a = {20013,20108,30149};
    String aaa = new String (a,0,3);    //從0開始取3位
    System.out.println("=aaa==>"+aaa);
    //輸出
    中===>4e2d===>\u4e2d===>20013
    二===>4e8c===>\u4e8c===>20108
    病===>75c5===>\u75c5===>30149
    =aaa==>中二病

javascript  : 

	var g = '中';
	for (var i=0;i<g.length;i++){
		options.response.write(g.charCodeAt(i)+"======="+g.charAt(i)+"<br>");
	}
	//輸出    20013=======中
