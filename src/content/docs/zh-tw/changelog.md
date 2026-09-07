---
title: "更新日誌"
---

## v1.16.23

### 新功能

- (`/search hsr`) 新增敵人分類。
- (`/challenge hsr`) 混沌回憶、虛構敘事及末日幻影卡片新增星啟模式。
- (`/challenge zzz`) 危局強襲戰卡片新增困難模式。
- (`/gacha-log import`) 絕區零的 HoYoLAB 帳號現可一鍵匯入抽卡紀錄，無需提供網址。
- (`/mimo`) 新增點數歷史紀錄檢視。
- (`/accounts`) 顯示所選帳號各項自動任務的狀態與最後執行時間。
- (`/profile zzz`) 新增 Sigrid 的卡片數據。

### 優化

- (`/search`) 拆分為 `/search genshin` 與 `/search hsr` 子指令，與 `/profile` 一致。
- (`/gacha-log import`) 匯入時僅獲取新紀錄，不再每次重新獲取完整歷史。
- (`/gacha-log view`) 自動更新常駐卡池物品清單，確保限定物品加入常駐池後 50/50 勝率統計仍然準確。
- (`/challenge hsr`) 即使未通關星啟關卡，也會顯示星啟隊伍。
- (`/challenge genshin stygian`) 恢復敵人弱點與強度資訊。
- (`/accompany`) 在角色檢視中顯示自動陪伴開關。
- (`/notes`) 移除崩壞：星穹鐵道的派遣欄位與派遣提醒，因遊戲中已不再有派遣功能。
- 自動任務的私訊通知若在排隊期間被關閉設定，將不再送出，並在每則通知中顯示動作發生的時間。
- 將最多 10 則自動任務通知合併為一則私訊，並捨棄超過 12 小時的成功通知。

### 問題修復

- (`/gacha-log view`) 修復絕區零 S 級角色在其自身 UP 卡池中抽出時被計算為 50/50 失敗的問題。

## v1.16.22

### 新功能

- (`/accompany`) 新增指令，可查看 HoYoLAB 角色陪伴的角色、設定你的陪伴角色並啟用自動簽到。
- (`/settings`) 新增與自動陪伴簽到功能相關的設定。
- (`/profile genshin`) 新增原神的 Enka 風格卡片。
- (`/profile hsr`) 新增崩壞：星穹鐵道新角色的卡片數據，包括姬子 SP。
- (`/profile zzz`) 新增絕區零 3.1 角色的卡片數據。
- (`/profile zzz`) 新增對 Lumiflux 屬性的支援。
- (`/card-settings`) 原神及崩壞：星穹鐵道的 Enka 風格卡片現可使用副詞條強化次數顯示開關。

### 優化

- (`/card-settings`) 重新設計圖片設定並將其併入卡片設定；`/profile` 中獨立的圖片設定按鈕已移除。
- (`/card-settings`) 所有模板皆可設定自訂圖片，當所選模板不支援時會顯示警告。
- (`/card-settings`) 官方立繪預覽現以實際的卡片圖片為準。
- (`/card-settings`) 移除自訂圖片的 Pixiv 支援，因其依賴的服務已無法使用。
- (`/profile genshin`) 移除 hattvr 模板；現有設定將遷移至 Enka 風格模板。
- 提升原神及崩壞：星穹鐵道指令中角色自動完成的速度與可靠性。

### 問題修復

- (`/profile`) 修復以參數傳入旅行者時未正確預選的問題。
- (`/profile zzz`) 修復音擎沒有副屬性時發生的錯誤。
- (`/profile zzz`) 修復 Velina 造型 ID 錯誤的問題。
- (`/card-settings`) 修復不同遊戲間角色 ID 衝突導致的崩潰問題。
- (`/card-settings`) 修復圖片選擇器未跳至目前圖片所在頁面的問題。
- (`/characters zzz`) 修復陣營篩選選項超過 25 個時的崩潰問題。
- (`/characters genshin`) 修復送出空白篩選選擇時發生的錯誤。
- (`/challenge`) 當目前期數沒有資料時顯示歷史紀錄。
- (`/challenge genshin`) 修復部分排名沒有資料時，深境螺旋傷害資訊區塊完全消失的問題。
- (`/events`) 修復活動獎勵稀有度未知時發生的錯誤。
- (`/search`) 修復測試版物品自動完成的錯誤。
- 修復說明文件連結開啟錯誤語言版本的問題。

