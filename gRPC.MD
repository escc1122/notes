評估報告:

結論:可以導入，但現在不是時機。

目前gRPC-Web尚未成熟，官方證實屬於實驗階段，不管是後續的維護&穩定度都是未知，
若導入實驗性階段的技術，勢必未來要肯定會更新頻繁，如果導入已上線的遊戲，
風險會比較大，客戶體驗品質無法保證。


我們將分成三大部分來討論，報告內容如下:

一.成熟度(穩定性)
  1. gRPC-Web 不支援http2。
  2. gRPC-Web 不支援proto直接使用。
  3. gRPC-Web TypeScript為實驗性質。
  4. gRPC-Web 屬於實驗性質。
  5. gRPC-Web 直連實驗性質。
  6. 目前瀏覽器不支援gRPC(注1)。
  7. gRPC 不等於gRPC-Web，故需要透過gRPC-Web來實現。
  8. 無法從原生瀏覽器上直接Debug，需要透過第三方插件。
  9. 白鷺第三方套件支援程度(注2)。

二.安全性
	1.XSRF(跨站請求偽造)、XSS(跨網站指令碼) 官方待發佈
	
三.性能上
	1.gRPC-Web建立在上htpp1上，不支援http2



注
1. https://docs.microsoft.com/en-us/aspnet/core/grpc/browser?view=aspnetcore-6.0
2. https://kknews.cc/zh-tw/news/22zyamy.html
3. https://github.com/grpc/grpc-web/blob/master/doc/browser-features.md

參考文獻:
* https://github.com/grpc/grpc-web
* https://docs.microsoft.com/en-us/aspnet/core/grpc/comparison?view=aspnetcore-6.0
