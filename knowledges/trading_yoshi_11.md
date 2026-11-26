---
title: "Quy tắc Reclaim Entry (Vào lệnh lại) khi bị Stop Loss săn thanh khoản trước khi giá chạy đúng hướng"
source_author: "YoShi SMART TRADING (trên video dẫn nguồn nội dung / disclaimer: Scarface Trades)"
video_duration: "16:04"
video_type:
  - "Price Action / Key Level / Cấu trúc đỉnh đáy"
  - "SMC / ICT (Liquidity, Bẫy thanh khoản)"
  - "Quản lý vốn, quản trị rủi ro, tâm lý giao dịch, kỷ luật"
  - "Review lệnh / Live trading / Backtest"
markets:
  - "Chung (Cổ phiếu, Quyền chọn, Ngoại hối/Forex, Hợp đồng tương lai/Futures, Tiền điện tử/Crypto)"
timeframes_htf:
  - "5 phút (M5)"
  - "Ngày hôm trước (Daily / Previous Day)"
timeframes_ltf:
  - "1 phút (M1)"
tools:
  - "Mức cao nhất / thấp nhất của nến 5 phút đầu tiên (First 5-Minute Candle High/Low)"
  - "Mức cao nhất / thấp nhất phiên tiền thị trường (Premarket High/Low: 04:00 AM - 09:30 AM EST)"
  - "Mức cao nhất / thấp nhất ngày hôm trước (Previous Day High/Low: 09:30 AM - 16:00 PM EST)"
tags:
  - "Reclaim Entry"
  - "Stop Loss Hunt"
  - "Break and Retest"
  - "First 5-Minute Candle Strategy"
  - "Premarket High Low"
  - "Previous Day High Low"
  - "Risk Reward Ratio 2R"
  - "Day Trading"
  - "Price Action"
extraction_confidence: "Cao – Video giải thích rất chi tiết, hình ảnh chart trực quan và có 3 case study cụ thể kèm con số rủi ro/lợi nhuận thực tế."
---

# Quy tắc Reclaim Entry (Vào lệnh lại) khi bị Stop Loss săn thanh khoản trước khi giá chạy đúng hướng

## 0. TL;DR
- Video giải quyết bẫy tâm lý và kỹ thuật kinh điển: thiết lập vào lệnh (setup) chuẩn, vào lệnh đúng kế hoạch nhưng bị dính Stop Loss (SL) ở mức giá thấp/cao nhất tạm thời, sau đó giá lập tức chạy thẳng về mục tiêu chốt lời (Take Profit - TP). [NÓI]
- Giải pháp cốt lõi là quy tắc **"Reclaim Entry" (Vào lệnh thu hồi / Vào lệnh lại)**: khi lệnh 1 bị dính SL nhưng cấu trúc thị trường lớn hơn chưa bị phá vỡ (vẫn giữ được xu hướng/đáy hỗ trợ hợp lý), nhà giao dịch kiên nhẫn chờ giá vượt/đóng cửa trở lại qua mốc phá vỡ ban đầu với nến có xung lực mạnh (strong price action confirmation) để vào lại lệnh cùng hướng. [NÓI]
- Áp dụng kết hợp trên 3 chiến lược breakout cơ bản trong 90 phút đầu ngày: Nến 5 phút đầu tiên, Mức cao/thấp phiên tiền thị trường (Premarket H/L), và Mức cao/thấp ngày hôm trước (Previous Day H/L). [NÓI]
- Tỷ lệ Risk:Reward (R:R) luôn duy trì tối thiểu 2R để một lệnh Reclaim thắng có thể bù đắp lệnh thua đầu tiên và vẫn tạo ra lợi nhuận ròng. [NÓI]

## 1. Tổng quan
- **Vấn đề giải quyết:** Hiện tượng 90% nhà giao dịch thua lỗ hoặc nản lòng vì setup đẹp nhưng bị quét SL trước khi thị trường di chuyển theo đúng nhận định; loại bỏ tâm lý FOMO, sợ hãi, bực bội và giao dịch trả thù (revenge trading). [NÓI]
- **Đối tượng phù hợp:** Người mới bắt đầu lẫn nhà giao dịch chuyên nghiệp. [NÓI]
- **Thị trường áp dụng:** Mọi thị trường tài chính (Cổ phiếu, Quyền chọn / Options, Ngoại hối / Forex, Futures / Hợp đồng tương lai, Crypto / Tiền điện tử). [NÓI]
- **Thời gian áp dụng:** Tập trung chủ yếu vào 90 phút đầu tiên của ngày giao dịch (khi 90% lợi nhuận trong ngày của các nhà giao dịch được tạo ra). [NÓI]
- **Khung thời gian:**
  - Khung quan sát mốc tham chiếu (HTF): 5 phút (M5) hoặc Daily (mức ngày hôm trước). [NÓI]
  - Khung vào lệnh (LTF): 1 phút (M1). [NÓI, HÌNH]
