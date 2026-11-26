~~~
---
title: "Hệ thống giao dịch ICT tinh gọn: Thanh khoản, Cấu trúc, Market Maker Model và 3 mô hình Entry"
source_author: "Yoshi Smart Trading"
video_duration: "09:58"
video_type: [SMC / ICT, Price Action / Key Level, Mô hình nến, Quản lý vốn, Review lệnh / Live trading]
markets: [Chung, Forex, Indices, Crypto]
timeframes_htf: [Weekly, Daily, 4 Hour, 1 Hour, 15 Minute]
timeframes_ltf: [4 Hour, 1 Hour, 15 Minute, 5 Minute, 1 Minute]
tools: [Biểu đồ nến sạch (Clean Chart), Fair Value Gap (FVG), Swing High / Swing Low]
tags: [ICT, SMC, Liquidity, FVG, IFVG, CISD, MSS, Power of 3, Market Maker Models, Multi-timeframe]
extraction_confidence: "Cao – Nội dung video trình bày mạch lạc, slide chữ tiếng Anh kèm thuyết minh tiếng Việt rõ ràng từng định nghĩa, quy tắc và ví dụ minh họa."
---
~~~

# Hệ thống giao dịch ICT tinh gọn: Thanh khoản, Cấu trúc, Market Maker Model và 3 mô hình Entry

## 0. TL;DR
- Video hệ thống hóa toàn bộ phương pháp giao dịch ICT thành 4 trụ cột cốt lõi: Thanh khoản (Liquidity), Cấu trúc thị trường (Market Structure), Mô hình nhà tạo lập (Market Maker Models), và Sức mạnh của 3 (Power of 3 - PO3) [NÓI].
- Giá luôn di chuyển như nam châm từ vùng thanh khoản nội bộ (Internal Range Liquidity - IRL / FVG) sang vùng thanh khoản bên ngoài (External Range Liquidity - ERL / Swing High, Swing Low) và ngược lại [NÓI].
- Quy tắc bất biến: "No key level tap = No Trade" (Không chạm vùng giá quan trọng HTF thì tuyệt đối không vào lệnh) [NÓI], [HÌNH].
- Cung cấp 3 mô hình vào lệnh (Entry Models) cụ thể trên khung thời gian nhỏ (LTF): Inverted FVG (IFVG), Change in State of Delivery (CISD), và Market Structure Shift (MSS) + FVG [NÓI], [HÌNH].
- Bắt buộc áp dụng ma trận đồng bộ khung thời gian (Time Frame Alignment) và duy trì tỷ lệ R:R tối thiểu 2:1 cho mọi vị thế [NÓI], [HÌNH].

---

## 1. Tổng quan
- **Mục tiêu / Vấn đề giải quyết**: Đơn giản hóa phương pháp ICT phức tạp thành một quy trình có tính hệ thống cao, loại bỏ thông tin thừa nhằm giúp trader không còn bị dính bẫy quét Stop Loss (Stop Hunt) của nhà cái trước khi giá chạy đúng hướng [NÓI].
- **Đối tượng phù hợp**: Trader đã từng học hoặc áp dụng ICT/SMC nhưng hay bị thua lỗ do quá tải khái niệm, mong muốn tìm kiếm quy tắc vào lệnh nhất quán [NÓI].
- **Thị trường áp dụng**: Áp dụng chung cho thị trường tài chính (Forex, Chỉ số chứng khoán như NQ, Crypto...) [HÌNH], [SUY LUẬN: Trên chart hiển thị mã NQM5 - Nasdaq Futures].
- **Khung thời gian áp dụng**: Đa khung thời gian kết hợp theo cặp cố định (Weekly/4H, Daily/1H, 4H/15m, 1H/5m, 15m/1m) [HÌNH], [NÓI].
- **Công cụ & Chỉ báo**: Biểu đồ giá nến trần (Clean Chart), không sử dụng bất kỳ chỉ báo dao động hay đường trung bình truyền thống nào; chỉ dùng các cấu trúc giá tự nhiên: Fair Value Gap (FVG) và Swing Points [HÌNH].

