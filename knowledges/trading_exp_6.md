---
title: "Những Khung Giờ Giá Hay Quét SL Trong Ngày Và Cách Xử Lý Lệnh Limit"
source_author: "Thắng (xưng tên 'em Thắng' ở cuối video)"
video_duration: "01:26"
video_type: ["Price Action / Key Level / Cấu trúc đỉnh đáy / Mô hình nến, mô hình giá", "SMC / ICT (Liquidity, FVG/Imbalance, OB, Breaker, BOS/CHOCH, Inducement, Killzone, Premium/Discount)", "Quản lý vốn, quản trị rủi ro, tâm lý giao dịch, nhật ký giao dịch, kỷ luật", "Kiến thức nền cho người mới"]
markets: ["XAUUSD (Gold Spot / U.S. Dollar hiển thị một phần ở góc trái trên biểu đồ)", "Giao dịch trong ngày (Intraday) nói chung"]
timeframes_htf: ["KHÔNG RÕ"]
timeframes_ltf: ["Khung thời gian nhỏ (tác giả nhắc tới nhưng không nêu số phút cụ thể)"]
tools: ["TradingView", "2 đường trung bình động (Moving Average) màu xanh dương và màu cam trên biểu đồ (không được nhắc tới trong lời nói)"]
tags: ["Stop Loss", "Quét SL", "Quét thanh khoản", "Lệnh Limit", "Khung giờ giao phiên", "Intraday Trading", "Nến rút chân", "Breakeven", "SL hòa"]
extraction_confidence: "Cao – Âm thanh rõ ràng, nội dung ngắn gọn và tập trung vào một chủ đề cụ thể, tuy nhiên biểu đồ bị cắt một phần thông tin khung thời gian và trục giá."
---

# Những Khung Giờ Giá Hay Quét SL Trong Ngày Và Cách Xử Lý Lệnh Limit

## 0. TL;DR
- Nhiều trader (cả người mới lẫn người giao dịch lâu năm) thường mắc sai lầm vào lệnh sai thời điểm, đặc biệt là khi đặt lệnh Limit trong ngày [NÓI].
- Có 3 khung giờ chính trong ngày giá dễ quét SL nhất do đặc thù giao phiên: 8:00 sáng, 12:30 trưa và 8:30 tối [NÓI].
- Tại các khung giờ giao phiên này, giá thường có hành vi "quét hai đầu" hoặc "quét hẳn một đầu" (quét thanh khoản / đá SL hoặc đá SL hòa) trước khi chạy theo chiều ngược lại lên TP [NÓI].
- Giải pháp: Né đặt lệnh Limit tại 3 khung giờ trên; thay bằng việc canh vào lệnh bằng tay (Market) khi giá đã quét SL và xuất hiện các cây nến rút chân ở khung thời gian nhỏ [NÓI].

---

## 1. Tổng quan
- **Mục tiêu / vấn đề video giải quyết**: Khắc phục lỗi vào lệnh sai thời điểm (đặc biệt là lệnh Limit và thói quen dời SL về hòa vốn) dẫn đến việc bị giá quét SL hoặc đá SL hòa trước khi chạy đúng hướng về TP [NÓI].
- **Đối tượng phù hợp**: Cả người mới (hay mắc phải) và người đã giao dịch lâu năm nhưng không để ý, áp dụng cho người giao dịch trong ngày (intraday) [NÓI].
- **Thị trường, sản phẩm, khung thời gian, phiên giao dịch áp dụng**:
  - Thị trường / Sản phẩm: Giao dịch trong ngày nói chung [NÓI]. Trên màn hình biểu đồ minh họa là sản phẩm `Gold Spot / U.S. Do...` (XAUUSD) với mức giá Bid/Ask hiển thị ở góc trái trên khoảng `4,881.140` – `4,898.260` [HÌNH].
  - Khung thời gian: Không nêu khung thời gian chính trên biểu đồ (bị che khuất) [HÌNH]; tác giả chỉ đề cập đến việc quan sát "khung thời gian nhỏ" khi canh nến rút chân để vào lệnh tay [NÓI].
  - Phiên giao dịch / Khung giờ: Tập trung vào các thời điểm giao phiên trong ngày gồm 8:00 sáng, 12:30 trưa, và 8:30 tối [NÓI] (Múi giờ: VIDEO KHÔNG ĐỀ CẬP, nhưng theo ngữ cảnh buổi sáng/trưa/tối bằng tiếng Việt là giờ Việt Nam GMT+7 [SUY LUẬN]).