- **Công cụ & Chỉ báo:** Không dùng chỉ báo phụ trợ phức tạp; chỉ sử dụng thuần túy biểu đồ nến (Price Action), các đường ngang đánh dấu Key Level (Đỉnh/Đáy nến M5 đầu tiên, Premarket High/Low, Previous Day High/Low). [NÓI, HÌNH]

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Bản chất thanh khoản & Hành vi Market Maker:** Các tổ chức tài chính lớn và Market Maker thường đẩy giá quét qua các mức SL hiển nhiên (nằm ngay dưới/trên các mức Breakout thông thường) để gom đủ thanh khoản trước khi đẩy giá đi theo xu hướng thực tế. [NÓI]
- **Sự khác biệt giữa "Mất đà" và "Phá vỡ cấu trúc":** Việc giá chạm SL ban đầu thường chỉ là một pha điều chỉnh quá đà hoặc mất đà tăng tạm thời (loss of momentum), chứ chưa phải là sự đảo chiều hay phá vỡ cấu trúc xu hướng tổng thể. Cấu trúc thị trường chỉ bị vô hiệu hóa khi mức đáy/đỉnh cấu trúc then chốt (major swing low/high) thực sự bị xuyên thủng. [NÓI]
- **Sức mạnh của Reclaim (Lấy lại vị thế):** Khi giá quay trở lại và đóng cửa vượt lên trên (đối với lệnh Long) hoặc giảm xuống dưới (đối với lệnh Short) mốc giá quan trọng bằng một cây nến có hành động giá mạnh mẽ, điều đó chứng minh phe kiểm soát ban đầu (ví dụ: phe mua) đã tái tham gia và kiểm soát lại thị trường. [NÓI]
- **Toán học xác suất (R:R tối thiểu 2R):** Nhờ duy trì tỷ lệ R:R tối thiểu 2R (rủi ro 1 phần, ăn 2 phần), nếu lệnh đầu tiên lỗ 1R và lệnh Reclaim Entry ăn 2R, tổng kết chuỗi lệnh vẫn lãi ròng +1R. [NÓI]

## 3. Thuật ngữ & Định nghĩa
| Thuật ngữ | Định nghĩa theo tác giả trong video | Cách nhận diện trên biểu đồ |
| :--- | :--- | :--- |
| **Reclaim Entry** | Quy tắc vào lại vị thế giao dịch sau khi lệnh ban đầu bị dính Stop Loss, khi giá quay trở lại mức cản then chốt và phe ban đầu tái chiếm quyền kiểm soát. [NÓI] | Nến M1 đóng cửa ngược trở lại qua đường Key Level đã bị phá vỡ trước đó kèm lực nến rõ ràng. [NÓI, HÌNH] |
| **First 5-Minute Candle Strategy** | Chiến lược xác định biên độ dao động của cây nến 5 phút đầu tiên sau giờ mở cửa thị trường. [NÓI] | Vẽ 2 đường ngang tại đỉnh cao nhất (High) và đáy thấp nhất (Low) của nến M5 đầu tiên, sau đó chuyển sang khung M1 tìm điểm phá vỡ. [NÓI, HÌNH] |
| **Premarket High / Low** | Mức giá cao nhất và thấp nhất được hình thành trong phiên tiền thị trường từ 04:00 AM đến 09:30 AM EST. [NÓI] | Kẻ 2 đường ngang đánh dấu đỉnh và đáy của vùng nến nằm trong khung thời gian 04:00 AM - 09:30 AM EST (vùng nền màu xám trên chart). [NÓI, HÌNH] |
| **Previous Day High / Low (PDH / PDL)** | Mức giá cao nhất và thấp nhất trong giờ giao dịch chính khóa (09:30 AM - 16:00 PM EST) của ngày hôm trước. [NÓI] | Kẻ 2 đường ngang tại đỉnh cao nhất và đáy thấp nhất của phiên ngày hôm trước. [NÓI, HÌNH] |
| **Structure Invalidation Level** | Mức giá mà nếu thị trường vượt qua, cấu trúc xu hướng của thiết lập mới thực sự bị phá vỡ hoàn toàn. [NÓI] | Đáy thấp nhất của sóng đẩy trước đó (đối với xu hướng tăng) hoặc đỉnh cao nhất của sóng giảm trước đó (đối với xu hướng giảm). [NÓI, HÌNH] |