---

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Cơ chế thanh khoản**: Giá luôn di chuyển về nơi tập trung nhiều lệnh dừng lỗ (Stop Loss) nhất vì các quỹ lớn/nhà đầu tư tổ chức cần khối lượng thanh khoản đối ứng đó để quét lệnh và khớp vị thế khối lượng lớn của họ [NÓI].
- **Lực hút nam châm**: Thị trường dao động liên tục giữa hai trạng thái: tìm kiếm sự cân bằng qua vùng mất cân bằng thanh khoản nội bộ (FVG) và săn tìm thanh khoản bên ngoài phạm vi (đỉnh/đáy xoay chiều) [NÓI].
- **Bẫy tích lũy của Smart Money (Market Maker Models)**: Trên đường giá hồi về vùng FVG khung lớn, thị trường thường cố tình tạo ra từ 2 vùng tích lũy (consolidation) trở lên để dụ trader nhỏ lẻ vào lệnh sớm. Khi giá quét sạch SL dưới các vùng tích lũy này và chạm vào HTF FVG, đó mới là điểm đảo chiều thực sự của nhà cái [NÓI].
- **Chu kỳ Power of 3 (PO3)**: Thị trường luôn vận hành theo kịch bản 3 bước: Tích lũy (Accumulation) -> Quét dừng lỗ/Thao túng (Stop Run / Manipulation) -> Đảo chiều/Bứt phá mạnh (Reversal / Distribution) [NÓI], [HÌNH].

---

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo tác giả trong video | Cách nhận diện trên biểu đồ |
| :--- | :--- | :--- |
| **Liquidity (Thanh khoản)** | Nơi tập trung nhiều lệnh dừng lỗ nhất của trader nhỏ lẻ, là đích đến liên tục của dòng tiền lớn [NÓI]. | Các đỉnh/đáy xoay chiều rõ ràng hoặc các khoảng trống giá chưa được lấp đầy [NÓI]. |
| **External Liquidity (ERL)** | Thanh khoản bên ngoài biên độ dao động [NÓI], [HÌNH]. | Các đỉnh xoay chiều (Swing High) hoặc đáy xoay chiều (Swing Low) [HÌNH]. |
| **Internal Liquidity (IRL)** | Thanh khoản nội bộ nằm bên trong phạm vi sóng [NÓI], [HÌNH]. | Các khoảng trống giá trị hợp lý (Fair Value Gap - FVG) [HÌNH]. |
| **Fair Value Gap (FVG)** | Khoảng trống giá trị hợp lý, xuất hiện khi có một cây nến thân lớn tạo ra vùng trống giữa bóng nến của nến trước và nến sau [NÓI]. | Mô hình 3 nến: Khoảng cách giữa bóng nến (wick) của nến 1 và bóng nến của nến 3 không chạm vào nhau [NÓI], [HÌNH]. |
| **Swing Low (Đáy xoay)** | Đáy cấu trúc tiêu chuẩn theo mô hình 3 nến [NÓI]. | Nến ở giữa có mức giá thấp nhất, hai nến hai bên có đáy cao hơn [NÓI], [HÌNH]. |
| **Swing High (Đỉnh xoay)** | Đỉnh cấu trúc tiêu chuẩn theo mô hình 3 nến [NÓI]. | Nến ở giữa có mức giá cao nhất, hai nến hai bên có đỉnh thấp hơn [NÓI], [HÌNH]. |
| **Manipulation (Thao túng)** | Cú quét qua đỉnh/đáy nhưng không có động lượng duy trì, nến không đóng cửa được ngoài mức đó (weak sweep) [NÓI], [HÌNH]. | Râu nến đâm xuyên qua đỉnh/đáy cũ nhưng thân nến đóng cửa ngược lại vào bên trong phạm vi [HÌNH]. |
| **Displacement (Dịch chuyển)** | Cú phá vỡ mạnh mẽ, dứt khoát thể hiện sự tham gia của dòng tiền lớn [NÓI], [HÌNH]. | Nến thân dài đóng cửa vượt qua điểm cấu trúc và để lại một FVG mới [NÓI], [HÌNH]. |
| **Market Structure Shift (MSS)** | Sự chuyển đổi cấu trúc thị trường từ chuỗi đỉnh/đáy thấp hơn sang tạo đỉnh cao hơn thực sự (hoặc ngược lại) [NÓI]. | Thân nến đóng cửa vượt qua đỉnh/đáy cấu trúc gần nhất kèm theo sự xuất hiện của một FVG [NÓI], [HÌNH]. |
| **Inverted FVG (IFVG)** | Khoảng trống giá bị đảo ngược vai trò sau khi giá đóng cửa xuyên thủng [NÓI], [HÌNH]. | Một FVG giảm (bearish FVG) bị một cây nến tăng đóng cửa hoàn toàn vượt qua phía trên [NÓI], [HÌNH]. |
| **Change in State of Delivery (CISD)** | Sự thay đổi trạng thái phân phối của nến [NÓI], [HÌNH]. | Một chuỗi các cây nến cùng màu kiểm soát thị trường bị một cây nến/nhịp nến đối lập nuốt trọn hoàn toàn (engulf) [NÓI], [HÌNH]. |
| **Power of 3 (PO3)** | Chu kỳ chuyển động 3 pha của giá trong ngày hoặc một nhịp sóng: Tích lũy - Quét dừng lỗ - Đảo chiều [NÓI], [HÌNH]. | Vùng đi ngang (sideway) -> Nhúng xuống quét đáy (fakeout/stop run) -> Bứt phá mạnh theo hướng ngược lại [NÓI], [HÌNH]. |

