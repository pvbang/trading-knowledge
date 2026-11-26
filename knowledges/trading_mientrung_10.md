---
title: "Chiến lược Scalping Vàng bắt đảo chiều: Công thức CHoCH + OTE (Fibonacci)"
source_author: "TradingMienTrung"
video_duration: "01:38"
video_type: ["SMC / ICT", "Fibonacci", "Price Action / Key Level / Cấu trúc đỉnh đáy"]
markets: ["XAUUSD"]
timeframes_htf: ["VIDEO KHÔNG ĐỀ CẬP"]
timeframes_ltf: ["1H"]
tools: ["Fibonacci Retracement (tùy chỉnh OTE)", "AI của TradingView"]
tags: ["Scalping", "XAUUSD", "CHoCH", "OTE", "Fibonacci", "Đảo chiều", "SMC", "ICT", "TradingMienTrung"]
extraction_confidence: "Cao – Video ngắn, hình ảnh bảng thông số và mức giá trên biểu đồ rõ nét, lời nói khớp với thao tác vẽ."
---

# Chiến lược Scalping Vàng bắt đảo chiều: Công thức CHoCH + OTE (Fibonacci)

## 0. TL;DR
- Video hướng dẫn công thức bắt đảo chiều để scalping Vàng (XAUUSD): Đợi cấu trúc tạo `CHoCH` -> Kéo Fibonacci tìm vùng `OTE` -> Đợi giá hồi về `OTE` và vào lệnh[cite: 1].
- Áp dụng đối xứng cho cả hai chiều: xu hướng tăng đảo chiều sang giảm (Short) và xu hướng giảm đảo chiều sang tăng (Long)[cite: 1].
- Vùng `OTE` được thiết lập trên công cụ Fibonacci từ mức `0.618` đến `0.79`, trong đó mức `0.705` là mốc quan trọng nhất (dùng làm điểm Entry trên biểu đồ minh họa)[cite: 1].
- Có thể kết hợp đưa công thức này vào công cụ AI trên TradingView để tự động phân tích biểu đồ và xuất tín hiệu giao dịch[cite: 1].