- **Công cụ & thiết lập chỉ báo**:
  - Biểu đồ nến Nhật trên nền tảng TradingView [HÌNH].
  - Trên biểu đồ có hiển thị 2 đường chỉ báo dạng đường trung bình (một đường màu cam bám sát giá hơn và một đường màu xanh dương mượt hơn), kèm con số `8` ở góc trên bên trái dưới tên mã, nhưng tác giả hoàn toàn không đề cập hay sử dụng 2 đường này trong bài giảng [HÌNH].

---

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Luận điểm cốt lõi theo lời tác giả**:
  - Theo thống kê cá nhân của tác giả, trong ngày có 3 khung giờ giao phiên chính là 8:00 sáng, 12:30 trưa và 8:30 tối [NÓI].
  - Vì là thời điểm giao phiên nên hành vi giá thường "quét hai đầu" hoặc "quét hẳn một đầu" (quét thanh khoản / quét một phần SL) trước khi đi theo chiều ngược lại [NÓI].
  - Do cơ chế này, nếu đặt sẵn lệnh Limit tại các khung giờ đó, lệnh rất dễ bị khớp và bị quét SL trước, sau đó giá mới chạy thẳng một mạch lên TP [NÓI].
  - Tương tự, với những người đã có vị thế từ trước và có thói quen dời SL hòa về điểm Entry (Breakeven), hành vi quét tại khung giờ này sẽ "đá SL hòa" rồi giá mới đi tiếp [NÓI].
- **Điều kiện thị trường phù hợp / KHÔNG phù hợp**:
  - Áp dụng cho giao dịch trong ngày (intraday) tại các mốc thời gian giao phiên [NÓI].
  - Các điều kiện xu hướng hay biên độ thị trường khác: VIDEO KHÔNG ĐỀ CẬP.
- **Giả định ngầm của phương pháp**:
  - Hành vi quét thanh khoản tại các giờ giao phiên (8:00, 12:30, 20:30) lặp lại đủ thường xuyên để việc bỏ lệnh Limit và chờ xác nhận nến rút chân mang lại lợi thế tốt hơn [SUY LUẬN: dựa trên việc tác giả khuyên né toàn bộ lệnh Limit ở các giờ này].