---

## 4. Hệ thống quy tắc

### 4.1 Điều kiện tiên quyết / Confluence (Checklist [ ])
- [ ] Giá trên khung thời gian lớn (HTF) phải chạm vào một Key Level rõ ràng: HTF Fair Value Gap (IRL) hoặc HTF Swing High/Low (ERL) [NÓI], [HÌNH].
- [ ] Tuân thủ tuyệt đối quy tắc: "No key level tap = No Trade" [HÌNH].
- [ ] Khung thời gian vào lệnh (LTF) phải tương ứng chính xác với khung HTF theo ma trận đồng bộ [NÓI], [HÌNH].
- [ ] Thiết lập tỷ lệ R:R tối thiểu đạt 2:1 [NÓI], [HÌNH].

### 4.2 Xác định bối cảnh & hướng (Bias)
- Xác định giá đang di chuyển từ đâu tới đâu: Nếu giá vừa hoàn tất quét thanh khoản bên ngoài (ERL), hướng tiếp theo là hút về thanh khoản nội bộ (IRL/FVG) [NÓI].
- Ngược lại, khi giá đã lấp đầy FVG trên HTF, hướng đi tiếp theo là bứt phá về phía đỉnh/đáy xoay chiều gần nhất (ERL) [NÓI].
- Hướng giao dịch (Buy/Sell) được quyết định dựa trên phản ứng của giá tại Key Level HTF [NÓI].

### 4.3 Tín hiệu kích hoạt (Triggers)
Sau khi giá chạm Key Level HTF, chuyển xuống LTF và chờ 1 trong 3 mô hình kích hoạt sau:
- **Trigger 1: Inverted FVG (IFVG)**: Giá xuyên qua và đóng nến hoàn toàn vượt qua một FVG ngược hướng đang cản đường [NÓI], [HÌNH].
- **Trigger 2: Change in State of Delivery (CISD)**: Nhịp nến tăng nuốt trọn (engulf) toàn bộ chuỗi nến giảm liên tiếp trước đó vừa quét thanh khoản [NÓI], [HÌNH].
- **Trigger 3: MSS + FVG**: Giá đóng nến phá vỡ đỉnh cấu trúc gần nhất (Swing High) và hình thành một FVG mới [NÓI], [HÌNH].

### 4.4 Entry
- **Với Mô hình IFVG**: Vào lệnh Market ngay khi cây nến đóng cửa xuyên thủng hoàn toàn FVG ngược chiều [NÓI], [HÌNH].
- **Với Mô hình CISD**: Vào lệnh ngay khi toàn bộ nhịp nến giảm trước đó bị nuốt trọn (engulfed) [NÓI], [HÌNH].
- **Với Mô hình MSS + FVG**: Vào lệnh Limit khi giá hồi về kiểm tra (retrace) FVG mới hình thành sau phá vỡ cấu trúc [HÌNH] hoặc vào lệnh theo xác nhận nến đóng cửa [NÓI].

### 4.5 Stop Loss
- Quy tắc đặt SL cố định cho cả 3 mô hình: Đặt ngay bên dưới mức đáy thấp nhất vừa được tạo ra bởi cú thao túng/quét thanh khoản (Lowest Low vừa hình thành) [NÓI], [HÌNH].