## v1.16.21

### 新功能

- (`/profile hsr`) 新增崩壞：星穹鐵道 4.3 角色的卡片數據。
- (`/profile zzz`) 新增絕區零 3.0 角色的卡片數據。
- (`/profile`) 新增崩壞：星穹鐵道及絕區零的 Enka 風格卡片。
- (`/profile zzz`) 新增對風屬性的支援。
- (`/characters zzz`) 顯示音擎及技能等級。

### 優化

- (`/profile`) 透過快取縮放後的圖片來加快卡片生成速度。
- (`/characters`) 快取已生成的頁面以加快翻頁速度。
- (`/events`) 為不支援活動行事曆的遊戲顯示明確的功能不支援訊息。
- (`/notes`) 在手機推播通知中顯示提醒文字。

### 問題修復

- (`/challenge hsr`) 處理末日幻影、混沌回憶及虛構敘事中不完整的樓層資料，避免發生錯誤。
- (`/profile`) 修復原神傷害加成屬性錯誤地預設為風元素的問題。
- (`/profile`) 修復原神卡片因缺少屬性及服裝圖片數據而發生的錯誤。
- (`/profile zzz`) 修復絕區零 3.0 模板 2 角色的圖片位置。
- (`/card-settings`) 修復設定原神旅行者時發生的驗證錯誤。
- (`/search`) 修復開啟沒有數據的角色的語音或故事頁面時發生的錯誤。
- (`/redeem`) 改善兌換碼錯誤的處理。
- 修復停用通知後未生效、可能導致收到非預期的自動兌換私訊的問題。
- 當設定中未設定語言時，改用你的 Discord 客戶端語言。

## v1.16.20

### 新功能

- (`/profile zzz`) 新增絕區零 2.8 角色的卡片數據。
- (`/profile zzz`) 新增星見雅造型的卡片數據。

### 優化

- (`/profile hsr`) 優化角色卡片中的屬性顯示邏輯，包括歡愉傷害加成屬性。

### 問題修復

- (`/profile zzz`) 修復新絕區零角色缺少影畫圖片的問題。
- (`/profile`) 保留以參數傳入的角色順序。
- (`/gacha-log`) 為缺少的抽卡物品圖標顯示佔位圖片。

## v1.16.19

### 新功能

- (`/challenge hsr anomaly`) 現在將獲取最近三次的異相仲裁挑戰資料。
- (`/mimo`) 支援完成原神的看影片任務。
- (`/notes`) 新增打開雲·絕區零的按鈕。
- (`/profile hsr`) 顯示開拓者的命途，取代元素。

### 優化

- (`/profile`) 新增對新角色以及歡愉開拓者的支援。
- (`/challenge zzz shiyu`) 隱藏新卡片佈局中的通關時間文字。

### Bug Fixes

- (`/challenge hsr anomaly`) 修復空角色格的圖標位置。
- (`/profile zzz`) 修復愛芮及南宮羽圖片位置錯誤和沒有顯示服裝的問題。

## v1.16.18

### 新功能

- (`/profile`) 新增對絕區零 2.7 和崩壞：星穹鐵道 4.1 角色的支援。

### 問題修復

- (`/characters zzz`) 修復角色過多時的性能問題。
- (`/events hsr`) 修復異相仲裁在下拉選單中顯示錯誤名稱的問題。
- (`/card-settings`) 修復絕區零「無效查詢」錯誤的問題。
- (`/notes`) 修復在UI切換帳號時的錯誤問題。
- (`/search`) 修復在崩壞：星穹鐵道中搜索書籍時的錯誤。
- (`/profile zzz`) 修復愛芮的圖片在隊伍卡片中顯示不當的問題。
- (`/profile zzz`) 修復潘引壺造型缺少卡片數據的問題。

## v1.16.17a

### 優化

- 「你知道嗎？」提示訊息更新 - 2026年4月1日

## v1.16.17

### 新功能