---

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **Lệnh Limit** | Lệnh chờ đặt sẵn tại một mức giá dự kiến đảo chiều/hồi về [NÓI]. | Không hiển thị công cụ vẽ lệnh trên chart; chỉ được nhắc bằng lời [NÓI]. |
| **Khung giờ giao phiên** | 3 mốc thời gian trong ngày gồm: 8:00 sáng, 12:30 trưa, 8:30 tối [NÓI]. | Trên chart được đánh dấu bằng các nhãn chữ tại các đỉnh/đáy: `Quét SL Tối` (màu đỏ), `Quét SL Sáng` (màu xanh ngọc), `Quét SL Trưa` (màu cam) và đường gióng dọc mờ [HÌNH]. |
| **Quét hai đầu / Quét hẳn một đầu / Quét thanh khoản** | Hành vi giá đánh thủng qua vùng đỉnh hoặc đáy trước đó để chạm vào vùng đặt SL của các trader rồi mới đảo chiều đi ngược lại [NÓI]. | Giá tạo các nhịp chọc râu hoặc đóng nến vượt qua đỉnh/đáy cục bộ liền trước tại đúng các mốc giờ giao phiên rồi lập tức đảo chiều mạnh [HÌNH]. |
| **SL hòa (Breakeven)** | Điểm dừng lỗ được dời về đúng mức giá vào lệnh (Entry) sau khi lệnh đã chạy [NÓI]. | Giá lùi về chạm lại vùng đáy/vùng vào lệnh trước đó trước khi tăng tiếp [NÓI, HÌNH]. |
| **Canh vào tay** | Không đặt lệnh chờ Limit tự động mà quan sát trực tiếp để vào lệnh thủ công khi có tín hiệu nến [NÓI]. | VIDEO KHÔNG ĐỀ CẬP thao tác cụ thể trên phần mềm. |
| **Cây nến rút chân** | Nến có bóng nến (râu nến) dài thể hiện sự từ chối giá sau khi đã quét SL ở khung thời gian nhỏ [NÓI]. | Các cây nến tại vùng đáy `Quét SL Trưa` và đỉnh `Quét SL Sáng` có râu chọc qua cản rồi đóng cửa rút ngược lại [HÌNH]. |

---

## 4. Hệ thống quy tắc

### 4.1 Điều kiện tiên quyết / Confluence
- [ ] Đang giao dịch trong ngày (Intraday) [NÓI].
- [ ] Thời gian hiện tại rơi vào một trong 3 khung giờ giao phiên: `08:00` sáng, `12:30` trưa, hoặc `20:30` tối [NÓI].

### 4.2 Xác định bối cảnh & hướng (Bias)
- Cách xác định xu hướng chính hoặc vùng cản để đợi giá: VIDEO KHÔNG ĐỀ CẬP (tác giả chỉ mặc định tình huống người giao dịch đã có sẵn ý định canh lệnh, ví dụ canh Long vào buổi trưa) [NÓI].

### 4.3 Tín hiệu kích hoạt (Trigger)
1. Giá thực hiện hành vi quét SL / quét thanh khoản (quét qua vùng đặt SL dự kiến hoặc vùng đáy/đỉnh trước đó) trong khung giờ giao phiên [NÓI, HÌNH].
2. Xuất hiện các "cây nến rút chân" ở trong khung thời gian nhỏ sau khi đã quét SL [NÓI].

### 4.4 Entry (Loại lệnh & Vị trí)
- **Quy tắc cứng (theo khuyến nghị của tác giả)**: Không sử dụng lệnh Limit tại 3 khung giờ 8:00 sáng, 12:30 trưa và 8:30 tối [NÓI].
- **Loại lệnh thay thế**: "Canh vào tay" (vào lệnh trực tiếp bằng tay sau khi có xác nhận) [NÓI].
- **Vị trí vào lệnh**: Vào lệnh tại những cây nến rút chân ở khung thời gian nhỏ sau khi giá đã quét SL [NÓI].

### 4.5 Stop Loss (SL)
- Quy tắc đặt SL cụ thể cho lệnh vào tay (đặt cách râu nến bao nhiêu pip/giá): VIDEO KHÔNG ĐỀ CẬP.
- **Lưu ý về dời SL hòa**: Tại khung giờ giao phiên (như 12:30 trưa), nếu đã vào lệnh trước đó và dời SL hòa về Entry thì rất dễ bị giá quay lại "đá SL hòa" rồi mới đi tiếp [NÓI].

### 4.6 Take Profit (TP) / Quản lý lệnh
- Quy tắc xác định điểm TP, tỷ lệ R:R, chốt lời từng phần: VIDEO KHÔNG ĐỀ CẬP (tác giả chỉ mô tả hiện tượng sau khi quét SL thì giá "chạy thẳng một mạch lên TP") [NÓI].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- **Không đặt lệnh chờ Limit**: Tuyệt đối né đặt sẵn lệnh Limit trong các khung giờ 8:00 sáng, 12:30 trưa và 8:30 tối [NÓI].
- Điều kiện hủy kèo khi canh tay: VIDEO KHÔNG ĐỀ CẬP.