## 4. Hệ thống quy tắc
Video trình bày 3 chiến lược xác định Key Level kết hợp chung với một Quy tắc cốt lõi: **Vào lệnh Reclaim Entry**.

### Chiến lược 1: Cây nến 5 phút đầu tiên (First 5-Minute Candle)
#### 4.1 Điều kiện tiên quyết & Xác định Key Level
- Chờ nến 5 phút (M5) đầu tiên sau giờ mở cửa hoàn tất đóng nến. [NÓI]
- Đánh dấu mức cao nhất (High) và mức thấp nhất (Low) của cây nến 5 phút này. [NÓI]
- Chuyển sang khung thời gian 1 phút (M1) để theo dõi phản ứng giá. [NÓI]

#### 4.2 Thiết lập ban đầu (Lệnh 1)
- **Tín hiệu:** Giá phá vỡ (Breakout) ra khỏi mức High hoặc Low của nến 5 phút, sau đó quay lại kiểm tra (Retest). [NÓI]
- **Entry lệnh 1:** Vào lệnh tại điểm kiểm tra lại (Retest) khi xuất hiện nến hành động giá xác nhận (ví dụ: nến bật tăng bảo vệ mức High). [NÓI, HÌNH]
- **Stop Loss lệnh 1:** Đặt tại đáy của cây nến đẩy (impulse candle) dẫn đến điểm vào lệnh hoặc mức giá đóng cửa ngược lại mức High/Low. [NÓI, HÌNH]
- **Take Profit lệnh 1:** Tỷ lệ R:R tối thiểu 2R, hoặc các mốc tâm lý số tròn (ví dụ: mốc 412). [NÓI, HÌNH]

#### 4.3 Quy tắc Reclaim Entry (Lệnh 2 - Khi lệnh 1 bị SL)
- **Điều kiện kiểm tra cấu trúc:** Kiểm tra xem mức đáy cấu trúc chính (Structure Invalidation Level) đã bị phá vỡ chưa. Nếu chưa bị phá vỡ, cấu trúc tăng vẫn còn nguyên giá trị, lệnh lỗ chỉ là do mất đà tạm thời. [NÓI]
- **Tín hiệu kích hoạt:** Giá quay đầu tăng ngược trở lại và tiến về mốc High của nến 5 phút. [NÓI]
- **Xác nhận (Confirmation):** Xuất hiện cây nến đóng cửa mạnh mẽ vượt lên trên mức High của nến 5 phút (nến nén/nến xanh thân lớn đẩy lên). [NÓI, HÌNH]
- **Entry Reclaim:** Vào lệnh Buy ngay sau khi nến xác nhận đóng cửa. [NÓI, HÌNH]
- **Stop Loss Reclaim:** Giữ nguyên mức dừng lỗ theo cấu trúc hoặc đặt dưới đáy của cây nến xác nhận vừa đóng cửa. [NÓI, HÌNH]
- **Take Profit Reclaim:** Giữ nguyên mục tiêu lợi nhuận ban đầu với tỷ lệ tối thiểu 2R. [NÓI]

---

### Chiến lược 2: Mức cao nhất & Thấp nhất phiên tiền thị trường (Premarket High/Low)
#### 4.1 Điều kiện tiên quyết & Xác định Key Level
- Xác định phiên tiền thị trường: từ 04:00 AM đến 09:30 AM (giờ miền Đông - EST). [NÓI]
- Đánh dấu mức cao nhất (Premarket High) và mức thấp nhất (Premarket Low) trong khoảng thời gian này. [NÓI]