### 4.6 Take Profit / Quản lý lệnh
- **Vị trí TP**: Đặt tại đỉnh xoay chiều (Swing High) trên khung thời gian lớn HTF, hoặc vùng "Đỉnh thất bại" (Failed High - đỉnh không tạo được đáy mới thấp hơn) [NÓI], [HÌNH].
- **Tỷ lệ R:R**: Bắt buộc đạt tỷ lệ Risk/Reward tối thiểu là 2:1 trở lên [NÓI], [HÌNH].
- **Quản lý lệnh đang chạy**: Một khi setup tăng đã kích hoạt, mọi nhịp giá rơi xuống dưới đáy tạm thời được xem là thao túng tiếp diễn, trader có thể cân nhắc dời Stop Loss lên các đáy mới này để bảo toàn vốn và giảm thiểu rủi ro [NÓI].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- Thị trường chạm vào vùng thanh khoản nhưng không xuất hiện hiện tượng Dịch chuyển (Displacement) và không tạo ra bất kỳ FVG mới nào [NÓI], [HÌNH].
- Giá chưa chạm vào bất kỳ Key Level HTF nào ("No key level tap = No Trade") [HÌNH].
- Tỷ lệ R:R đo đạc từ Entry đến đỉnh mục tiêu HTF nhỏ hơn 2:1 [NÓI], [HÌNH].

---

## 5. Case Study / Ví dụ biểu đồ

### Ví dụ 1: Cơ chế nam châm thanh khoản IRL sang ERL (01:05 - 01:50)
- **Mốc thời gian**: 01:05 - 01:50.
- **Sản phẩm & Khung thời gian**: Biểu đồ nến mẫu (không hiện rõ cặp tiền, [SUY LUẬN: Minh họa nguyên lý chung]).
- **Bối cảnh**: Giá đang nằm trong xu hướng tăng và vừa hồi về một vùng FVG tăng (IRL) [NÓI], [HÌNH].
- **Hành động giá**: Giá chạm FVG, phản ứng bật tăng, để lại FVG tiếp diễn và tiến thẳng lên quét đỉnh cũ (Swing High - ERL) [NÓI], [HÌNH].
- **Quy tắc minh họa**: Giá luôn di chuyển có trật tự từ vùng mất cân bằng nội bộ sang vùng thanh khoản đỉnh/đáy bên ngoài [NÓI].

### Ví dụ 2: Nhận diện Manipulation và nhắm mục tiêu "Đỉnh thất bại" (02:35 - 03:36)
- **Mốc thời gian**: 02:35 - 03:36.
- **Sản phẩm & Khung thời gian**: Biểu đồ nến [HÌNH].
- **Bối cảnh**: Giá rơi xuống kiểm tra 2 đáy cũ liền kề [HÌNH].
- **Hành động giá**: Râu nến đâm xuyên qua 2 đáy nhưng không có nến nào đóng cửa bên dưới mức đó (không có Displacement). Sau đó giá quay đầu tăng, đóng nến vượt đỉnh cấu trúc nhỏ và tạo FVG (MSS) [NÓI], [HÌNH].
- **Target TP**: Tác giả xác định một đỉnh Swing High trước đó có nhiệm vụ đẩy giá xuống tạo đáy sâu hơn nhưng đã thất bại (Failed High) -> Đỉnh này trở thành mục tiêu thanh khoản hoàn hảo để chốt lời [NÓI], [HÌNH].
- **Bài học rút ra**: Không được nhầm lẫn râu quét đáy là phá vỡ cấu trúc; không đóng nến vượt qua đồng nghĩa với thao túng (Manipulation) [NÓI].

### Ví dụ 3: Mô hình Market Maker - Bẫy tích lũy kép (04:06 - 05:27)
- **Mốc thời gian**: 04:06 - 05:27.
- **Khung thời gian**: HTF kết hợp LTF [HÌNH].
- **Bối cảnh**: Trên HTF, giá đang điều chỉnh giảm về một HTF FVG [NÓI], [HÌNH].
- **Phân tích LTF**: Trên đường rơi xuống, giá tạo ra 2 vùng tích lũy đi ngang (Accumulation 1 và Accumulation 2) [NÓI], [HÌNH]. Trader nhỏ lẻ mua sớm ở vùng đi ngang và đặt SL ngay dưới đó.
- **Diễn biến**: Giá đâm sầm xuống quét toàn bộ SL của 2 vùng tích lũy, chạm khít vào HTF FVG, sau đó xuất hiện một cú bứt phá mạnh (Displacement) tạo FVG mới trên LTF [NÓI], [HÌNH].
- **Bài học**: Chờ đợi giá quét hết thanh khoản của các vùng tích lũy LTF và xác nhận phản ứng tại HTF FVG mới được tìm điểm vào [NÓI].