## 1. Tổng quan
- **Mục tiêu video giải quyết**: Cung cấp "giáo án bắt đảo chiều" tinh gọn để scalping Vàng hiệu quả [NÓI][cite: 1].
- **Đối tượng phù hợp**: VIDEO KHÔNG ĐỀ CẬP.
- **Thị trường áp dụng**: Vàng (`XAUUSD`) [NÓI, HÌNH][cite: 1].
- **Khung thời gian**: Lời nói không quy định khung thời gian cố định (chỉ nói có thể yêu cầu AI phân tích trên khung thời gian của TradingView) [NÓI][cite: 1]. Trên màn hình ví dụ AI hiển thị chữ `XAUUSD 1H` [HÌNH][cite: 1].
- **Phiên giao dịch**: VIDEO KHÔNG ĐỀ CẬP.
- **Công cụ & Thiết lập chỉ báo**:
  - Công cụ Fibonacci Retracement (được tác giả đặt tên mẫu là `OTE` trong phần cài đặt của TradingView) [HÌNH][cite: 1].
  - Các mốc Fibonacci được tích chọn hiển thị trong bảng cài đặt (từ `00:45` đến `00:56`) [HÌNH][cite: 1]:
    - `0` (màu xám)[cite: 1]
    - `0.5` (màu xanh lá)[cite: 1]
    - `0.618` (màu xanh lá)[cite: 1]
    - `0.705` (màu đỏ/cam)[cite: 1]
    - `0.79` (màu xanh cổ vịt)[cite: 1]
    - `0.886` (màu cam)[cite: 1]
    - `1` (màu xám)[cite: 1]
  - Tùy chọn hiển thị khác trong bảng cài đặt Fibonacci [HÌNH][cite: 1]: Bật "Đường xu hướng" (nét đứt), Độ rộng đường = `1`, Kéo dài = `Không mở rộng`, bật "Sử dụng một màu" = tắt, bật "Hình nền", bật "Các mức" (`Giá trị`), bật "Các mức giá", Nhãn = `Trái` / `Giữa`, Cỡ chữ = `12`[cite: 1].

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Luận điểm cốt lõi**: Video trình bày dưới dạng công thức thực hành nhanh ("Trend + CHoCH + đợi hồi về OTE + Entry"), không giải thích lý thuyết nền tảng tại sao giá phản ứng ở vùng OTE hay cơ chế thanh khoản đằng sau [NÓI][cite: 1].
- **Điều kiện thị trường phù hợp**: Thị trường đang có xu hướng rõ ràng (Trend tăng hoặc Trend giảm) và bắt đầu xuất hiện tín hiệu đảo chiều cấu trúc (`CHoCH`) [NÓI, HÌNH][cite: 1].
- **Điều kiện KHÔNG phù hợp**: VIDEO KHÔNG ĐỀ CẬP.

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| `CHoCH` | Tín hiệu giá đảo chiều từ xu hướng hiện tại sang hướng ngược lại [NÓI][cite: 1]. | Khi đang trong xu hướng tăng, một nhịp giảm mạnh phá vỡ đáy gần nhất tạo đỉnh mới thấp hơn hoặc phá cấu trúc tăng; ngược lại với xu hướng giảm phá đỉnh gần nhất (được đánh dấu bằng hộp chữ nhật màu đỏ có chữ `CHoCH` hoặc đường kẻ ngang tại mức giá bị phá) [HÌNH][cite: 1]. |
| `OTE` | Vùng canh vào lệnh sau khi kéo Fibonacci trên nhịp sóng tạo `CHoCH`, nằm từ mốc `0.618` đến `0.79`, có mốc quan trọng ở giữa là `0.705` [NÓI][cite: 1]. | Vùng hộp màu xanh lá cây được tô nổi bật giữa mức `0.618` và `0.79` trên công cụ Fibonacci [HÌNH][cite: 1]. |

## 4. Hệ thống quy tắc

### 4.1 Điều kiện tiên quyết / Confluence
- [ ] Xác định được một xu hướng trước đó (Trend tăng hoặc Trend giảm) [NÓI][cite: 1].
- [ ] Giá đảo chiều phá vỡ cấu trúc tạo ra `CHoCH` [NÓI][cite: 1].
- [ ] Đã kéo công cụ Fibonacci trên con sóng vừa tạo `CHoCH` để xác định vùng `OTE` (`0.618` – `0.79`) [NÓI, HÌNH][cite: 1].

### 4.2 Xác định bối cảnh & hướng (Bias)
- **Canh Bán (Short)**: Bối cảnh trước đó là `Trend tăng`, sau đó giá sập xuống tạo `CHoCH` giảm [NÓI, HÌNH][cite: 1].
- **Canh Mua (Long)**: Bối cảnh trước đó là `Trend giảm`, sau đó giá bật tăng mạnh tạo `CHoCH` tăng [NÓI, HÌNH][cite: 1].

### 4.3 Tín hiệu kích hoạt (Trigger)
- Giá hồi ngược trở lại (pullback) chạm vào vùng `OTE` (`0.618` – `0.79`) sau khi đã tạo `CHoCH` [NÓI, HÌNH][cite: 1].

### 4.4 Entry (Điểm vào lệnh)
- **Vị trí nói bằng lời**: Đợi giá quay về vùng `OTE` (`0.618` đến `0.79`), lưu ý mốc quan trọng `0.705` [NÓI][cite: 1].
- **Vị trí chính xác trên hình**: Trong cả các ví dụ vẽ tay và ví dụ AI, điểm đặt lệnh (cạnh giữa của công cụ đo R:R) đều được đặt chính xác tại mức Fibonacci `0.705` [HÌNH][cite: 1].
- **Loại lệnh**: VIDEO KHÔNG ĐỀ CẬP trực tiếp bằng lời (nhưng cách đặt sẵn công cụ R:R tại đúng mốc `0.705` và bảng tín hiệu AI gợi ý đây là lệnh chờ Limit hoặc vào ngay khi chạm vùng OTE) [SUY LUẬN – dựa trên hình vẽ công cụ đo lệnh cố định tại mức 0.705][cite: 1].