#### 4.2 Thiết lập ban đầu (Lệnh 1)
- **Tín hiệu:** Sau khi mở cửa, giá phá vỡ Premarket Low (đối với Short) hoặc Premarket High (đối với Long). [NÓI]
- **Retest:** Chờ giá quay lại kiểm tra với hành động giá yếu (weak price action), bị từ chối tại mức cản. [NÓI]
- **Entry & SL lệnh 1:** Vào lệnh theo hướng phá vỡ; SL đặt quá mức nến đảo chiều hoặc mức phá vỡ trên nến đóng cửa tăng. [NÓI, HÌNH]
- **Take Profit lệnh 1:** Tối thiểu 2R. [NÓI]

#### 4.3 Quy tắc Reclaim Entry (Lệnh 2)
- **Đánh giá cấu trúc:** Mức SL của lệnh 1 thường do đặt quá hẹp. Nhìn lại biểu đồ nếu vùng tích lũy trước đó của phe bán/mua chưa bị vi phạm (chưa tạo đỉnh/đáy đảo chiều xu hướng chính), cấu trúc giao dịch vẫn hợp lệ. [NÓI]
- **Tín hiệu & Xác nhận:** Chờ giá quay trở lại mức Premarket Low (hoặc Premarket High) và xuất hiện cây nến đóng cửa từ chối mạnh mẽ (nến từ chối giảm, lực bán quay trở lại). [NÓI, HÌNH]
- **Entry Reclaim:** Vào lại lệnh cùng hướng ban đầu. [NÓI]
- **Stop Loss Reclaim:** Đặt cùng mức dừng lỗ cấu trúc hoặc phía trên đỉnh nến xác nhận từ chối. [NÓI, HÌNH]
- **Take Profit Reclaim:** Giữ nguyên mục tiêu ban đầu (tỷ lệ 2R đến 3R). [NÓI, HÌNH]

---

### Chiến lược 3: Mức cao nhất & Thấp nhất ngày hôm trước (Previous Day High/Low)
#### 4.1 Điều kiện tiên quyết & Xác định Key Level
- Quay lại phiên giao dịch ngày hôm trước (giờ chuẩn 09:30 AM - 16:00 PM EST). [NÓI]
- Đánh dấu mức cao nhất (Previous Day High - PDH) và mức thấp nhất (Previous Day Low - PDL). [NÓI]

#### 4.2 Thiết lập ban đầu (Lệnh 1)
- **Tín hiệu:** Giá phá vỡ PDH lên trên, sau đó retest ngay lập tức. [NÓI, HÌNH]
- **Entry & SL lệnh 1:** Vào lệnh Buy tại điểm retest; SL đặt dưới nến đóng cửa tăng hoặc dưới mức cản. [NÓI, HÌNH]
- **Take Profit lệnh 1:** Hướng về vùng thanh khoản tiếp theo (ví dụ: Premarket High). [NÓI]

#### 4.3 Quy tắc Reclaim Entry (Lệnh 2)
- **Kỷ luật tâm lý:** Không vội vàng vào lệnh ngay lập tức sau khi bị SL; không giao dịch trả thù. [NÓI]
- **Đánh giá cấu trúc:** Giá tạo đáy cao hơn (Higher Low), cấu trúc tăng khung lớn không bị phá vỡ. [NÓI, HÌNH]
- **Xác nhận:** Chờ đợi phe mua tái tham gia, xuất hiện cây nến xanh lớn đóng cửa vượt dứt khoát lên trên mức PDH. [NÓI, HÌNH]
- **Entry Reclaim:** Vào lệnh Buy ngay khi nến xác nhận đóng cửa trên PDH. [NÓI, HÌNH]
- **Stop Loss Reclaim:** Đặt ở mức hợp lý theo cấu trúc (dưới điểm phá vỡ của cây nến xác nhận). [NÓI]
- **Take Profit Reclaim:** Nhắm tới mức Premarket High hoặc tỷ lệ tối thiểu 2R. [NÓI]

---

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy bỏ Reclaim Entry
- Tuyệt đối không vào lệnh lại một cách mù quáng ngay sau khi bị cắn SL. [NÓI]
- Không vào lệnh Reclaim nếu cấu trúc thị trường chính đã bị phá vỡ (ví dụ: giá đâm thủng đáy/đỉnh cấu trúc vô hiệu hóa). [NÓI]
- Không vào lệnh nếu không có cây nến đóng cửa xác nhận lực đẩy mạnh mẽ (chỉ có râu nến quét qua nhưng nến không đóng cửa được ngoài mức cản). [NÓI]

