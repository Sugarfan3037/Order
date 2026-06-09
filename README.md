# 🍔 Java Swing 餐飲點餐管理系統

## 📖 專案簡介

本專案為使用 **Java Swing** 搭配 **Eclipse WindowBuilder** 開發之桌面式點餐系統。

系統模擬早餐店或飲料店的實際點餐流程，提供商品選購、數量調整、會員折扣、訂單明細顯示、收據列印及即時時間顯示等功能。

透過本專案實踐：

- Java GUI設計
- 事件驅動程式設計(Event Driven Programming)
- 物件導向程式設計(OOP)
- Swing元件操作
- 訂單管理邏輯設計

---

# 🎯 專案目標

建立一套簡易且完整的餐飲點餐系統，使使用者能夠：

1. 選擇商品
2. 調整數量
3. 即時查看訂單內容
4. 使用會員優惠
5. 計算最終金額
6. 列印收據

---

# 🖥 系統畫面

## 主畫面

建議將專案截圖放置於：

```text
images/mainUI.png
```

```markdown
![系統主畫面](images/mainUI.png)
```

---

# ✨ 系統功能

## 飲料類

| 商品 | 單價 |
|------|------|
| 紅茶 | NT$20 |
| 綠茶 | NT$20 |
| 奶茶 | NT$30 |

## 餐點類

| 商品 | 單價 |
|------|------|
| 漢堡 | NT$60 |
| 薯條 | NT$50 |
| 雞塊 | NT$50 |
| 總匯三明治 | NT$80 |

## 商品數量控制

透過「+」與「-」按鈕調整商品數量。

特色：

- 數量不可低於0
- 即時更新畫面
- 自動刷新訂單明細

## 即時訂單明細

當商品數量變更時，系統會自動更新訂單內容。

範例：

```text
紅茶 x2 = 40元
奶茶 x1 = 30元
漢堡 x1 = 60元
```

## 會員折扣功能

會員可享有九折優惠。

```java
if(member.isSelected())
{
    finalPrice = total * 0.9;
}
```

## 結帳功能

流程：

```text
商品總額
↓
會員判斷
↓
折扣計算
↓
顯示最終金額
```

範例：

```text
原價：300元
會員：是
折扣：30元
應付金額：270元
```

## 清除訂單

- 商品數量歸零
- 清除訂單明細
- 清除結帳資訊

## 收據列印

```java
textArea.print();
```

## 即時時鐘

使用：

- Timer
- LocalDateTime
- DateTimeFormatter

每秒更新一次時間。

---

# 🏗 系統架構

```text
OrderUI
│
├── 飲料區
├── 餐點區
├── 明細區
├── 會員功能
├── 結帳系統
└── 收據列印
```

---

# 📦 類別設計

## Order.java

負責：

- 儲存訂單資料
- 商品數量管理
- 訂單總額計算

## OrderUI.java

負責：

- GUI介面顯示
- 按鈕事件處理
- 訂單明細更新
- 結帳功能

---

# 🔧 使用技術

| 技術 | 說明 |
|--------|--------|
| Java | 核心程式語言 |
| Swing | GUI介面 |
| WindowBuilder | 視窗設計工具 |
| OOP | 物件導向設計 |
| Event Listener | 事件監聽 |
| Timer | 即時時鐘 |

---

# 📈 系統流程圖

```text
開始
 ↓
選擇商品
 ↓
調整數量
 ↓
更新訂單明細
 ↓
是否會員？
 ↓
是 → 9折
否 → 原價
 ↓
結帳
 ↓
列印收據
 ↓
結束
```

---

# 🚀 執行方式

## Clone Repository

```bash
git clone https://github.com/your-account/Java-Ordering-System.git
```

## Import Project

1. Eclipse → Import Existing Project
2. 執行 `OrderUI.java`

---

# 📚 學習成果

✅ Java Swing GUI設計

✅ WindowBuilder應用

✅ Event Handling

✅ OOP設計概念

✅ 訂單管理邏輯

✅ 收據列印功能

✅ 即時資料更新

---

# 👨‍💻 Author

范天

Department of Information Management

Java Desktop Application Project