### Ví dụ 4: Giao dịch thực tế kiếm $41,100 bằng Power of 3 (05:45 - 06:27)
- **Mốc thời gian**: 05:45 - 06:27.
- **Thời gian giao dịch**: Thứ Năm, ngày 11/05/2023 (theo nhật ký Daily Journal hiển thị trên màn hình: Net P&L: +$41,100.00) [HÌNH], [NÓI].
- **Bối cảnh & Cấu trúc**: Thị trường mở phiên bằng một vùng tích lũy đi ngang (Accumulation) [NÓI], [HÌNH].
- **Setup**: Giá thực hiện một cú quét dừng lỗ (Stop Run) đâm xuyên qua các đáy của vùng tích lũy, sau đó bật ngược trở lại vùng giá cũ và bứt phá tăng mạnh (Reversal/Distribution) [NÓI], [HÌNH].
- **Kết quả**: Bắt trọn sóng tăng mạnh trong ngày dựa vào việc kiên nhẫn chờ cú Stop Run hoàn tất [NÓI].

### Ví dụ 5: Setup Entry Model 1 - Inverted FVG (07:32 - 08:30)
- **Mốc thời gian**: 07:32 - 08:30.
- **Bối cảnh**: Giá chạm vùng HTF FVG tăng ở phía dưới, đồng thời test vùng thanh khoản đáy ngoài phạm vi [HÌNH].
- **Kích hoạt**: Trên đường giảm xuống có một cây nến giảm tạo FVG (bearish FVG). Ngay sau khi chạm HTF FVG, một nến xanh tăng mạnh đóng cửa vượt hẳn lên trên khoảng FVG giảm này (tạo IFVG) [NÓI], [HÌNH].
- **Entry**: Vào lệnh Buy tại giá đóng cửa của cây nến xuyên thủng FVG [NÓI], [HÌNH].
- **SL / TP**: SL đặt dưới đáy râu nến thấp nhất vừa tạo; TP đặt tại đỉnh Swing High phía trên. Tỷ lệ R:R đo được trên chart vượt mức 2:1 [HÌNH].

### Ví dụ 6: Setup Entry Model 2 & 3 - CISD và MSS + FVG (08:30 - 09:28)
- **Mốc thời gian**: 08:30 - 09:28.
- **Bối cảnh**: Sau khi quét thanh khoản (Liquidity Sweep) tại vùng hỗ trợ quan trọng [HÌNH].
- **Mô hình CISD**: Trước đó có một chuỗi các cây nến giảm liên tiếp áp đảo. Ngay sau đó xuất hiện lực mua cực mạnh nuốt trọn (engulf) toàn bộ cụm nến giảm này -> Cho phép vào lệnh Buy ngay lập tức [NÓI], [HÌNH].
- **Mô hình MSS + FVG**: Nhịp tăng đó đồng thời phá vỡ đỉnh cấu trúc gần nhất (structural break) và để lại một FVG tăng lớn xuyên qua đỉnh cũ -> Điểm vào lệnh Buy tiếp theo là khi giá retrace nhẹ về FVG này [HÌNH].
- **SL / TP**: SL tại đáy thấp nhất; TP tại đỉnh HTF mục tiêu [HÌNH].

---

## 6. Tips, Tricks & Cảnh báo
- **Mẹo lọc tín hiệu giả**: Nếu giá chạm vào vùng thanh khoản nhưng nến sau đó không tạo được FVG mới, hãy cảnh giác vì giá có xu hướng quay lại quét đỉnh/đáy đối diện mà không đảo chiều theo kỳ vọng [NÓI].
- **Mẹo gồng lệnh / nhồi lệnh**: Sau khi setup đảo chiều tăng đã kích hoạt, nếu giá có những nhịp nhúng xuống dưới đáy tạm thời thì đừng hoảng sợ; đó hầu hết là các pha thao túng phụ (mini-manipulation) để tiếp tục đẩy giá lên [NÓI].
- **Cảnh báo bẫy tâm lý**: Rất nhiều trader thấy giá đi ngang (consolidation) là vội vàng vào lệnh sớm. Nhà cái luôn thích quét sạch SL dưới các vùng đi ngang này trước khi chạm vào HTF FVG rồi mới đảo chiều thật [NÓI].
- **Thói quen kỷ luật**: "Without an entry model, everything else is just theory" (Không có mô hình vào lệnh cụ thể, mọi kiến thức khác chỉ là lý thuyết suông) [HÌNH].