---

## 5. Case Study / Ví dụ chart

### 5.1 Tổng quan 3 điểm quét SL trên biểu đồ trong ngày
- **Mốc thời gian trong video**: `00:00` – `00:33` và `00:56` – `01:26`.
- **Sản phẩm & Khung thời gian**: `Gold Spot / U.S. Do...` (XAUUSD), khung thời gian: KHÔNG RÕ [HÌNH].
- **Bối cảnh & Những gì hiển thị trên chart**:
  - Biểu đồ đánh dấu 3 vị trí đảo chiều lớn trong ngày bằng 3 nhãn chú thích [HÌNH]:
    1. Nhãn màu đỏ `Quét SL Tối` ở đáy bên trái màn hình, nơi giá giảm mạnh tạo râu dưới rồi bật tăng mạnh [HÌNH].
    2. Nhãn màu xanh ngọc `Quét SL Sáng` ở đỉnh cao nhất giữa màn hình, nơi giá tăng vọt lên tạo đỉnh nhọn rồi sập mạnh xuống dưới cả 2 đường MA [HÌNH].
    3. Nhãn màu cam `Quét SL Trưa` ở vùng đáy bên phải màn hình, nơi giá giảm xuống, tạo nhịp nhúng xuống dưới đáy nhỏ liền trước rồi bật tăng trở lại [HÌNH].
- **Mục đích minh họa**: Minh họa trực quan cho thống kê 3 khung giờ trong ngày (tối, sáng, trưa) mà giá thường quét SL một đầu trước khi đi mạnh theo chiều ngược lại [NÓI, HÌNH].