- (`/profile hsr`) 新增對崩壞：星穹鐵道 4.0 新角色的支援，包括全新的歡愉命途。
- (`/challenge zzz shiyu`) 新增對式輿防衛戰 v2 的支援。
- (`/profile zzz`) 新增 ZZZ 2.6 角色的卡片資料。

### 問題修復

- (`/challenge zzz shiyu`) 修復卡片渲染問題，並處理獲取式輿防衛戰資料時的錯誤。
- (`/characters hsr`) 修復命途角色數量缺失時篩選器崩潰的問題。
- (`/events zzz`) 修復武器物件解析錯誤。
- (`/profile hsr`) 修復頂尖配置排名百分比格式錯誤的問題。
- (`/notes`) 修復崩壞3缺少體力提醒間隔的問題。
- 修復 zh-CN 及其他語言的本地化換行問題。

## v1.16.16

### 新功能

- (`/profile zzz`) 新增 ZZZ 2.5 角色卡片資料，包括簡·杜的服裝。
- (`/profile hsr`) 新增對歡愉命途類型的初步支持。
- (`/gacha-log`) 新增對 ZZZ 新卡池類型的支持（僅官方導入）。
- (`/build zzz`) 在攻略概覽中顯示攻略作者和最後更新日期。

### 優化

- (`/build zzz`) 改善了攻略章節的間距和可讀性。

### 問題修復

- (`/gacha-log upload`) 修復了 UIGF v4.1 導入無法正常工作的問題。
- (`/notes`) 允許將即時便籤通知時間設置為提前 0 小時（即恰好到時通知）。
- (`/mimo`) 禁用原神旅行 Mimo 的自動抽獎功能。
- (`/mimo`) 處理獲取原神旅行 Mimo 任務時的 -510001 錯誤。

## v1.16.15

### 新功能

- (`/build zzz`) 新增顯示絕區零角色面板的指令。
- (`/profile hsr`) 新增大理花的卡片資料。
- (`/mimo`) 重新啟用原神旅行 Mimo 支援。
- (`/mimo`) 新增對新的原神旅行 Mimo 任務類型的支援。
- 改善字體檢測以更好地處理阿拉伯語和其他非拉丁文字。

### 優化

- (`/profile hsr`) 改善大理花的卡片顏色。
- 實作零停機更新 - 機器人在程式碼更新期間不會再離線。

### 問題修復

- (`/profile genshin`) 修復轉換 HoYoLAB 原神角色時的 KeyError。
- (`/gacha-log view`) 修復崩壞:星穹鐵道和絕區零抽卡紀錄中缺少物品圖示的問題。
- (`/gacha-log view`) 修復小螢幕設備上的 UI 問題。
- 修復開關切換按鈕未正確返回 `False` 的問題。
- 修復多個內部部署和排程問題。

## v1.16.14

### 新功能

- (`/profile`) 新增對 ZZZ 新角色的支援。
- (`/exploration`) 新增新地區。
- (`/events`) 新增對 ZZZ 的支援。

### 優化

- (`/characters`) 預設依等級排序角色。
- (`/characters`) 為角色稀有度在卡片背景添加微光效果。
- (`/about`) 使用者連結改用 Discord 協定 URL。
- 新增假設定按鈕，引導使用者使用 `/settings`。

### 問題修復

- (`/challenge genshin`) 修復幽境危戰和幻想真境劇詩卡片的文字溢出問題。
- (`/challenge genshin theater`) 修復語言為越南語時秘奧挑戰不顯示的問題。
- (`/challenge hsr anomaly`) 修復賽季名稱文字溢出問題。
- (`/settings`) 修復無法為旅行 Mimo 設定選擇帳戶的問題。
- (`/settings`) 修復未定事件簿帳戶可以訪問提醒設定的問題。
- (`/profile hsr`) 修復面板卡片中行跡位置的問題。
- (`/profile hsr`) 修復特定角色缺少屬性圖示的問題。
- (`/search`, `/profile zzz`) 修復艾蓮、11 號等角色在自動完成中缺失的問題。
- (`/settings`) 修復點擊兌換通知開關時更改了錯誤設定的問題。
- (`/profile zzz`) 修復麗娜的圖片在隊伍卡片中未置中的問題。
- 將 UID 遮罩字元從「*」改為「x」以避免 Markdown 格式問題。

