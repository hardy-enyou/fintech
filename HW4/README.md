# 作業4
- 到telegram搜尋botfather

- /newbot 取名 取id

- 建立新的lambda函式 
- 執行時間選python3.7
- 上傳助教給的檔案(aws-educate-chatbox.zip)
- 執行時間設定編輯(前面改成main)
- 建立layer
- 上傳python.zip 執行時間選全部的python
- 回到lambda下面的layer選自訂上船建立的layer
- 新增觸發 選api gateway 類型選rest 安全性開啟
- 點進創好的api gateway後 整合請求
- 關掉lambda代理整合
- 操作 部屬api 第一個選default
- 回到lambda的程式碼 打開config
- 複製telegram的token碼到telegram token
- 複製api 終端節點的網址到webhook url
- eploy
- 到processor
- 複製code碼(助教給的)到下面的run data
- deploy
- 去看自己的api碼(助教的api link)
- 跟自己創的chatbox說話後重整api
- 參照助教給的test case data把(上一部的api給找到後複製到lambda的test下面的
程式碼)
- 按test
- 如果出錯那要到processor.py的29行把引號改對之後reploy在test
- 回到api gateway 資源 any 測試
- 方法選post  請求內文放上面括號中的程式碼
- [HW4影片連結](https://youtu.be/cVs-RodPZ4U)