## 5. Case Study / Ví dụ biểu đồ

### Ví dụ 1: Chiến lược nến 5 phút đầu tiên (First 5-Minute Candle Strategy)
- **Mốc thời gian:** 04:43 - 09:04 [HÌNH]
- **Khung thời gian:** M5 (xác định vùng cản ban đầu) và M1 (vào lệnh). [NÓI, HÌNH]
- **Hướng lệnh:** Long (Buy). [HÌNH]
- **Bối cảnh trước setup:** Giá mở cửa phiên chính, sau phiên tiền thị trường đi ngang giảm nhẹ. [HÌNH]
- **Diễn biến Lệnh 1:**
  - Nến M5 đầu tiên đóng cửa, đánh dấu High và Low. [NÓI]
  - Trên M1, giá phá vỡ lên trên mức High của nến 5 phút, sau đó quay lại kiểm tra (retest). [NÓI, HÌNH]
  - Vào lệnh Buy tại điểm retest. [NÓI]
  - Stop Loss: Đặt dưới nến đẩy vào lệnh ($1,360 rủi ro). [NÓI, HÌNH]
  - Take Profit: Nhắm tới số tròn tâm lý 412, kỳ vọng lợi nhuận $2,850, tỷ lệ R:R khoảng 2.22R. [NÓI, HÌNH]
  - Kết quả lệnh 1: Giá quay xuống đóng cửa dưới mức High của nến 5 phút, cắn SL của lệnh ($1,360 lỗ). [NÓI, HÌNH]
- **Diễn biến Lệnh 2 (Reclaim Entry):**
  - Đánh giá cấu trúc: Đáy thấp nhất của cấu trúc tăng trước đó (Structure Invalidation Low) không hề bị phá vỡ. Việc quét SL chỉ là mất đà tạm thời. [NÓI]
  - Xác nhận: Phe mua quay lại đẩy giá vượt lên trên mức High của nến 5 phút, xuất hiện nến M1 đóng cửa tăng mạnh. [NÓI, HÌNH]
  - Entry Reclaim: Vào Buy khi nến M1 đóng cửa trên mức High. [NÓI, HÌNH]
  - Stop Loss: Đặt dưới chân nến xác nhận, rủi ro khoảng $1,330. [NÓI, HÌNH]
  - Take Profit: Giữ nguyên mục tiêu ban đầu, lợi nhuận tiềm năng $2,810 (tỷ lệ R:R ~ 2.11R). [HÌNH]
  - Kết quả: Lệnh đạt thẳng mục tiêu TP chỉ trong vòng 2 phút. [NÓI, HÌNH]
  - Bài học: Lỗ lệnh 1 là $1,360, nhưng thắng lệnh 2 được $2,810, tài khoản vẫn có lợi nhuận ròng lớn thay vì tức giận bỏ cuộc. [NÓI, SUY LUẬN: Tính toán từ các con số tác giả đưa ra]

---

### Ví dụ 2: Chiến lược Premarket High/Low
- **Mốc thời gian:** 09:05 - 13:08 [HÌNH]
- **Khung thời gian:** M1 (sau khi xác định mức cản Premarket 04:00 - 09:30 EST). [NÓI, HÌNH]
- **Hướng lệnh:** Short (Sell). [HÌNH]
- **Bối cảnh:** Vùng tiền thị trường có mức biến động đáy rõ ràng. Thị trường mở cửa phá vỡ xuống dưới Premarket Low. [NÓI, HÌNH]
- **Diễn biến Lệnh 1:**
  - Giá phá vỡ Premarket Low, sau đó quay lại kiểm tra với lực nến yếu. [NÓI]
  - Vào lệnh Short tại điểm kiểm tra lại. [NÓI]
  - Stop Loss: Đặt quá hẹp ngay phía trên nến đóng cửa tăng ($410 rủi ro). [NÓI, HÌNH]
  - Take Profit: Mục tiêu vùng giá gần 6915, lợi nhuận tiềm năng khoảng $800 (tỷ lệ 2R). [NÓI, HÌNH]
  - Kết quả lệnh 1: Phe mua xuất hiện đẩy nhẹ lên cắn SL ($410 lỗ). [NÓI, HÌNH]