---

## 7. Quản trị rủi ro & Ma trận khung thời gian
- **Tỷ lệ R:R bắt buộc**: Tối thiểu 2:1 cho mọi vị thế giao dịch [NÓI], [HÌNH].
- **Nguyên tắc dừng lỗ**: Luôn neo Stop Loss tại điểm cực trị (đáy thấp nhất đối với lệnh Buy) do pha thao túng tạo ra, không đặt SL lơ lửng giữa chừng [NÓI], [HÌNH].
- **Ma trận đồng bộ khung thời gian (Bắt buộc tuân thủ)** [HÌNH], [NÓI]:
  - Key Level khung **Weekly** (Tuần) -> Tìm tín hiệu Entry trên khung **4 Hour**.
  - Key Level khung **Daily** (Ngày) -> Tìm tín hiệu Entry trên khung **1 Hour**.
  - Key Level khung **4 Hour** -> Tìm tín hiệu Entry trên khung **15 Minute**.
  - Key Level khung **1 Hour** -> Tìm tín hiệu Entry trên khung **5 Minute**.
  - Key Level khung **15 Minute** -> Tìm tín hiệu Entry trên khung **1 Minute**.

---

## 8. Đặc tả logic cho LLM / Bot

Quy tắc thuật toán hóa hệ thống (trình bày cho kịch bản BUY / LONG; kịch bản SELL / SHORT mang tính đối xứng hoàn toàn):

- ĐIỀU KIỆN BỐI CẢNH (HTF CONTEXT)
  - Xác định cặp khung thời gian đồng bộ `HTF` và `LTF` theo bảng chuẩn: `(Weekly, 4H)`, `(Daily, 1H)`, `(4H, 15m)`, `(1H, 5m)`, `(15m, 1m)`.
  - Quét tìm Key Level trên `HTF`:
    - `HTF_Key_Level` = `HTF_FVG` (Internal Range Liquidity) HOẶC `HTF_Swing_Low` (External Range Liquidity).
  - Điều kiện kích hoạt bối cảnh:
    - `Price_Action` trên `HTF` chạm vào `HTF_Key_Level`.
    - Nếu KHÔNG chạm: `Status = NO_TRADE` (Quy tắc "No key level tap = No Trade").

- ĐIỀU KIỆN LỌC & THAO TÚNG TRÊN LTF (MANIPULATION FILTER)
  - Khi giá chạm `HTF_Key_Level`, chuyển sang quan sát trên `LTF`.
  - Kiểm tra điều kiện quét thanh khoản (Liquidity Sweep):
    - Giá tạo đáy mới thấp hơn đáy cũ trên `LTF` nhưng giá đóng cửa nến `Close` KHÔNG nằm dưới đáy cũ (`Low_sweep < Previous_Low` VÀ `Close > Previous_Low`).
  - Đánh dấu mức giá thấp nhất của nhịp quét: `Lowest_Low = min(Low)`.