### 4.5 Stop Loss (Cắt lỗ)
- **Quy tắc bằng lời**: VIDEO KHÔNG ĐỀ CẬP.
- **Quy tắc trên hình**:
  - Trong Ví dụ 1 (Short) và Ví dụ 2 (Long): Mức Stop Loss của công cụ đo R:R được đặt trùng khít với mốc `1` của Fibonacci (tức ngay tại đỉnh bắt đầu nhịp giảm tạo CHoCH đối với lệnh Short, và ngay tại đáy bắt đầu nhịp tăng tạo CHoCH đối với lệnh Long) [HÌNH][cite: 1].
  - Trong Ví dụ 3 (AI TradingView): Mức Stop Loss đặt cao hơn một chút hoặc trùng quanh vùng đỉnh `1` của Fibonacci [HÌNH][cite: 1].

### 4.6 Take Profit / Quản lý lệnh
- **Quy tắc bằng lời**: VIDEO KHÔNG ĐỀ CẬP.
- **Quy tắc trên hình**:
  - Trong Ví dụ 1 và Ví dụ 2: Mức Take Profit (cạnh dưới/trên của hộp xanh công cụ đo R:R) được kéo vừa khít tới mốc `0` của Fibonacci (tức đáy của con sóng tạo CHoCH giảm trong Ví dụ 1, và đỉnh của con sóng tạo CHoCH tăng trong Ví dụ 2) [HÌNH][cite: 1].
  - Với Entry tại `0.705`, SL tại `1.0` và TP tại `0.0`, tỷ lệ R:R cố định theo cấu trúc Fibonacci này hiển thị trên hình là `2.39` (làm tròn từ $(0.705 - 0) / (1 - 0.705) = 0.705 / 0.295 \approx 2.3898$) [HÌNH, SUY LUẬN – tính toán xác nhận từ thông số trên hình][cite: 1].
  - Quản lý lệnh (dời SL, chốt lời từng phần): VIDEO KHÔNG ĐỀ CẬP.

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- VIDEO KHÔNG ĐỀ CẬP.

## 5. Case Study / Ví dụ chart