- **Diễn biến Lệnh 2 (Reclaim Entry):**
  - Đánh giá cấu trúc: Cổ phiếu trước đó có vùng tích lũy mà phe mua đã thử nhảy vào 3-4 lần rồi mới phá vỡ. Giá chưa từng phá vỡ cấu trúc giảm lớn hơn. [NÓI]
  - Tín hiệu xác nhận: Giá bị từ chối chính xác tại đáy của nến M5 trước đó, phe bán xuất hiện trở lại và có nến M1 đóng cửa nén mạnh quay trở lại dưới mức Premarket Low. [NÓI, HÌNH]
  - Entry Reclaim: Vào lệnh Short lại. [NÓI, HÌNH]
  - Stop Loss: Giữ nguyên quy tắc dừng lỗ cấu trúc, rủi ro khoảng $310. [NÓI, HÌNH]
  - Take Profit: Giữ nguyên mức TP ban đầu, tiềm năng lợi nhuận khoảng $930 (tỷ lệ R:R đạt 3R). [NÓI, HÌNH]
  - Kết quả: Lệnh chạm thẳng mục tiêu TP lớn. [NÓI, HÌNH]

---

### Ví dụ 3: Chiến lược Previous Day High/Low
- **Mốc thời gian:** 13:09 - 16:04 [HÌNH]
- **Khung thời gian:** Daily (lấy mức ngày hôm trước: phiên thứ Năm cho ngày giao dịch thứ Sáu) và M1 (thực thi). [NÓI, HÌNH]
- **Hướng lệnh:** Long (Buy). [HÌNH]
- **Bối cảnh:** Giờ giao dịch mở cửa, giá phá vỡ mức Previous Day High (PDH) lên trên. [NÓI, HÌNH]
- **Diễn biến Lệnh 1:**
  - Giá phá vỡ PDH và retest ngay lập tức. [NÓI, HÌNH]
  - Vào lệnh Buy; SL đặt dưới nến đóng cửa tăng ($420 rủi ro). [NÓI, HÌNH]
  - Take Profit: Nhắm tới đỉnh phiên tiền thị trường (Premarket High) - vùng thanh khoản tiếp theo, lợi nhuận tiềm năng $1,930 (R:R > 4R). [NÓI, HÌNH]
  - Kết quả lệnh 1: Bị dính SL rất nhanh do một cú giật quét xuống. [NÓI, HÌNH]
- **Diễn biến Lệnh 2 (Reclaim Entry):**
  - Kiểm soát tâm lý: Tác giả nhấn mạnh "không vội vàng thực hiện lệnh khác ngay lập tức, mà kiên nhẫn chờ xem có sự lấy lại nào xuất hiện hay không". [NÓI]
  - Đánh giá cấu trúc: Giá tạo một đáy cao hơn (Higher Low), cấu trúc tăng hoàn toàn không bị vô hiệu hóa. [NÓI, HÌNH]
  - Xác nhận: Phe mua lớn tham gia trở lại, đẩy một cây nến xanh đóng cửa dứt khoát trên mức PDH. [NÓI, HÌNH]
  - Entry Reclaim: Vào lệnh Buy ngay sau cây nến xác nhận. [NÓI, HÌNH]
  - Stop Loss: Đặt tại mức phá vỡ của cây nến này ($840 rủi ro). [NÓI, HÌNH]
  - Take Profit: Nhắm mục tiêu mức Premarket High, lợi nhuận tiềm năng $1,650 (tỷ lệ ~ 2R). [NÓI, HÌNH]
  - Kết quả: Giá bứt phá mạnh mẽ chạm thẳng mục tiêu lợi nhuận cao nhất trước giờ mở cửa. [NÓI, HÌNH]

