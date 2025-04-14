# LINE-message-API

# LINE 群組定時自動訊息通知設定指南：
1. 前往 LINE Developer Console，建立一個 Provider，並記下你設定的 Provider 名稱：
   https://developers.line.biz/zh-hant/services/messaging-api/
2. 選擇"Create a Messaging API channel"，點擊"Create a LINE Official Account"，經過以下3個步驟：<br/>
   【登錄公司／店鋪資訊】填寫帳號資訊：帳號名稱、電子郵件帳號、公司所在國家或地區、業種，點擊下方"確定"<br/>
   【確認輸入內容】點擊"完成"<br/>
   【申請完成】<br/>
3. 申請完成後出現"您的LINE官方帳號已建立完成"頁面
4. 記住"帳號資訊"的基本ID: @999xxxx(舉例) 
5. 點擊"稍後進行認證(前往管理畫面)"
6. 同意我們使用您的資訊，點選"同意"
7. LINE官方帳號使用條款更新啟事，點選"了解並繼續使用"
8. 頁面會自動轉到 LINE Official Account Manager
   8.1 若尚未擁有帳號，登入 LINE 官方帳號管理後台，可免費註冊一個：https://tw.linebiz.com/login/ )
   8.2 成功登入後，建立新的 LINE 官方帳號。請注意：帳號名稱在修改後的 7 天內無法再次變更。
   8.3 建立LINE官方帳號：此名稱將顯示於LINE的好友名單及聊天畫面中，填寫基本訊息(EMAIL等)。
   8.4 上述基本訊息填寫完之後會出現 "您的LINE官方帳號已建立完成"，暫不選擇"申請認證帳號"，直接選擇"稍後進行認證(前往管理畫面)"，記憶住"帳號資訊"的基本ID: @999xxxx(舉例) 。
   8.5 依序點選"同意"、"了解並繼續使用"、"下一步"，點選"下一步"之後，直接點選"前往主頁"(暫不點選"增加好友人數")。
9. 彈窗：開始經營帳號前(1/2)，點擊右上角的 "X"
8. 點擊該頁面右上角"設定"，點擊之後：<br/>
    (1) 點擊左側選單的 設定 > 帳號設定 > 功能設定 > "接受邀請加入群組或多人聊天" (點擊變更)。<br/>
    (2) 點擊左側選單的 設定 > 回應設定 > 回應功能 > "加入好友的歡迎訊息" (取消選取)。<br/>
    (3) 點擊左側選單的 設定 > 回應設定 > 回應功能 > "自動回應訊息" (取消選取)。<br/>
    (4) 點擊左側選單的 設定 > 回應設定 > 回應功能 > Webhook > (下方綠色小字)"開啟Messaging API的設定畫面" (點擊綠色小字後跳頁)。<br/>
9. LINE Official Account Manager - Messaging API：<br/>
    (1) 點選"啟用Messaging API"<br/>
    (2) 選擇服務提供者：選擇上述 1 在 LINE Developer Console 所建立的 Provider 名稱，點選同意<br/>
    (3) 暫不填寫 "隱私權政策"、"服務條款" (選填，可以不填寫)，直接點選確定<br/>
    (4) 最終會出現 [啟用Messaging API] ，直接點選確定<br/>
================================================================================
================================================================================
10. 登入 Google 雲端硬碟的 JavaScript Apps Script 平台 (Google Apps Script)
    https://script.google.com/home?hl=zh-tw
11. 成功登入後，點擊左上角" + 新專案"
12. 先將"程式嗎.gs"檔案的右側 Code Window 中的默認程式碼： function myFunction() {} 刪除
13. 再將 GitHub Code (例如：punch out) 複製黏貼到"程式嗎.gs"檔案的右側 Code Window
14. 點擊儲存：將專案儲存至雲端硬碟
15. 點擊執行，會出現"需要授權"
16. 依序點擊以下：
    審查授權 >
    選擇帳戶 >
    出現紅色三角警語 (這個應用程式未經Google驗證) >
    點擊警語下方左側的 "進階" >
    點擊 "前往「未命名的專案」(不安全)" >
    選取要讓「未命名的專案」存取的範圍，選擇"全選" > 

13. 點擊左側選單的"專案設定"，在"一般設定"的時區選擇"台北標準時間-台北(GMT+08:00)"
14. 點擊左側選單的"編輯器"
15. 先將"程式嗎.gs"檔案的右側 Code Window 中的默認程式碼： function myFunction() {} 刪除
16. 再將 GitHub Code (punch out) 複製黏貼到"程式嗎.gs"檔案的右側 Code Window
17. 修改 GitHub Code 中的
    (1) line_token、token：改成
    (2) userId (先不改)
    (3) 其他：例如 訊息(message)、時間 (days[]、atHour()、nearMinute())
   
   