- TÍN HIỆU KÍCH HOẠT VÀO LỆNH (CHỌN 1 TRONG 3 TRIGGER TRÊN LTF)
  - Mô hình 1: Inverted FVG (`IFVG_Trigger`)
    - Tìm một `Bearish_FVG` gần nhất hình thành trong nhịp giảm vừa qua.
    - Điều kiện kích hoạt: Xuất hiện một cây nến tăng có `Close > Bearish_FVG_Top`.
    - `Entry_Price` = Giá `Close` của cây nến phá vỡ FVG đó.
  - Mô hình 2: Change in State of Delivery (`CISD_Trigger`)
    - Xác định chuỗi nến giảm liên tiếp kiểm soát trước cú quét (`Consecutive_Down_Candles`).
    - Điều kiện kích hoạt: Nến tăng mới xuất hiện có giá `Close` đóng vượt lên trên mức giá mở cửa của cây nến giảm đầu tiên trong chuỗi (`Close > First_Down_Candle_Open`).
    - `Entry_Price` = Giá `Close` khi hoàn tất mô hình nhấn chìm (engulf).
  - Mô hình 3: Market Structure Shift + FVG (`MSS_Trigger`)
    - Xác định `Recent_Swing_High` theo quy tắc 3 nến (`High[i-1] < High[i]` VÀ `High[i+1] < High[i]`).
    - Điều kiện: Nến tăng phá vỡ dứt khoát với `Close > Recent_Swing_High` ĐỒNG THỜI tạo ra `Bullish_FVG` mới (`Low[i+2] > High[i]`).
    - `Entry_Price` = Limit tại biên trên của `Bullish_FVG` khi giá retrace.

- ĐIỀU KIỆN VÀO LỆNH & QUẢN TRỊ RỦI RO (ORDER EXECUTION)
  - `Stop_Loss` = `Lowest_Low` (đáy râu thấp nhất của pha thao túng).
  - `Take_Profit` = `HTF_Recent_Swing_High` (hoặc mức đỉnh thất bại `Failed_High`).
  - Kiểm tra tỷ lệ R:R:
    - `Risk` = `Entry_Price - Stop_Loss`.
    - `Reward` = `Take_Profit - Entry_Price`.
    - Điều kiện lọc: NẾU `(Reward / Risk) < 2.0` THÌ HỦY LỆNH (`Cancel_Trade`).
    - NẾU `(Reward / Risk) >= 2.0` THÌ KÍCH HOẠT LỆNH BUY.

- QUẢN LÝ LỆNH ĐANG CHẠY (POSITION MANAGEMENT)
  - NẾU giá tiếp tục tạo cấu trúc tăng và có nhịp nhúng nhẹ tạo đáy mới `New_Local_Low` cao hơn `Stop_Loss`:
    - Cho phép dời `Stop_Loss` lên dưới `New_Local_Low` để giảm thiểu rủi ro.

---

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Quy tắc Entry IFVG**: Tác giả vừa nói vào lệnh ngay khi cây nến đóng cửa vượt qua IFVG, nhưng trên hình vẽ minh họa có hiển thị nhịp test lại vùng IFVG trước khi tăng mạnh. Video không nêu rõ ưu tiên vào lệnh Market ngay hay đặt lệnh Limit chờ retest [NÓI], [HÌNH].
- **Khối lượng giao dịch (Risk %)**: Tác giả khoe mức lợi nhuận lớn ($41,100/ngày và tài khoản tăng hơn $123,000 trong 1 tháng) nhưng hoàn toàn KHÔNG đề cập đến tỷ lệ rủi ro trên mỗi lệnh (% risk per trade) hay số lot cụ thể sử dụng [HÌNH].
- **Độ rộng FVG**: Video không quy định độ lớn tối thiểu (tính theo pip hay tick) của một FVG hợp lệ để tránh tín hiệu FVG quá nhỏ gây nhiễu trên khung thời gian thấp (như 1m/5m) [VIDEO KHÔNG ĐỀ CẬP].

---

## 10. Thông tin khác
- **Thống kê / Bằng chứng giao dịch của tác giả**:
  - Giao dịch thực tế ngày 11/05/2023 đạt lợi nhuận +$41,100 trong một ngày nhờ mô hình PO3 [HÌNH].
  - Hiển thị lợi nhuận tài khoản: Giao dịch Short NQM5 đạt các mốc +$16,786.50 và +$17,365.50; tổng biến động lợi nhuận trong 1 tháng đạt +$123,822.89 [HÌNH] (Các số liệu này do tác giả cung cấp trên video, chưa được kiểm chứng độc lập).
- **Trích dẫn đáng chú ý**:
  - "Price moves like a magnet from one liquidity pool to the next" (Giá di chuyển như một thanh nam châm từ vùng thanh khoản này sang vùng thanh khoản khác) [HÌNH].
  - "No key level tap = No Trade" (Không chạm vùng giá quan trọng thì không có giao dịch) [HÌNH].
  - "Without an entry model, everything else is just theory" (Nếu thiếu một mô hình vào lệnh cụ thể, mọi thứ còn lại chỉ là lý thuyết suông) [HÌNH].