## 6. Tips, Tricks & Cảnh báo
- **Tập trung khung giờ vàng:** 90% lợi nhuận trong ngày của hầu hết nhà giao dịch được tạo ra trong 90 phút đầu tiên sau khi mở cửa; không cần ngồi trước màn hình cả ngày. [NÓI]
- **Tâm lý chấp nhận SL:** Việc có quy tắc Reclaim Entry giúp tâm lý cực kỳ thoải mái khi đặt và bị dính Stop Loss ở lệnh đầu tiên, vì biết rằng kế hoạch vẫn còn cơ hội vào lại lệnh tốt hơn. [NÓI]
- **Sai lầm gồng lỗ:** Rất nhiều nhà giao dịch không chịu cắt lỗ vì hy vọng giá sẽ quay trở lại, dẫn đến các khoản lỗ lớn gấp nhiều lần khoản lãi. Quy tắc này cho phép cắt lỗ dứt khoát và chỉ vào lại khi có xác nhận. [NÓI]
- **Cảnh báo vào lệnh mù quáng:** Có quy tắc Reclaim không đồng nghĩa với việc cứ bị cắn SL là lao vào Buy/Sell lại ngay (Revenge trading). Bắt buộc phải chờ nến đóng cửa xác nhận lực (candle close with strong price action) và cấu trúc chưa bị gãy. [NÓI]
- **Mẹo R:R tối thiểu 2R:** Luôn bảo đảm tỷ lệ R:R ít nhất 2R. Ví dụ cược $100 để ăn $200; nếu lệnh 1 thua mất $100, lệnh Reclaim thắng được $200 thì tổng kết vẫn lãi $100. [NÓI]

## 7. Quản trị rủi ro & Tâm lý
- **Quy tắc dừng lỗ dứt khoát:** Luôn tuân thủ SL ở lệnh đầu tiên, không thả trôi SL hoặc dịch chuyển SL xa hơn. [NÓI]
- **Tỷ lệ R:R cố định:** Tối thiểu 1:2 (2R). [NÓI]
- **Khối lượng rủi ro:** Được tính toán bằng khoảng cách từ Entry đến SL theo cấu trúc (trong các ví dụ thực tế của tác giả dao động từ $310 đến $1,360 tùy biên độ nến). [HÌNH]
- **Kiểm soát cảm xúc:** Loại bỏ hoàn toàn sự ức chế (frustrated), tức giận (angry), bối rối (confused), căng thẳng (stressed), mệt mỏi vì thua cuộc (tired of losing) hay nỗi sợ bỏ lỡ cơ hội (FOMO) bằng quy trình máy móc hóa (mechanical rules-based system). [NÓI, HÌNH]

## 8. Đặc tả logic cho LLM / Bot

Quy tắc thuật toán dưới đây được mô tả đối xứng cho cả chiều LONG (Buy) và SHORT (Sell).

- ĐIỀU KIỆN THỜI GIAN & BỐI CẢNH (CONTEXT):
  - `Trading_Session` = "90 phút đầu tiên kể từ giờ mở cửa chính thức" (09:30 AM EST trở đi)
  - Xác định một trong 3 loại `Key_Level`:
    - Loại 1: `Key_Level_High` và `Key_Level_Low` của nến 5 phút đầu tiên (First M5 Candle)
    - Loại 2: `Premarket_High` và `Premarket_Low` hình thành từ 04:00 AM đến 09:30 AM EST
    - Loại 3: `Previous_Day_High` và `Previous_Day_Low` hình thành từ 09:30 AM đến 16:00 PM EST ngày hôm trước

- THIẾT LẬP VÀO LỆNH BAN ĐẦU (TRADE 1 - LONG):
  - TRIGGER 1:
    - Giá nến M1 đóng cửa vượt lên trên `Key_Level_High`
    - Giá M1 có nhịp hồi kiểm tra lại (`Retest`) tại `Key_Level_High`
  - ENTRY 1:
    - `Entry_Price_1` = Giá đóng cửa nến M1 phản ứng tăng tại vùng Retest
  - STOP LOSS 1:
    - `SL_Price_1` = Đáy của cây nến xung lực đẩy hoặc điểm nến M1 đóng cửa quay lại dưới `Key_Level_High`
  - TAKE PROFIT 1:
    - `TP_Price_1` >= `Entry_Price_1` + 2 * (`Entry_Price_1` - `SL_Price_1`) hoặc mốc cản thanh khoản tiếp theo

- ĐIỀU KIỆN QUẢN LÝ THUA LỖ LỆNH 1:
  - Nếu Giá chạm `SL_Price_1`:
    - Khớp lệnh Stop Loss ngay lập tức
    - Chuyển trạng thái sang `WAITING_FOR_RECLAIM`

- ĐIỀU KIỆN LỌC RECLAIM (RECLAIM FILTER):
  - Xác định `Structure_Invalidation_Level` = Đáy swing low quan trọng gần nhất trước cú breakout
  - ĐIỀU KIỆN HỦY:
    - NẾU giá chạm hoặc đóng cửa dưới `Structure_Invalidation_Level`:
      - HỦY toàn bộ kịch bản Reclaim (Cấu trúc bị phá vỡ hoàn toàn)
      - Trạng thái = `CANCELLED`