### 5.2 Ví dụ chi tiết: Pha quét SL buổi trưa (12:30)
- **Mốc thời gian trong video**: `00:33` – `00:55`.
- **Sản phẩm, khung thời gian, hướng lệnh**: Sản phẩm `Gold Spot / U.S. Do...` [HÌNH], khung thời gian: KHÔNG RÕ, hướng lệnh minh họa: Long (Mua) [NÓI].
- **Bối cảnh trước setup**: Sau nhịp giảm mạnh từ đỉnh `Quét SL Sáng`, giá tạo một vùng đáy đi ngang ngắn hạn ở phía dưới hai đường MA [HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Từ `00:34` đến `00:38`, tác giả rê chuột chỉ vào vùng nhãn màu cam `Quét SL Trưa` và giải thích rằng trước khi đi lên, giá đã có hành vi quét thanh khoản trước rồi mới đi lên [NÓI, HÌNH].
  - Từ `00:39` đến `00:55`, biểu đồ được phóng to vào khu vực `Quét SL Trưa` [HÌNH]:
    - Tác giả chỉ chuột vào vùng đáy trước đó (khoảng `00:48` – `00:50`) nơi các trader thường vào lệnh Long hoặc đặt lệnh chờ Long [NÓI, HÌNH].
    - Ngay tại cột mốc có đường kẻ dọc mờ và nhãn `Quét SL Trưa`, xuất hiện một cụm nến giảm đỏ tiếp nối bởi cây nến xanh có râu dưới quét thủng nhẹ qua các đáy liền kề bên trái, sau đó đóng cửa rút lên và tạo chuỗi nến xanh tăng mạnh vượt lên trên hai đường MA [HÌNH].
- **Entry / SL / TP cụ thể**: Không nêu mức giá số học cụ thể (trục giá bên phải bị cắt khỏi khung hình) [HÌNH].
- **Kết quả và bài học tác giả rút ra**:
  - Nếu đặt lệnh Long (Limit) sớm ở vùng đáy hoặc vào lệnh ở đáy trước rồi kéo SL hòa về điểm Entry, nhịp nhúng lúc 12:30 trưa sẽ quét một phần SL hoặc "đá SL hòa" trước khi giá tiếp tục đi lên mạnh [NÓI].
  - Bài học: Phải né lệnh Limit ở khung giờ này và đợi giá quét SL xong, xuất hiện nến rút chân ở khung nhỏ mới vào lệnh bằng tay [NÓI].
- **Minh họa cho quy tắc**: Quy tắc 4.3, 4.4 và 4.7 (ví dụ thuận về hành vi thị trường và phản ví dụ cho việc đặt lệnh Limit / kéo SL hòa sai thời điểm) [NÓI].

---

## 6. Tips, Tricks & Cảnh báo
- **Sai lầm phổ biến cần tránh**: Vào lệnh sai thời điểm (đặc biệt là treo lệnh Limit) tại các giờ giao phiên là lỗi không chỉ người mới mà cả trader lâu năm không để ý vẫn dính [NÓI].
- **Cảnh báo về 3 khung giờ nhạy cảm**: Luôn cảnh giác vào lúc 8:00 sáng, 12:30 trưa và 8:30 tối vì đây là lúc giá hay "quét hai đầu" hoặc "quét hẳn một đầu" [NÓI].
- **Cảnh báo về thói quen kéo SL hòa (Breakeven)**: Thói quen dời SL về điểm Entry ngay trước hoặc trong khung giờ giao phiên (như 12:30 trưa) rất dễ khiến lệnh bị đá hòa vốn ngay trước khi giá chạy thật [NÓI].
- **Mẹo lọc tín hiệu nhiễu / thay đổi cách vào lệnh**: Thay vì đặt lệnh chờ Limit ở các khung giờ trên, hãy chuyển sang "canh vào tay", đợi quá trình quét SL diễn ra xong và xuất hiện các cây nến rút chân ở khung thời gian nhỏ rồi mới vào [NÓI].

---

## 7. Quản trị rủi ro & Tâm lý
- Video không đề cập đến công thức tính khối lượng (lot), % rủi ro mỗi lệnh hay giới hạn lỗ ngày/tuần.
- Về quản lý vị thế và tâm lý thực chiến: Tác giả nhấn mạnh việc kiểm soát điểm đặt lệnh (không phó mặc cho lệnh Limit trong giờ giao phiên) và lưu ý rủi ro của thói quen kéo SL về hòa vốn quá sớm tại các mốc giờ nhạy cảm [NÓI].

---

## 8. Đặc tả logic cho LLM / Bot

Quy tắc trong video mang tính chất **Bộ lọc thời gian (Time Filter)** và **Điều kiện chuyển đổi phương thức vào lệnh (Order Execution Mode)** hơn là một hệ thống giao dịch hoàn chỉnh độc lập. Dưới đây là logic mã hóa phần quy tắc có trong video (áp dụng đối xứng cho cả `LONG` và `SHORT`):

- **BIẾN ĐẦU VÀO & THAM SỐ**:
  - `current_time`: Thời gian hiện tại trong ngày [NÓI]
  - `timezone`: `UNSPECIFIED_IN_VIDEO` (Suy luận là `UTC+7` theo ngữ cảnh người nói tại Việt Nam [SUY LUẬN])
  - `high_risk_sweep_times`: Danh sách các mốc giờ giao phiên gồm `08:00`, `12:30`, `20:30` [NÓI]
  - `time_window_buffer`: `UNSPECIFIED_IN_VIDEO` (Khoảng thời gian trước/sau mỗi mốc giờ cần né lệnh Limit)
  - `ltf_timeframe`: `UNSPECIFIED_IN_VIDEO` (Khung thời gian nhỏ dùng để canh nến rút chân)

- **ĐIỀU KIỆN BỐI CẢNH & LỌC THỜI GIAN (TIME FILTER)**:
  - `IF` `trading_style == INTRADAY` `AND` `current_time` nằm trong vùng `high_risk_sweep_times` (+/- `time_window_buffer`):
    - `SET` `allow_limit_orders = FALSE` (Hủy hoặc không đặt lệnh chờ Limit) [NÓI]
    - `SET` `execution_mode = MANUAL_CONFIRMATION` (Chuyển sang chế độ chờ xác nhận sau quét) [NÓI]
    - `WARNING`: Nếu đang có vị thế mở với `SL == entry_price` (Breakeven), cảnh báo nguy cơ cao bị quét `SL` hòa [NÓI]

- **TRIGGER & ENTRY (KHI Ở CHẾ ĐỘ CHỜ XÁC NHẬN)**:
  - **Đối với lệnh LONG**:
    - `IF` `execution_mode == MANUAL_CONFIRMATION`:
      - Điều kiện 1 (`liquidity_sweep_down`): `SUBJECTIVE:` Giá giảm xuống quét qua vùng đáy cục bộ hoặc vùng đặt SL của phe Mua trước đó [NÓI, HÌNH]
      - Điều kiện 2 (`rejection_candle_ltf`): `SUBJECTIVE:` Xuất hiện các cây nến rút chân (râu dưới dài, đóng cửa rút lên) trên khung `ltf_timeframe` ngay sau khi quét [NÓI]
      - `IF` `liquidity_sweep_down == TRUE` `AND` `rejection_candle_ltf == TRUE`:
        - `EXECUTE` lệnh `LONG` (Market / vào tay) tại cây nến rút chân [NÓI]
  - **Đối với lệnh SHORT** (Đối xứng theo nguyên lý "quét hai đầu / quét một đầu" và ví dụ `Quét SL Sáng` trên chart):
    - `IF` `execution_mode == MANUAL_CONFIRMATION`:
      - Điều kiện 1 (`liquidity_sweep_up`): `SUBJECTIVE:` Giá tăng vọt quét qua vùng đỉnh cục bộ hoặc vùng đặt SL của phe Bán trước đó [NÓI, HÌNH]
      - Điều kiện 2 (`rejection_candle_ltf`): `SUBJECTIVE:` Xuất hiện các cây nến rút chân trên khung `ltf_timeframe` ngay sau khi quét [NÓI]
      - `IF` `liquidity_sweep_up == TRUE` `AND` `rejection_candle_ltf == TRUE`:
        - `EXECUTE` lệnh `SHORT` (Market / vào tay) tại cây nến rút chân [NÓI]

- **SL, TP & ĐIỀU KIỆN HỦY**:
  - `stop_loss_placement`: `UNSPECIFIED_IN_VIDEO`
  - `take_profit_placement`: `UNSPECIFIED_IN_VIDEO`
  - `invalidation_condition`: `UNSPECIFIED_IN_VIDEO`

---

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Thiếu khung thời gian cụ thể trên biểu đồ**: Góc trên bên trái của biểu đồ bị cắt khuất tên khung thời gian hiện tại; khi tác giả khuyên vào lệnh ở "khung thời gian nhỏ", tác giả cũng không nêu rõ là M1, M5 hay M15 [NÓI, HÌNH].
- **Thiếu độ rộng của vùng giờ cần né (Time Window)**: Tác giả nêu 3 mốc giờ `8:00 sáng`, `12:30 trưa`, `8:30 tối` [NÓI], nhưng không nói rõ cần hủy/né lệnh Limit trong khoảng bao nhiêu phút trước và sau các mốc giờ này (ví dụ: từ 12:15 đến 12:45 hay cả tiếng đồng hồ).
- **Thiếu thông số của 2 đường Moving Average trên biểu đồ**: Trên màn hình có 2 đường MA màu cam và xanh dương (kèm số `8` ở góc trái trên) [HÌNH], nhưng tác giả không giải thích chúng là EMA hay SMA chu kỳ bao nhiêu và có vai trò gì trong việc xác định xu hướng hay không.
- **Thiếu quy tắc đặt SL và TP sau khi vào tay**: Khi vào lệnh tại cây nến rút chân ở khung nhỏ, video không chỉ rõ đặt SL ngay dưới râu nến rút chân hay cách một khoảng bao nhiêu, cũng như cách đo TP.
- **Câu hỏi cần làm rõ trước khi áp dụng / bot hóa**:
  1. Khoảng đệm thời gian (buffer) quanh các mốc `08:00`, `12:30`, `20:30` (theo giờ GMT+7) là bao nhiêu phút?
  2. Khung thời gian chuẩn để xác định vùng thanh khoản bị quét và khung thời gian nhỏ (`LTF`) để tìm nến rút chân cụ thể là khung nào?
  3. Tiêu chí định lượng cho "cây nến rút chân" (tỷ lệ râu nến so với thân nến) và vị trí đặt SL/TP sau khi vào lệnh là gì?

---

## 10. Thông tin khác
- **Công cụ, nền tảng, sàn giao dịch được nhắc tới**:
  - Biểu đồ phân tích: TradingView [HÌNH].
  - Sàn giao dịch: Exness [NÓI, HÌNH].
- **Kết quả/thống kê tác giả nêu**: Tác giả cho biết 3 khung giờ dễ quét SL nhất là kết quả từ việc "như mình thống kê ở trong ngày" [NÓI] (không công bố bảng số liệu thống kê chi tiết hay cỡ mẫu kiểm chứng).
- **Quảng cáo / Upsell**:
  - Chữ chạy trên màn hình lúc `00:10` – `00:14`: "Trade Exness mà chưa được nhận hoàn phí LH mình hỗ trợ nhé!" [HÌNH].
  - Lời nói cuối video (`01:17` – `01:21`): Tác giả (xưng là "em Thắng") mời những ai đang giao dịch trên sàn Exness mà chưa cài hoàn phí (rebate/backcom) thì liên hệ để được hỗ trợ, đồng thời kêu gọi lưu video và follow kênh [NÓI].
- **Trích dẫn nguyên văn đáng giữ**:
  - "Trong ngày nó sẽ có 3 cái khung giờ chính dễ quét SL nhất, đó chính là 8 giờ sáng này, 12 giờ 30 trưa này, và 8 giờ 30 tối. Lý do là bởi vì đây là những cái khung giờ giao phiên, chính vì vậy nên là giá thường có cái hành vi là quét hai đầu hoặc là quét hẳn một đầu trước khi nó đi theo cái chiều ngược lại." [NÓI]
  - "Tất cả những cái lệnh Limit các bạn né những cái khung giờ này ra cho mình nhá, và thay cái lệnh Limit đấy bằng việc là chúng ta canh vào tay. Nếu mà giá quét SL rồi và sau đấy có những cây nến rút chân ở trong khung thời gian nhỏ chẳng hạn, thì chúng ta có thể vào lệnh ở những cây nến rút chân đấy nhá." [NÓI]
- **Ghi chú của người trích xuất**:
  - [SUY LUẬN] Theo giờ Việt Nam (GMT+7), mốc 8:00 sáng tương ứng với thời điểm mở cửa các thị trường chứng khoán lớn tại châu Á (Tokyo/Singapore/Hồng Kông), 12:30 trưa là giai đoạn nghỉ trưa phiên Á chuẩn bị chuyển giao sang tiền phiên Âu (Pre-London), và 8:30 tối (20:30) là thời điểm mở cửa phiên Mỹ (New York) và thường trùng giờ công bố tin tức kinh tế Mỹ (vào mùa Đông là 20:30, mùa Hè là 19:30). Khi áp dụng cho bot tự động, cần lưu ý sự thay đổi giờ mùa Hè / mùa Đông (DST) của phiên Âu và phiên Mỹ so với giờ Việt Nam.