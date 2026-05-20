# 📚 BookListView 圖書管理程式

## 功能說明

### 1. 書籍清單顯示
啟動程式後，ListView 會自動載入以下 8 本書籍資料，每筆包含書名、作者、類別三個欄位：

| 書名 | 作者 | 類別 |
|------|------|------|
| 三國演義 | 羅貫中 | 章回小說 |
| 西遊記 | 吳承恩 | 章回小說 |
| 唐詩三百首 | 孫洙 | 詩選 |
| 楚辭 | 劉向 | 詩歌 |
| 西廂記 | 王實甫 | 戲曲 |
| 水滸傳 | 施耐庵 | 章回小說 |
| 紅樓夢 | 曹雪芹 | 章回小說 |
| 牡丹亭 | 湯顯祖 | 戲曲 |

---

### 2. 切換檢視方式
右上角下拉選單 `cmbView` 可切換 ListView 的顯示模式：

| 選項 | 對應 View 模式 |
|------|----------------|
| 大圖示 | `LargeIcon` |
| 詳細資料 | `Details` |
| 小圖示 | `SmallIcon` |
| 清單 | `List` |
| 大圖示加詳細資料 | `Tile` |

<img width="537" height="332" alt="image" src="https://github.com/user-attachments/assets/4d320894-701c-4d27-9ba5-4464f73f046e" />
<img width="536" height="332" alt="image" src="https://github.com/user-attachments/assets/ff9932c2-ecae-4a11-8014-5bf001851bac" />
<img width="533" height="334" alt="image" src="https://github.com/user-attachments/assets/77ff9e02-3bc8-4877-bc1a-d6e9c2f459bd" />
<img width="535" height="331" alt="image" src="https://github.com/user-attachments/assets/5d7cfd5b-046b-4866-9d9d-2d0b4bc77b4b" />
<img width="535" height="332" alt="image" src="https://github.com/user-attachments/assets/3331c96b-5513-4484-99b5-1730c91452b5" />

---

### 3. 借書功能
雙擊 ListView 中的書籍項目，會彈出確認訊息方塊：

- 按下 **是(Y)**：將該書加入右側借書清單
- 按下 **否(N)**：取消，不做任何動作
- 若書籍**已在借書清單中**，則不會再次彈出訊息

<img width="533" height="330" alt="image" src="https://github.com/user-attachments/assets/86231181-69dd-4273-9239-02a52c70ebda" />

<img width="535" height="331" alt="image" src="https://github.com/user-attachments/assets/173fe014-46ea-4104-b25a-6a7c1c55510e" />


---

## 介面配置

| 控制項 | 名稱 | 說明 |
|--------|------|------|
| ListView | `lvwBooks` | 顯示書籍清單，支援多種檢視模式 |
| ComboBox | `cmbView` | 切換 ListView 的檢視方式 |
| ListBox | `lstBorrow` | 顯示已借書籍清單 |
| ImageList | `imgL` | 大圖示影像來源（90×120） |
| ImageList | `imgS` | 小圖示影像來源（15×20） |
| GroupBox | `grpView` | 包覆檢視方式選單 |
| GroupBox | `grpBorrow` | 包覆借書清單 |
| Panel | `pnlTools` | 右側工具面板容器 |

---