- TÍN HIỆU KÍCH HOẠT VÀO LỆNH LẠI (TRADE 2 - RECLAIM ENTRY LONG):
  - TRIGGER 2:
    - Giá duy trì phía trên `Structure_Invalidation_Level`
    - Giá quay trở lại và có nến M1 đóng cửa vượt dứt khoát lên trên `Key_Level_High`
    - `SUBJECTIVE:` Tác giả mô tả là "cây nến hành động giá mạnh mẽ với sự tham gia của phe mua"
  - ENTRY RECLAIM:
    - `Entry_Price_2` = Giá đóng cửa của cây nến M1 xác nhận vừa vượt qua `Key_Level_High`
  - STOP LOSS RECLAIM:
    - `SL_Price_2` = Đáy của cây nến xác nhận M1 (hoặc đáy cấu trúc hợp lý gần nhất)
  - TAKE PROFIT RECLAIM:
    - `TP_Price_2` = `TP_Price_1` (hoặc đảm bảo tỷ lệ tối thiểu 2R: `Entry_Price_2` + 2 * (`Entry_Price_2` - `SL_Price_2`))

- ĐỐI XỨNG CHO SHORT (SELL):
  - Thay thế `Key_Level_High` bằng `Key_Level_Low`
  - Thay thế `Structure_Invalidation_Level` (đáy) bằng đỉnh swing high cấu trúc quan trọng
  - Đổi chiều logic kiểm tra Breakout xuống dưới, Retest, Stop Loss phía trên, và Reclaim khi nến M1 đóng cửa nén mạnh quay trở lại dưới `Key_Level_Low`.

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Tiêu chuẩn "Nến hành động giá mạnh mẽ":** Tác giả dùng thuật ngữ trực quan như "strong price action candle", "bulls stepping in", "strong push", nhưng không đưa ra con số định lượng cụ thể (như thân nến chiếm bao nhiêu %, volume đột biến bao nhiêu lần so với đường trung bình). [SUY LUẬN: Cần kết hợp quan sát nến Marubozu/thân lớn hoặc volume xác nhận nếu lập trình bot].
- **Mức Stop Loss của Lệnh Reclaim:** Trong ví dụ 1, SL đặt dưới chân nến xác nhận; trong ví dụ 2, tác giả nói dùng "cùng mức dừng lỗ cấu trúc" (same stop loss); ở ví dụ 3, tác giả nói "đặt ở mức phá vỡ của cây nến này". Tác giả linh hoạt giữa SL theo nến xác nhận và SL theo đáy cấu trúc mà không quy định cứng một công thức pip/tick cố định.
- **Thời gian chờ Reclaim:** Video không quy định thời gian tối đa để setup Reclaim có hiệu lực (ví dụ: sau khi SL thì trong vòng bao nhiêu cây nến M1 giá phải quay lại? Nếu giá đi ngang 2 tiếng thì còn hiệu lực không?).

## 10. Thông tin khác
- **Kênh & Nguồn tham chiếu:** Yoshi Smart Trading; disclaimer nhắc tới bản quyền giáo dục của Scarface Trades. [HÌNH]
- **Tài liệu miễn phí đi kèm:** Video nhắc tới danh sách phát miễn phí và khóa học 10 giờ đào tạo chuyên sâu về các khái niệm giao dịch được đặt trong phần mô tả video. [NÓI]
- **Tuyên bố kết quả của tác giả:** Tác giả hiển thị các kết quả giao dịch mẫu P&L (ví dụ: +$1,507.29 ngày 04/03/2026; +$1,365.24 ngày 28/02/2026; +$1,260.08 ngày 02/03/2026) với tuyên bố kinh nghiệm 7 năm giao dịch. Các con số này mang tính chất minh họa cá nhân, chưa được bên thứ ba kiểm chứng độc lập. [HÌNH]
- **Trích dẫn đáng chú ý:**
  - *"90% of traders lose because they don't understand one rule institutions, banks, and profitable traders use."* [HÌNH]
  - *"Trade 90 minutes / day because that's when 90% of profits are made."* [NÓI, HÌNH]