### 5.1 Ví dụ 1: Lệnh Short đảo chiều từ Trend tăng (00:00 – 00:24 & 01:00 – 01:13)
- **Mốc thời gian**: Xuất hiện ở đầu video (`00:00` – `00:24`) và lặp lại lúc (`01:00` – `01:13`)[cite: 1].
- **Sản phẩm & Hướng lệnh**: Vàng (`XAUUSD`), lệnh Bán (Short) [NÓI, HÌNH][cite: 1]. Khung thời gian không hiện trên góc chart nhưng đối chiếu mức giá trùng với đoạn sau là `1H` [SUY LUẬN][cite: 1].
- **Bối cảnh trước setup**: Giá đang trong một xu hướng tăng (`TREND TĂNG` được tô vùng xanh lá từ đáy lên đỉnh `4,383.17`), đi ngang tạo vùng đỉnh rồi sập mạnh một cây nến đỏ dài kết hợp các nến giảm tiếp theo phá qua vùng đáy cấu trúc gần nhất quanh `4,317` [HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart**:
  - Đánh dấu nhãn `CHoCH` màu đỏ tại vùng đáy bị phá vỡ [HÌNH][cite: 1].
  - Kéo Fibonacci từ đỉnh `1 (4,383.17)` xuống đáy nhịp giảm `0 (4,219.25)` [NÓI, HÌNH][cite: 1].
  - Các mốc giá Fibonacci cụ thể trên màn hình [HÌNH][cite: 1]:
    - `1`: `4,383.17`[cite: 1]
    - `0.886`: `4,364.48`[cite: 1]
    - `0.79`: `4,348.74`[cite: 1]
    - `0.705`: `4,334.81`[cite: 1]
    - `0.618`: `4,320.54`[cite: 1]
    - `0.5`: `4,301.21`[cite: 1]
    - `0`: `4,219.25`[cite: 1]
  - Tô nổi bật vùng hộp xanh lá có chữ `OTE` nằm giữa mức `0.79 (4,348.74)` và `0.618 (4,320.54)` [HÌNH][cite: 1].
  - Khoanh tròn vùng nến rút râu khi giá hồi lên chạm vào vùng `OTE` và chạm mức `0.705` [HÌNH][cite: 1].
- **Entry / SL / TP cụ thể** (đọc từ công cụ Short Position trên màn hình) [HÌNH][cite: 1]:
  - **Entry**: `4,334.81` (tại mốc Fibo `0.705`)[cite: 1].
  - **Stop Loss**: `4,383.17` (tại mốc Fibo `1`), tương ứng khoảng dừng lỗ `48.36` giá (`1.12%`), hiển thị `4,836` ticks/points[cite: 1].
  - **Take Profit**: `4,219.25` (tại mốc Fibo `0`), tương ứng khoảng mục tiêu `115.56` giá (`2.67%`), hiển thị `11,556` ticks/points[cite: 1].
  - **Tỷ lệ Lợi nhuận/Rủi ro (R:R)**: `2.39`[cite: 1].
- **Kết quả**: Giá chạm vùng OTE (quá nhẹ lên trên `0.705` một chút nhưng chưa chạm `0.79`), sau đó giảm mạnh một mạch xuyên qua mốc TP `0 (4,219.25)` [HÌNH][cite: 1].
- **Minh họa quy tắc**: Minh họa thuận cho quy tắc `Trend tăng + CHoCH + hồi về OTE -> Short`[cite: 1].

### 5.2 Ví dụ 2: Lệnh Long đảo chiều từ Trend giảm (00:25 – 00:37)
- **Mốc thời gian**: `00:25` – `00:37`[cite: 1].
- **Sản phẩm & Hướng lệnh**: Vàng (`XAUUSD`), lệnh Mua (Long) [NÓI, HÌNH][cite: 1].
- **Bối cảnh trước setup**: Giá đang trong xu hướng giảm, tạo đáy thấp nhất tại `3,998.05`, sau đó bật tăng mạnh bằng các nến xanh lớn phá qua đỉnh gần nhất tạo `CHoCH` lên mức `4,116.85` [NÓI, HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart**:
  - Đánh dấu hộp đỏ `CHoCH` tại vùng đỉnh cũ bị phá vỡ [HÌNH][cite: 1].
  - Kéo Fibonacci từ đáy `1 (3,998.05)` lên đỉnh `0 (4,116.85)` [NÓI, HÌNH][cite: 1].
  - Các mốc giá Fibonacci hiển thị trên màn hình (chữ khá nhỏ nhưng đọc được các mốc chính) [HÌNH][cite: 1]:
    - `0`: `4,116.85`[cite: 1]
    - `0.5`: `4,057.45`[cite: 1]
    - `0.618`: `4,043.43`[cite: 1]
    - `0.705`: `4,033.10`[cite: 1]
    - `0.79`: `4,023.00`[cite: 1]
    - `0.886`: `4,011.59`[cite: 1]
    - `1`: `3,998.05`[cite: 1]
  - Đánh dấu hộp xanh `OTE` từ `0.618` đến `0.79` và khoanh tròn điểm giá hồi về chạm `0.705` [HÌNH][cite: 1].
- **Entry / SL / TP cụ thể** [HÌNH][cite: 1]:
  - **Entry**: `4,033.10` (mốc Fibo `0.705`)[cite: 1].
  - **Stop Loss**: `3,998.05` (mốc Fibo `1`)[cite: 1].
  - **Take Profit**: `4,116.85` (mốc Fibo `0`)[cite: 1].
- **Kết quả**: Sau khi rút chân tại vùng OTE (`0.705` – `0.79`), giá bật tăng mạnh vượt qua mức TP `4,116.85` [HÌNH][cite: 1].
- **Minh họa quy tắc**: Minh họa thuận cho quy tắc `Trend giảm + CHoCH + hồi về OTE -> Long`[cite: 1].

### 5.3 Ví dụ 3: Ứng dụng dán công thức vào AI của TradingView (01:14 – 01:37)
- **Mốc thời gian**: `01:14` – `01:37`[cite: 1].
- **Sản phẩm & Khung thời gian**: `XAUUSD`, khung `1H` (hiển thị trong hộp thoại: `TÍN HIỆU CHoCH + OTE — XAUUSD 1H`) [HÌNH][cite: 1].
- **Bối cảnh & Thao tác**:
  - Tác giả gõ câu lệnh vào khung chat AI: `"Hãy tạo cho tôi tín hiệu theo CHoCH + OTE"` [HÌNH][cite: 1].
  - Trên biểu đồ là chính đoạn giá của Ví dụ 1 (đỉnh `4,383.17`, đường kẻ ngang đánh dấu `CHoCH 4,317.72`, kéo Fibo xuống đáy quanh `4,218` – `4,219`) [HÌNH][cite: 1].
- **Kết quả trả về từ hộp thoại AI và đường kẻ ngang trên chart** [HÌNH][cite: 1]:
  - AI xuất bảng `TÍN HIỆU CHoCH + OTE — XAUUSD 1H` gồm:
    - Trạng thái: `Tín hiệu BÁN (SHORT)`[cite: 1].
    - Điểm vào lệnh (Entry): Hiển thị các mức trong vùng OTE, đường kẻ ngang màu xanh lá trên trục giá đánh dấu `Entry: 4,335.00` (xấp xỉ mốc `0.705` là `4,334.72`)[cite: 1].
    - Stop Loss (SL): Đường kẻ ngang màu đỏ đánh dấu `SL: 4,385.00` (nằm ngay phía trên đỉnh `1 (4,383.17)` khoảng gần 2 giá)[cite: 1].
    - Take Profit (TP): Đường kẻ ngang trên trục giá hiển thị `TP1: 4,218.59` (ngay đáy `0`) và `TP2: 4,155.00` (mở rộng xuống dưới)[cite: 1].
- **Kết quả**: Giá khớp lệnh và giảm sâu qua cả `TP1` và `TP2` [HÌNH][cite: 1].

## 6. Tips, Tricks & Cảnh báo
- **Mốc quan trọng trong vùng OTE**: Dù vùng OTE kéo dài từ `0.618` đến `0.79`, tác giả nhấn mạnh phải đặc biệt lưu ý mốc `0.705` nằm ở giữa vì mốc này "khá là quan trọng" [NÓI][cite: 1].
- **Tự động hóa bằng AI**: Thay vì tự ngồi dò tìm thủ công hoàn toàn, có thể copy công thức (`Trend + CHoCH + OTE`) dán vào con AI trên TradingView để yêu cầu nó tự phân tích biểu đồ trên khung thời gian đang xem và xuất ra điểm Entry đúng theo công thức [NÓI][cite: 1].

## 7. Quản trị rủi ro & Tâm lý
- Video không đề cập đến phần trăm rủi ro mỗi lệnh (Risk %), cách tính khối lượng (lot size), hay tâm lý giao dịch.

## 8. Đặc tả logic cho LLM / Bot

Quy tắc trong video có tính đối xứng hoàn toàn giữa lệnh LONG và SHORT[cite: 1]. Dưới đây là đặc tả cấu trúc điều kiện (lưu ý một số định nghĩa cấu trúc gốc cần tham số hóa thêm vì video chỉ chỉ bằng mắt):

- **THAM SỐ CẤU HÌNH (`PARAMETERS`)**:
  - `FIBO_OTE_UPPER` = `0.618`[cite: 1]
  - `FIBO_OTE_OPTIMAL` = `0.705`[cite: 1]
  - `FIBO_OTE_LOWER` = `0.79`[cite: 1]
  - `LOOKBACK_SWING` = `UNSPECIFIED_IN_VIDEO` (Số nến để xác định đỉnh/đáy cấu trúc)

- **LOGIC CHO LỆNH BÁN (`SHORT_SETUP`)**:
  - **ĐIỀU KIỆN BỐI CẢNH (`CONTEXT`)**:
    - `prior_trend == UPTREND` (`SUBJECTIVE`: Giá tạo các nhịp tăng rõ ràng trước đó trên biểu đồ)[cite: 1]
    - Xác định đỉnh cao nhất của xu hướng tăng: `swing_high_1` (tương ứng mốc Fibo `1.0`)[cite: 1]
    - Xác định đáy cấu trúc gần nhất trước khi tạo đỉnh `swing_high_1`: `last_higher_low`[cite: 1]
  - **ĐIỀU KIỆN KÍCH HOẠT CẤU TRÚC (`STRUCTURE_SHIFT`)**:
    - Giá giảm mạnh phá vỡ xuống dưới `last_higher_low` -> Xác nhận có `bearish_CHoCH == TRUE`[cite: 1]
    - Đợi nhịp giảm kết thúc và bắt đầu hồi lên, xác định đáy thấp nhất của nhịp giảm đó: `swing_low_0` (tương ứng mốc Fibo `0.0`)[cite: 1]
  - **TÍNH TOÁN VÙNG GIÁ (`FIBO_CALCULATION`)**:
    - `range` = `swing_high_1 - swing_low_0`[cite: 1]
    - `ote_low_price` = `swing_low_0 + range * 0.618`[cite: 1]
    - `ote_mid_price` = `swing_low_0 + range * 0.705`[cite: 1]
    - `ote_high_price` = `swing_low_0 + range * 0.79`[cite: 1]
  - **ĐIỀU KIỆN VÀO LỆNH (`TRIGGER & ENTRY`)**:
    - `IF` giá hồi lên (`pullback`) đi vào vùng `[ote_low_price, ote_high_price]` (tức `0.618` đến `0.79`)[cite: 1]:
      - `ENTRY_SHORT` = Đặt lệnh tại `ote_mid_price` (mốc `0.705`)[cite: 1]
      - (Lưu ý: Video không nói rõ đặt Sell Limit sẵn tại `0.705` hay đợi nến phản ứng trong vùng `0.618 - 0.79`, nhưng hình minh họa đặt cố định ở `0.705`)[cite: 1]
  - **STOP LOSS & TAKE PROFIT (`SL_TP`)**:
    - `SL_SHORT` = `swing_high_1` (mốc Fibo `1.0`) hoặc cộng thêm một khoảng đệm nhỏ `BUFFER = UNSPECIFIED_IN_VIDEO`[cite: 1]
    - `TP_SHORT` = `swing_low_0` (mốc Fibo `0.0`)[cite: 1]
  - **ĐIỀU KIỆN HỦY (`INVALIDATION`)**:
    - `UNSPECIFIED_IN_VIDEO` (Thông thường theo logic Fibo: hủy nếu giá chạm `swing_low_0` hoặc phá lên trên `swing_high_1` trước khi khớp lệnh, nhưng tác giả không nói).

- **LOGIC CHO LỆNH MUA (`LONG_SETUP`)**:
  - Ngược lại hoàn toàn (đối xứng) với `SHORT_SETUP`[cite: 1]:
    - `prior_trend == DOWNTREND` -> Giá phá đỉnh gần nhất tạo `bullish_CHoCH == TRUE`[cite: 1].
    - Kéo Fibo từ đáy `swing_low_1` (mốc `1.0`) lên đỉnh nhịp phá vỡ `swing_high_0` (mốc `0.0`)[cite: 1].
    - `ote_high_price` = `swing_high_0 - range * 0.618`[cite: 1].
    - `ote_mid_price` = `swing_high_0 - range * 0.705`[cite: 1].
    - `ote_low_price` = `swing_high_0 - range * 0.79`[cite: 1].
    - `ENTRY_LONG` = `ote_mid_price` (`0.705`) khi giá hồi xuống vùng OTE[cite: 1].
    - `SL_LONG` = `swing_low_1` (`1.0`)[cite: 1].
    - `TP_LONG` = `swing_high_0` (`0.0`)[cite: 1].

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Cách xác định đáy kết thúc của sóng CHoCH (Mốc Fibo 0)**: Trên biểu đồ quá khứ, tác giả kéo Fibo từ đỉnh `1` xuống đáy `0` rất chuẩn xác. Tuy nhiên trong thực chiến (real-time), khi giá đang rơi tạo `CHoCH`, video không nêu quy tắc làm sao biết giá đã tạo đáy `0` xong để bắt đầu kéo Fibo (ví dụ: cần mấy nến hồi xanh, hay chạm hỗ trợ nào).
- **Cách thức khớp lệnh (Limit hay Market Confirmation)**: Tác giả nói "đợi cho giá quay về vùng OTE, entry, lụm" [NÓI][cite: 1], còn trên hình điểm Entry luôn đặt ngay vạch `0.705` [HÌNH][cite: 1]. Không rõ người giao dịch nên đặt lệnh chờ (Limit) cố định tại `0.705`, hay đợi giá chạm vùng `0.618 - 0.79` rồi tìm tín hiệu nến đảo chiều mới vào lệnh.
- **Quy tắc xác định CHoCH hợp lệ**: Không nêu rõ phá vỡ bằng râu nến (wick) hay phải đóng thân nến (body close) qua đáy/đỉnh cũ mới được tính là `CHoCH`.
- **Khung thời gian chuẩn cho Scalping**: Tác giả nói đây là giáo án "scalping vàng" [NÓI][cite: 1], nhưng biểu đồ minh họa lại có biên độ dừng lỗ lên tới `48.36` giá Vàng (`4,334.81` lên `4,383.17`) và TP `115.56` giá trên khung `1H` [HÌNH][cite: 1] – đây là biên độ của giao dịch Swing/Intraday lớn chứ không phải biên độ vài giá của Scalping thông thường trên M1/M5.
- **Con AI của TradingView**: Từ `01:15` tác giả nhắc đến việc dán công thức vào "con AI của TradingView" [NÓI][cite: 1], trên màn hình hiện giao diện cửa sổ chat đè lên biểu đồ TradingView [HÌNH][cite: 1]. Tác giả không nói rõ đây là tính năng tích hợp nào, extension bên thứ ba hay công cụ riêng của nhóm.

## 10. Thông tin khác
- **Tài liệu & Kênh**:
  - Kênh phát hành: `TradingMienTrung` [NÓI, HÌNH][cite: 1].
  - Series: `"Series 100 Entry Trade Vàng"` / `"100 Entry Scalping Vàng"` [NÓI, HÌNH][cite: 1].
- **Quảng cáo / Kêu gọi hành động (CTA)**:
  - Tác giả nhắn người xem nếu chưa biết vùng OTE là gì thì tải bộ tài liệu do bên tác giả chuẩn bị sẵn để theo dõi [NÓI] (từ `00:38` đến `00:44`)[cite: 1].
  - Kêu gọi Follow kênh `TradingMienTrung` để theo dõi tiếp series 100 entry giao dịch vàng và cách dùng AI phân tích [NÓI] (từ `01:28` đến `01:37`)[cite: 1].
- **Trích dẫn nguyên văn đáng giữ**:
  - `"Ở đây mình sẽ có công thức là CHoCH + OTE và Entry."` (`00:05` – `00:09`)[cite: 1].
  - `"Vùng OTE này mình đang để ở cái mốc là từ 0.618 của Fibo đến 0.79, nhưng mà trong đó có cái mốc 0.705 khá là quan trọng, anh em lưu ý giúp mình nhé."` (`00:46` – `00:56`)[cite: 1].