## v1.16.13

### 新功能

- (`/profile`) 新增對新 HSR 和 ZZZ 角色的支援。
- (`/challenge genshin theater`) 新增對月諭聖牌挑戰的支援。
- (`/profile hsr`) 新增 HoYoLAB/米遊社角色的光錐數據。
- (`/challenge hsr anomaly`) 新增對異相仲裁的支援。
- (`/profile genshin`) 新增對奇偶(男)和奇偶(女)的支援。
- (`/gacha-log`) 新增對千星奇域的支援。
- (`/settings`) 改版設定指令的 UI。

### 優化

- (`/gacha-log view`) 改善抽卡紀錄檢視器的效能。
- 改善自動簽到、自動兌換和自動旅行 Mimo 任務的效能。
- 改善機器人的整體效能。

### 問題修復

修復了多個問題，詳情請參閱[完整更新日誌](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.13)。

## v1.16.12

注意：此版本因原神旅行 Mimo 已從 HoYoLAB 移除而停用該功能。待功能重新上線後將再次啟用。

### 新功能

- (`/profile`) 新增對星穹鐵道與絕區零新角色的支援。
- (`/gacha-log import`) 使用我們[自己的腳本](https://github.com/studiobutter/gacha-stuff)來匯入抽卡紀錄。
- (`/challenge zzz shiyu`) 將最快通關時間替換為總通關時間。
- (`/challenge genshin stygian`) 新增敵人弱點與強度資訊。
- 新增對挪德卡萊地區的支援。

### 優化

- (`/profile`) 為 Enka Network API 請求新增更完善的錯誤處理。
- (`/profile`) 為 Enka Network 面板 API 請求新增錯誤處理。
- (`/profile`) 為第三方卡片生成 API 新增錯誤處理。
- (`/accounts`) 處理 Discord OAuth2 API 錯誤。
- (`/notes`) 為提醒設定模態中的不同輸入新增說明。
- 由於 Discord 的錯誤，WEBP 圖片無法複製,因此我們現在改以 PNG 格式發送資訊圖表。

### 問題修復

- (`/gacha-log view`) 修復自選祈願角色未被計算為 50/50 失敗的問題。
- (`/gacha-log view`) 修復部分絕區零物品稀有度錯誤的問題。
- (`/search`) 修復未釋出的絕區零角色有時出現在自動完成中的問題。
- (`/challenge zzz shiyu`) 處理沒有總通關時間的情況。
- (`/upload`) 修復圖片上傳問題。
- (`/challenge genshin stygian`) 修復部分敵人的文字超出邊界的問題。
- (`/challenge zzz assault`) 修復過往挑戰中存取邦布圖示的問題。
- (`/gacha-log view`) 處理無效的卡池類型輸入。
- (`/challenge`) 修復當關卡階段超過 25 個時,挑戰階段下拉選單出現問題的問題。

## v1.16.11

### 新功能

- (`/search`) 新增冰開拓者。
- (`/accounts`) 新增電子郵件登入的設備識別碼，讓你可以在 Hoyoverse 帳號中心查看 Hoyo Buddy 的設備。

### 問題修復

- (`/profile zzz`) 更新 enka.py 以符合新的 API 格式。
- (`/profile`) 修復 Enka 結果總是以英文返回結果的問題。
- (`/exploration`) 修復部落等級文字超出圖片邊界的問題。
- 修復 en-GB 語言環境的翻譯問題。

## v1.16.10

### 新功能

- (`/profile hsr`) 支援新角色：海瑟音與刻律德菈。
- (`/gacha-log upload`) 當帳號遊戲與匯入遊戲不同時顯示錯誤。

### 優化

- (`/gacha-log import`) 改善匯入效能。
- 快取經常使用的資料，如設定與卡片設定，以提升效能。
- 模糊 UID 的 5 位數字而非 3 位。

### 問題修復

- (`/profile zzz`) 修復隊伍卡片缺少服裝圖片的問題。
- (`/profile zzz`) 修復 Alice 夏日服裝資料缺失的問題。
- (`/profile zzz`) 修復服裝資料導致的錯誤。
- (`/profile zzz`) 修復 Enka Network 面板有時不顯示的問題。
- (`/search`) 修復一般搜尋自動完成中顯示未發布內容的問題。

## v1.16.9

### 新功能

- (`/profile zzz`) 新增對 Enka Network 的支援。
- (`/about`) 為指令新增更多連結。
- 新增 `/changelog`、`/invite` 和 `/help` 指令。
- 新增對簡體中文和西班牙語的文檔支援。
- 新增[狀態頁面](https://status.seria.moe/?category=Hoyo%20Buddy)以查看機器人狀態。

### 優化

- (`/settings`) 此指令現在會以臨時訊息回應。

### 問題修復

- (`/accounts`) 修復帳戶登入問題。
- (`/gacha-log manage`) 修復 ZZZ 匯出時物品稀有度錯誤的問題。
- (`/gacha-log view`) 修復 HSR 聯動卡池角色和光錐的物品名稱顯示為「???」的問題。
- (`/profile genshin`) 修復數據來源為 HoYoLAB 時不顯示玩家嵌入內容的問題。

## v1.16.8

### 新功能

- (`/challenge zzz shiyu`) 新增通關時間。
- (`/challenge hsr`) 隱藏快速通關。
- (`/challenge hsr`) 新增「顯示 UID」選項。
- (`/gacha-log`) 支援星穹鐵道聯動卡池。
- (`/profile zzz`) 新增對新角色的支援：Alice 和 Yuzuha。
- (`/profile zzz`) 新增對代理人服裝的支援。
- 機器人在程式碼更新期間不會再離線。

### 優化

- (`/profile hsr`) 改善樣式 2 的文字位置。
- (`/events`) 改善亮色模式的色彩對比度。
- (`/gacha-log view`) 當更改卡池類型時更改網頁應用程式連結。
- (`/search`) 星穹鐵道角色故事現在以更清晰的方式顯示。
- 透過更好的快取改善圖片生成效能。
- 儲存圖片為 webp 格式而非 png 以減少檔案大小。

### 錯誤修復

- (`/redeem`) 修復小寫兌換碼未計算為已兌換的問題。
- (`/characters genshin`) 修復文字位置問題。
- (`/characters genshin`) 修復某些角色圖片樣式不同的問題。
- (`/profile hsr`) 修復樣式 2 中光錐名稱的字體問題。

## v1.16.7

### 新功能

- 新增阿拉伯語支援。
- (`/challenge genshin`) 新增「幽境危戰」卡片生成。
- (`/profile zzz`) 為樣式 4 的「閃能自動累積」新增縮寫。

### 優化

- (`/accounts`) 擷取帳號時顯示一個頁面。
- (`/accounts`) 更新米遊社登入的 APK 檔案 URL。
- (`/accounts`) 新增用於新增米遊社帳號的 aaid 輸入欄位。
- 利用多個 CPU 核心加快圖片生成速度。
- 圖片中的文字位置更精確。

### 問題修復

- (`/profile zzz`) 修復儀玄在樣式 1 中的圖片位置。
- (`/profile zzz`) 修復樣式 4 中「穿透值」數值未被翻譯的問題。
- (`/search`) 停用深境螺旋分類。
- (`/search`) 修復驅動盤分類沒有自動完成選項的問題。

## v1.16.6

### 新功能

- (`/profile zzz`) 新增 ZZZ 2.0 新角色卡片資料。

- (`/profile zzz`) 新增對命破代理人和貫穿力數值的支援。

- (`/gacha-log import`) 處理 authkey 例外狀況。

- 新增可關閉的週年慶公告。

### 優化

- (`/profile zzz`) 移除背景代理人名稱中的空格。

### 問題修復

- (`/characters genshin`) 處理無屬性角色的問題。

- (`/challenge genshin theater`) 處理無效角色 ID 的問題。

## v1.16.5

### 新功能

- (`/profile hsr`) 新增 v3.3 新角色卡片資料。
- (`/profile hsr`) 新增對記憶命途角色使用 StarRailCard 卡片樣式的支援。
- (`/profile`) 處理 Enka Network API 請求逾時錯誤。
- (`/search`) 啟用「未釋出內容」搜尋分類。

### 問題修復

- (`/redeem`) 移除指令中的 'user' 參數。
- (`/mimo`) 移除 mimo 自動任務嵌入中的 UID 模糊處理。
- (`/upload`) 處理過大的圖片檔案。
- (`/search`) 修復角色和光錐屬性計算公式錯誤的問題。
- (`/accounts`) 修復當使用者擁有超過 25 個帳戶時「下一頁」選項無法正常運作的問題。

## v1.16.4

### 新功能

- (`/profile genshin`) 支援無元素旅行者。
- 新增印地語字體。

### 優化

- (`/profile`) 移除角色資料快取。
- 為抽卡紀錄篩選條件添加約束條件。

### 問題修復

- (`/events`) 修復無法找到卡池公告的問題。
- (`/challenge genshin theater`) 修復幻想真境劇詩資料不顯示的問題。
- (`/profile`) 修復與 Enka Network 面板的相容性問題。
- (`/mimo`) 修復米遊社用戶能夠訪問該指令的問題。
- (`/notes`) 進行即時便籤檢查時忽略遊戲維護錯誤。
- (`/lb view`) 移除崩壞3的成就排行榜。
- (`/farm reminder`) 修復物品名稱顯示為"..."的問題。

## v1.16.3

### 新功能

- (`/profile zzz`) 新增薇薇安和雨果的卡片資料。
- 新增葡萄牙語 (巴西) 翻譯。
- 新增日語翻譯。

### 優化

- (`/profile zzz`) 調整了部分角色的圖片位置。
- (`/profile zzz`) 改善了卡片模板的圖片層級。

### 問題修復

- (`/notes`) 修復了質變儀通知無法正常運作的問題。
- (`/gacha-log upload`) 修復了某些 ZZZ 匯入方法導致的錯誤物品稀有度。

## v1.16.2

### 新功能

- (`/profile hsr`) 新增遐蝶和那刻夏的卡片資料。

### 問題修復

- (`/profile zzz`) 修復波可娜的圖片在卡片樣式 2 中位置錯誤的問題。
- (`/build genshin`) 修復用戶應用中聖遺物位置表情符號顯示錯誤的問題。

## v1.16.1

### 新功能

- (`/gacha-log upload`) 新增對 [Starward 啟動器](https://github.com/Scighost/Starward) 的絕區零部份匯入抽卡紀錄的支援。
- (`/redeem`) 新增通知設定。
- (`/accounts`) 新增獲取 aaid 的說明，方便用戶新增米遊社帳號。
- 新增「隱藏 UI」按鈕，適用於按鈕數量較多的指令。

### 優化

- (`/search`) 移除「未釋出內容」分類，詳情請參見[這則訊息](https://discord.com/channels/1000727526194298910/1042428379120545873/1346411349999357973)。
- (`/characters`) 允許在篩選器中不選擇任何項目。
- 提升自動任務的性能。

### 問題修復

修復了多個問題，詳情請查閱[完整更新日誌](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.1)。

## v1.16.0  

[給技術宅們](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.0)  

### 新增功能  

- (`/profile`) 在卡片設置中新增模板預覽。  
- (`/profile`) 在卡片模板下拉選單中顯示自訂圖片的可用性。  
- (`/notes`) 將《星穹鐵道》開拓力上限提升至 300。  
- (`/notes`) 新增「打開遊戲」按鈕。  
- (`/search zzz`) 新增核心技能等級選擇器。  
- (`/gacha-log import`) 匯入祈願記錄時，對比輸入的 UID 與當前帳號的 UID。  
- 自動根據 Discord 客戶端的語言設置新用戶的語言。  

### 優化  

- (`/redeem`) 改進使用者體驗，修復兌換已兌換禮包碼時無回應的問題。  
- (`/gacha-log`) 設置帳號參數為必填，避免混淆。  
- 為「缺少權限」和「訊息被 AutoMod 阻擋」的錯誤提供更明確的提示。  
- 簡化帳號設置過程中的提示文字。  

### 問題修復  

修復了多個錯誤並進行了一些改進。  

## v1.15.7  

### 新增功能  

- (`/web-events`) 新增命令來查看正在進行中的網頁活動，並設置通知器以提醒您有新活動。  
- (`/notes`) 為《絕區零》（ZZZ）新增懸賞委託和 Ridu 每週點數通知器。  
- (`/about`) 新增更新日誌按鈕。  

### 優化  

- (`/gacha-log view`) 修復緩存問題，提升祈願記錄頁面的性能。  
- (`/about`) 移除最新 Git 變更的顯示。  
- (`/mimo`) 在自動購買時，將旅行夥伴 Mimo 商店物品按照價格從高到低排序。  
- 改進其他語言的本地化。

### 問題修復  

- (`/characters genshin`) 修復因無屬性旅行者導致的 `KeyError` 問題。  
- (`/characters genshin`) 修復神里綾華天賦等級顯示錯誤的問題。  
- (`/stats`) 修復 ZZZ 中「未找到記錄卡片」的錯誤。  
- (`/build genshin`) 修復「沒有可繪製的阻止列表」的錯誤。  
- (`/gacha-log view`) 修復錯誤的 50/50 勝率計算。  
- (`/gacha-log view`) 修復 Web 應用中的 422 驗證錯誤。  
- (`/gacha-log view`) 處理無效的大小輸入。  
- (`/gacha-log import`) 處理匯入祈願記錄時的無效卡池類型問題。  
- (`/gacha-log import`) 修復 UIGF 匯入功能。  
- (`/mimo`) 在發送通知前確認任務完成狀態。  
- (`/mimo`) 在完成任務之間新增休眠間隔以避免觸發限速。  
- (`/mimo`) 移除任務名稱中的 HTML 標籤。  
- (`/mimo`) 修復購買物品後的錯誤。  
- (`/profile`) 修復不同遊戲的卡片設置混合的問題。  
- (`/profile genshin`) 修復隊伍卡片中顯示多餘天賦的問題。  
- (`/profile genshin`) 修復與 Mavuika 相關的驗證錯誤。  
- (`/search`) 修復 W-engine 精煉選擇器未更新所選值的問題。  
- (`/notes`) 修復《崩壞3》中的驗證錯誤。  
- (`/challenge zzz assault`) 修復增益圖標未顯示的問題。  

## v1.15.6

### 新增功能

- (`/mimo`) 新增旅行 Mimo 對於原神的支持（活動在撰寫時已經結束）。
- (`/mimo`) 新增自動抽獎功能。
- (`/challenge zzz`) 新增對於「危局強襲戰」遊戲模式的支持。
- (`/profile hsr`) 新增卡片樣式 2。
- (`/notes`) 新增對於絕區零懸賞委託及麗都週記任務資訊的顯示。

## 優化

- (`/check-in`) 減少重複的簽到 API 請求。

## 問題修復

- (`/mimo`) 修復當沒有完成任何任務或獲取任何積分時仍發送通知的問題。
- (`/mimo`) 修復有價值物品判斷方式的問題。
- (`/mimo`) 處理 -510001 錯誤。
- (`/mimo`) 修復在星穹鐵道中，有價值物品被誤認為裝飾品的問題。
- (`/mimo`) 當達到上限時禁用抽獎按鈕。
- (`/challenge zzz`) 修復卡片中錯誤的邦布圖片。
- (`/events`) 修復螺旋深淵進度錯誤的問題。
- (`/gacha-log view`) 修復錯誤的「距離上一稀有度的抽取次數」。
- 修復靜態圖片文件夾創建邏輯。

## v1.15.5  

### 新增功能  

- (`/mimo`) 自動完成需要在帖子下留言的任務。  
- (`/mimo`) 自動完成需要關注主題的任務。  
- (`/mimo`) 新增抽獎功能。  
- (`/mimo`) 新增通知設置。  
- (`/profile zzz`) 新增圖片設置，允許在構建卡中使用「Mindscape 3」的美術圖。  
- (`/profile zzz`) 新增春政 (Harumasa) 和雅 (Miyabi) 卡片數據。  
- (`/search`) 在某些公會中隱藏「未釋出內容」分類。  

### 優化  

- (`/mimo`) 在某些任務中顯示任務進度。  
- (`/mimo`) 在通知中顯示已完成任務的名稱。  
- (`/mimo`) 提升自動任務執行性能。  
- (`/challenge zzz shiyu`) 更新卡片佈局。  
- (`/challenge zzz shiyu`) 避免重複抓取代理人數據。  
- 在錯誤嵌入的頁腳顯示 Discord 伺服器邀請鏈接。  
- 在錯誤情況下解除項目加載狀態。  
- 在切換按鈕上新增開/關標籤。  
- 改進代理 API 請求邏輯。  
- 改善自動任務的錯誤處理邏輯。  

### 問題修復  

- (`/mimo`) 在兌換 Mimo 獎勵禮品碼後新增休眠間隔。  
- (`/mimo`) 修復任務清單中遺漏的任務。  
- (`/mimo`) 修復留言任務未被完成的問題。  
- (`/mimo`) 修復當沒有完成任何任務時仍發送通知的問題。  
- (`/mimo`) 自動完成中僅顯示 HoYoLAB 賬號。  
- (`/mimo`) 修復自動任務中的 `QuerySetError` 問題。  
- (`/mimo`) 修復帖子留言未被刪除的問題。  
- (`/mimo`) 處理旅行夥伴 Mimo 不可用於某些遊戲的情況。  
- (`/profile zzz`) 修復副屬性高亮未顯示在卡片上的問題。  
- (`/profile zzz`) 修復代理人被誤認為已緩存的問題。  
- (`/characters zzz`) 修復代理人總數顯示錯誤的問題。  
- (`/gacha-log upload`) 修復 zzz.rng.moe 導入時的問題。  
- (`/redeem`) 修復 Miyoushe 賬號出現在賬號自動完成選項中的問題。  
- (`/build genshin`) 處理某些角色缺失使用率的情況。  
- (`/events`) 修復 HSR 未來卡池未顯示為「尚未釋出」的問題。  
- 適配新的 ZenlessData 鍵值。  
- 修復 Hakushin API 的相關問題。  
- 捕獲 `dm_user` 方法中的一般異常情況。  

## v1.15.4  

### 新增功能  

- (`/build genshin`) 顯示角色隊伍配置的相關信息。  
- (`/mimo`) 新增指令來管理旅行 Mimo。  

### 優化  

- (`/build genshin`) 改善卡片設計。  
- (`/notes`) 使用事件日曆 API 檢查位面分裂事件。  

### 問題修復  

- (`/build genshin`) 修復一些 UI 問題。  
- (`/events`) 修復導致指令無法使用的問題。  
- (`/gacha-log upload`) 修復使用 UIGF 數據時的 `ValidationError` 問題。  
- (`/gacha-log upload`) 修復 UIGF 版本低於 3.0 時的 `KeyError` 問題。  
- (`/search`) 修復重複的自動完成選項問題。  

## v1.15.3  

先前版本中的錯誤程式碼導致部分使用者在登入時看到「請求次數過多」錯誤，請參閱[本文](./too-many-requests.md) 以了解更多資訊。

### 新增功能  

- (`/profile zzz`) 新增選擇器，可選擇想要突出的副屬性。  
- (`/profile hsr`) 新增 Fugue 和 Sunday 卡片數據。  

### 優化  

- (`/redeem`) 使用禮品碼本身掩蓋兌換鏈接。  
- (`/challenge genshin theater`, `/challenge genshin abyss`) 在卡片中顯示旅行者的元素屬性。  
- (`/accounts`) 對「請求過多」錯誤顯示自定義錯誤信息。  

### 問題修復  

- 修復指令未被翻譯為其他語言的問題。  
- 修復超時的模態未正確關閉的問題。  
- 修復 API 重試邏輯與錯誤處理邏輯。  
- 修復某些指令的 `ValueError` 問題。  
- 修復模態超時時間過短的問題。  
- 處理 Web 服務器重定向端點的 `KeyError` 問題。  
- (`/profile`) 處理從 Enka Network API 獲取數據時的 `EnkaAPIError` 問題。  
- (`/profile`) 更優雅地處理 Enka Network API 網關超時錯誤。  
- (`/profile`) 修復生成 AI 圖像時的 `BadRequestError` 問題。  
- (`/upload`) 修復上傳圖片時的 `BadRequestError` 問題。  

## v1.15.2 及以下

先前版本的更新日誌寫在 [Discord 伺服器](https://link.seria.moe/hb-dc) 內的 #更新 頻道中。  
