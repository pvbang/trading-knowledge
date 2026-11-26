---
title: "Hiểu Premium vs Discount để Lọc FVG và Tìm Điểm Vào Lệnh Tối Ưu"
source_author: "Giải Mã SMC (@giaimasmc)"
video_duration: "01:14"
video_type: ["SMC / ICT", "Volume / Order Flow / Volume Profile / Footprint / DOM"]
markets: ["NASDAQ", "Chung"]
timeframes_htf: ["KHÔNG RÕ"]
timeframes_ltf: ["15M"]
tools: ["FVG (Fair Value Gap)", "Premium / Discount (50% Range)", "Order Flow / Footprint"]
tags: ["SMC", "FVG", "Fair Value Gap", "Premium", "Discount", "Liquidity Sweep", "Order Flow", "NASDAQ", "15M"]
extraction_confidence: "Cao – Video ngắn, âm thanh và hình ảnh đồ họa minh họa rõ ràng, tuy nhiên một số quy tắc chi tiết về cách xác định biên độ giá và cách đọc Order Flow không được giải thích sâu."
---

# Hiểu Premium vs Discount để Lọc FVG và Tìm Điểm Vào Lệnh Tối Ưu[cite: 1]

## 0. TL;DR
- Không giao dịch mọi Fair Value Gap (FVG) xuất hiện trên biểu đồ vì vị trí hình thành mới là yếu tố quan trọng nhất [NÓI][cite: 1].
- Với lệnh mua (Long), tuyệt đối tránh mua tại FVG nằm ở vùng Premium (trên mức 50% biên độ giá) vì giá đã đắt và dễ trở thành thanh khoản thoát lệnh cho người khác [NÓI][cite: 1].
- Chỉ giao dịch FVG tăng hình thành trong vùng Discount (dưới mức 50% biên độ giá), nơi giá đang bị định giá thấp và có sự tham gia của các tổ chức [NÓI][cite: 1].
- Điểm vào lệnh có xác suất cao nhất khi hội tụ đủ 4 yếu tố: Quét thanh khoản (Liquidity Sweep / quét Stop Loss) + tạo FVG đảo chiều tăng + nằm trong vùng Discount + xác nhận bằng Order Flow [NÓI][cite: 1].

## 1. Tổng quan
- **Mục tiêu / vấn đề video giải quyết**: Cung cấp bộ lọc vị trí (Premium/Discount) kết hợp quét thanh khoản và Order Flow để nâng cao tỷ lệ thắng khi giao dịch với FVG, tránh bẫy mua đuổi ở vùng giá cao [NÓI, HÌNH][cite: 1].
- **Đối tượng phù hợp**: Video không đề cập[cite: 1].
- **Thị trường & sản phẩm**: Minh họa trực tiếp trên chỉ số `NASDAQ` [HÌNH]; nguyên lý áp dụng chung cho phương pháp SMC [SUY LUẬN: kênh tên là Giải Mã SMC và trình bày lý thuyết chung][cite: 1].
- **Khung thời gian**: Khung `15M` (15 phút) trên biểu đồ minh họa [HÌNH]; lời nói không giới hạn khung thời gian cụ thể [NÓI][cite: 1].
- **Phiên giao dịch áp dụng**: Video không đề cập[cite: 1].
- **Công cụ & thiết lập chỉ báo**:
  - Công cụ đo biên độ giá chia 2 vùng `Premium` và `Discount` tại mốc `50%` (điểm giữa của biên độ giá) [NÓI, HÌNH][cite: 1].
  - Vùng `FVG` (Fair Value Gap) được vẽ thủ công trên cụm 3 nến [HÌNH][cite: 1].
  - Biểu đồ `Order Flow` / Footprint hiển thị khối lượng chi tiết từng mức giá bên trong thân nến (không nêu tham số cài đặt cụ thể) [NÓI, HÌNH][cite: 1].

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Cơ chế của FVG**: Hình thành khi thị trường di chuyển mạnh đến mức bỏ qua hoàn toàn một số mức giá, tạo ra khoảng trống giữa râu nến thứ nhất và râu nến thứ ba; khoảng trống này đóng vai trò như một "nam châm" hút giá quay trở lại [NÓI][cite: 1].
- **Cơ chế định giá (Premium vs Discount)**:
  - Trên mức `50%` của biên độ giá là vùng `Premium` (giá đắt): Mua tại đây là vào quá muộn và "trở thành thanh khoản thoát lệnh cho một người thông minh hơn bạn" [NÓI][cite: 1].
  - Dưới mức `50%` của biên độ giá là vùng `Discount` (giá bị định giá thấp): Đây là vùng giá rẻ nơi các tổ chức lớn thực sự muốn tham gia mua vào [NÓI][cite: 1].
- **Cơ chế thao túng / Thanh khoản**: Nếu trước khi tạo FVG tăng trong vùng Discount mà giá có cú quét xuống dưới lấy thanh khoản (quét Stop Loss), thì đó là "một chuyển động có tính toán" nhằm loại bỏ những vị thế mua yếu trước khi đảo chiều thật sự [NÓI][cite: 1].
- **Điều kiện thị trường phù hợp / KHÔNG phù hợp**: Video chỉ minh họa bối cảnh thị trường có một biên độ giá (range) đã hình thành để kẻ mức 50%; không đề cập cách xử lý khi thị trường chạy xu hướng một chiều không rõ biên độ [HÌNH, SUY LUẬN: cần có đỉnh và đáy của biên độ để chia đôi 50%][cite: 1].

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **FVG (Fair Value Gap)** | Khoảng trống giá hình thành khi thị trường di chuyển mạnh bỏ qua một số mức giá, đóng vai trò như "nam châm" khi giá quay lại [NÓI][cite: 1]. | Cụm 3 cây nến cùng chiều (minh họa là nến tăng), trong đó có khoảng trống ở giữa cây nến thứ 1 và cây nến thứ 3 mà phần râu nến của chúng không chồng lên nhau [NÓI, HÌNH][cite: 1]. |
| **Premium** | Vùng giá đắt, nơi người mua muộn trở thành thanh khoản thoát lệnh cho người khác [NÓI][cite: 1]. | Nửa phía trên mức `50%` của biên độ giá (được tô màu tím hồng trên chart) [NÓI, HÌNH][cite: 1]. |
| **Discount** | Vùng giá đang bị định giá thấp, nơi các tổ chức muốn tham gia mua [NÓI][cite: 1]. | Nửa phía dưới mức `50%` (điểm giữa) của biên độ giá (được tô màu xanh tím nhạt trên chart) [NÓI, HÌNH][cite: 1]. |
| **Quét thanh khoản (`LIQ taken >`)** | Hành động giá quét xuống dưới đáy cũ để quét Stop Loss, loại bỏ các vị thế mua yếu trước khi đảo chiều [NÓI, HÌNH][cite: 1]. | Râu nến (hoặc thân nến) chọc thủng xuống dưới một đáy trước đó trong vùng Discount rồi rút lên tạo FVG tăng (ký hiệu `LIQ taken >` với đường nét đứt ngang đáy bị quét) [NÓI, HÌNH][cite: 1]. |
| **Order Flow** | Công cụ xác nhận dòng lệnh để tăng xác suất điểm vào (tác giả không định nghĩa chi tiết bằng lời) [NÓI][cite: 1]. | Hiển thị dưới dạng biểu đồ Footprint với các con số khối lượng mua/bán theo từng bước giá nằm dọc bên trong từng cây nến [HÌNH][cite: 1]. |

## 4. Hệ thống quy tắc
*(Lưu ý: Video chỉ trình bày quy tắc cho chiều Mua - Long. Chiều Bán - Short không được đề cập)*[cite: 1].

### 4.1 Điều kiện tiên quyết / Confluence (Checklist)
- [ ] Xác định được biên độ giá hiện tại và kẻ mức `50%` chia đôi vùng `Premium` (trên) và `Discount` (dưới) [NÓI, HÌNH][cite: 1].
- [ ] Giá đang ở trong vùng `Discount` (bên dưới điểm giữa `50%` của biên độ giá) [NÓI][cite: 1].
- [ ] Có sự kiện quét thanh khoản (`LIQ taken >` / quét Stop Loss) bên dưới một đáy trước đó trước khi FVG hình thành [NÓI, HÌNH][cite: 1].
- [ ] Xuất hiện cụm 3 nến tạo `FVG` tăng nằm bên trong vùng `Discount` [NÓI, HÌNH][cite: 1].
- [ ] Kết hợp xác nhận từ `Order Flow` [NÓI, HÌNH][cite: 1].

### 4.2 Xác định bối cảnh & hướng (Bias)
- **Quy tắc cứng**: Đối với lệnh Mua (Long), chỉ tìm kiếm cơ hội ở vùng `Discount` (dưới mức `50%` biên độ giá) [NÓI][cite: 1].
- **Dấu hiệu đảo chiều**: Cú quét Stop Loss kết hợp tạo `FVG` tăng ngay sau đó bên trong vùng `Discount` xác nhận ý đồ đảo chiều tăng có tính toán [NÓI][cite: 1].

### 4.3 Tín hiệu kích hoạt (Trigger)
- Sau khi giá quét thanh khoản (`LIQ taken >`) và đẩy lên mạnh tạo `FVG` tăng trong vùng `Discount`, chờ giá quay trở lại (pullback/retest) chạm vào vùng `FVG` đó và kết hợp quan sát `Order Flow` [NÓI, HÌNH][cite: 1].

### 4.4 Entry
- **Loại lệnh**: `VIDEO KHÔNG ĐỀ CẬP` bằng lời (trên hình minh họa công cụ đo lệnh đặt tại ranh giới/bên trong vùng `FVG` khi cây nến giảm quay lại test vùng `FVG`) [HÌNH][cite: 1].
- **Vị trí**: Tại vùng `FVG` tăng nằm trong vùng `Discount` (trên hình, mức Entry của khung lệnh nằm ở khoảng nửa trên của hộp `FVG`) [HÌNH][cite: 1].

### 4.5 Stop Loss (SL)
- **Quy tắc bằng lời**: `VIDEO KHÔNG ĐỀ CẬP`[cite: 1].
- **Quy tắc trên hình**: Đặt bên dưới vùng `FVG` (trên biểu đồ ở `01:08 - 01:13`, cạnh dưới của hộp Stop Loss màu đỏ nằm ngang mức đáy thân nến đầu tiên tạo FVG, cao hơn một chút so với đáy râu nến quét thanh khoản `LIQ taken >`) [HÌNH][cite: 1].

### 4.6 Take Profit (TP) / Quản lý lệnh
- **Quy tắc bằng lời**: `VIDEO KHÔNG ĐỀ CẬP`[cite: 1].
- **Quy tắc trên hình**: Đặt tại mức đỉnh cao nhất của biên độ giá (ranh giới trên cùng của vùng `Premium`), tương ứng tỷ lệ R:R khoảng xấp xỉ 1:3.5 đến 1:4 trên hình vẽ [HÌNH, SUY LUẬN: ước lượng trực quan từ độ cao hộp TP màu xanh so với hộp SL màu đỏ ở `01:10`][cite: 1].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- **Quy tắc cứng**: KHÔNG mua khi `FVG` tăng hình thành ở vùng `Premium` (phía trên mức `50%` của biên độ giá), vì lúc này giá đã đắt và vào lệnh quá muộn [NÓI, HÌNH][cite: 1].

## 5. Case Study / Ví dụ chart

### 5.1 Ví dụ 1 (Phản ví dụ): FVG thất bại trong vùng Premium
- **Mốc thời gian trong video**: `00:22 – 00:36` [HÌNH][cite: 1].
- **Sản phẩm, khung thời gian, hướng lệnh**: `NASDAQ`, khung `15M`, hướng xét lệnh Mua (Long) [NÓI, HÌNH][cite: 1].
- **Bối cảnh trước setup**: Giá tăng một mạch từ đáy lên cao, tạo một biên độ giá được chia làm 2 nửa: `Discount` ở dưới và `Premium` ở trên [HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Tác giả đánh dấu một vùng `FVG` tăng nằm khá cao trong nửa trên (`Premium` - vùng màu tím) [HÌNH][cite: 1].
  - Lý do không vào: Khoảng trống `FVG` nằm trên mức `50%` biên độ giá, tức giá đang đắt; mua ở đây là làm thanh khoản thoát lệnh cho người khác [NÓI][cite: 1].
- **Entry / SL / TP cụ thể**: Không có mức giá cụ thể (biểu đồ đồ họa không hiển thị trục giá) [HÌNH][cite: 1].
- **Kết quả và bài học**: Giá chạm vào vùng `FVG` ở `Premium`, chỉ phản ứng giữ giá trong 1-2 nến rồi đâm xuyên thủng mạnh xuống tận đáy vùng `Discount` [HÌNH]. Bài học: Vị trí quan trọng hơn bản thân mô hình FVG; tránh giao dịch FVG ở vùng giá đắt [NÓI][cite: 1].
- **Minh họa quy tắc**: Quy tắc 4.7 (Điều kiện KHÔNG vào lệnh khi FVG nằm trên mức 50% biên độ giá) [NÓI, HÌNH][cite: 1].

### 5.2 Ví dụ 2 (Ví dụ thuận): FVG xác suất cao trong vùng Discount có quét thanh khoản
- **Mốc thời gian trong video**: `00:00 – 00:02` và `00:36 – 01:14` [HÌNH][cite: 1].
- **Sản phẩm, khung thời gian, hướng lệnh**: `NASDAQ`, khung `15M`, lệnh Mua (Long) [NÓI, HÌNH][cite: 1].
- **Bối cảnh trước setup**: Giá đang dao động ở phần dưới (`Discount`) của biên độ giá tổng thể [HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Vẽ vùng `Premium` (trên 50%) và `Discount` (dưới 50%) [HÌNH][cite: 1].
  - Đánh dấu đường nét đứt `LIQ taken >` tại đáy cũ trong vùng `Discount`, nơi một cây nến giảm chọc râu xuống quét Stop Loss của các vị thế mua yếu [NÓI, HÌNH][cite: 1].
  - Ngay sau cú quét, giá bật tăng mạnh tạo `FVG` nằm hoàn toàn trong vùng `Discount` [NÓI, HÌNH][cite: 1].
  - Khi giá quay lại test vùng `FVG`, bật hiển thị `Order Flow` (Footprint) trên từng cây nến để xác nhận dòng tiền trước khi giá bứt phá lên vùng `Premium` [NÓI, HÌNH][cite: 1].
- **Entry / SL / TP cụ thể**: Không có con số mức giá trên trục tung; khung lệnh Long trên hình (`01:09`) đặt Entry tại vùng `FVG` khi nến retest, SL ngay dưới chân cụm nến tạo `FVG`, TP tại đỉnh vùng `Premium` [HÌNH][cite: 1].
- **Kết quả và bài học**: Giá từ vùng `FVG` trong `Discount` tăng mạnh một mạch lên vượt đỉnh vùng `Premium` và chạm TP [HÌNH]. Bài học: Sự kết hợp giữa Quét thanh khoản + FVG đảo chiều + Vùng Discount + Order Flow tạo nên điểm vào xác suất cao và có tính toán của tổ chức [NÓI][cite: 1].
- **Minh họa quy tắc**: Toàn bộ quy tắc ở mục 4.1 đến 4.6 [NÓI, HÌNH][cite: 1].

## 6. Tips, Tricks & Cảnh báo
- **Cảnh báo bẫy thanh khoản**: Đừng giao dịch mọi FVG chỉ vì thấy khoảng trống 3 nến; vị trí của FVG trong biên độ giá mới là yếu tố quyết định [NÓI][cite: 1].
- **Sai lầm phổ biến**: Mua tại FVG nằm trên mức `50%` biên độ giá (vùng `Premium`) khiến bạn vào lệnh quá muộn và trở thành thanh khoản thoát lệnh (exit liquidity) cho người thông minh hơn [NÓI][cite: 1].
- **Cách lọc tín hiệu nhiễu**: Luôn tự đặt 2 câu hỏi trước khi vào lệnh với FVG tăng: (1) FVG có nằm dưới điểm giữa `50%` (vùng `Discount`) không? (2) Trước khi tạo FVG, giá có quét xuống dưới để lấy thanh khoản (quét Stop Loss) không? [NÓI][cite: 1].
- **Mẹo nâng cao xác suất**: Kết hợp thêm `Order Flow` tại vùng `FVG` ở `Discount` sau cú quét thanh khoản để xác nhận điểm vào xác suất cao [NÓI, HÌNH][cite: 1].

## 7. Quản trị rủi ro & Tâm lý
Video không đề cập[cite: 1].

## 8. Đặc tả logic cho LLM / Bot
*(Lưu ý: Video chỉ mô tả chiều LONG. Chiều SHORT không được đề cập nhưng theo lý thuyết SMC thông thường sẽ đối xứng ngược lại; tuy nhiên để trung thực dữ liệu, dưới đây chỉ mã hóa chiều LONG đúng như video trình bày)*[cite: 1].

- **ĐIỀU KIỆN BỐI CẢNH (CONTEXT)**
  - Xác định `price_range_high` và `price_range_low` của biên độ giá hiện tại (`SUBJECTIVE:` Video không nêu quy tắc cụ thể để chọn đỉnh/đáy của biên độ giá `UNSPECIFIED_IN_VIDEO`) [HÌNH][cite: 1].
  - Tính điểm giữa: `equilibrium_50 = (price_range_high + price_range_low) / 2` [NÓI, HÌNH][cite: 1].
  - Định nghĩa vùng:
    - IF `price > equilibrium_50` THEN `zone = PREMIUM` [NÓI, HÌNH][cite: 1].
    - IF `price < equilibrium_50` THEN `zone = DISCOUNT` [NÓI, HÌNH][cite: 1].

- **ĐIỀU KIỆN LỌC & TRIGGER (LONG SETUP)**
  - Bước 1 (Quét thanh khoản): Kiểm tra có sự kiện `liquidity_sweep_low == True` (giá tạo đáy thấp hơn một đáy swing trước đó trong vùng `DISCOUNT` để quét Stop Loss) [NÓI, HÌNH][cite: 1].
  - Bước 2 (Hình thành FVG tăng): Ngay sau `liquidity_sweep_low`, xuất hiện cụm 3 nến (`candle_1`, `candle_2`, `candle_3`) thỏa mãn:
    - `candle_3.low > candle_1.high` (không có phần râu nến chồng lên nhau, tạo khoảng trống từ `fvg_bottom = candle_1.high` đến `fvg_top = candle_3.low`) [NÓI, HÌNH][cite: 1].
  - Bước 3 (Bộ lọc vị trí Premium/Discount):
    - IF `fvg_top <= equilibrium_50` (FVG nằm trong vùng `DISCOUNT`) THEN `fvg_valid = True` [NÓI, HÌNH][cite: 1].
    - IF `fvg_bottom > equilibrium_50` (FVG nằm trong vùng `PREMIUM`) THEN `fvg_valid = False` (Hủy kèo) [NÓI, HÌNH][cite: 1].
  - Bước 4 (Xác nhận bổ sung):
    - Khi giá quay lại chạm vào khoảng `[fvg_bottom, fvg_top]`, kiểm tra `order_flow_confirmation == True` (`SUBJECTIVE:` Video chỉ chiếu hình Footprint trên nến và nói "kết hợp thêm Order Flow", không nêu điều kiện số học cụ thể `UNSPECIFIED_IN_VIDEO`) [NÓI, HÌNH][cite: 1].

- **ENTRY / SL / TP (LONG)**
  - `ENTRY`: Mở vị thế Mua khi giá retest vùng `[fvg_bottom, fvg_top]` và `fvg_valid == True` và `order_flow_confirmation == True` [NÓI, HÌNH][cite: 1].
  - `SL`: Đặt dưới vùng FVG hoặc dưới đáy cụm nến tạo FVG (`UNSPECIFIED_IN_VIDEO` bằng lời; trên hình đặt quanh mức `candle_1.open` / dưới `fvg_bottom`) [HÌNH][cite: 1].
  - `TP`: Đặt tại `price_range_high` (đỉnh của vùng `PREMIUM` trên hình vẽ; `UNSPECIFIED_IN_VIDEO` bằng lời) [HÌNH][cite: 1].

- **ĐIỀU KIỆN HỦY (INVALIDATION)**
  - Bỏ qua tín hiệu Mua nếu FVG hình thành tại `zone == PREMIUM` (`price > equilibrium_50`) [NÓI][cite: 1].

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Cách xác định đỉnh/đáy của biên độ giá (Dealing Range)**: Tác giả nói lấy mức `50%` của biên độ giá nhưng không giải thích cách chọn đỉnh (Swing High) và đáy (Swing Low) nào để kẻ biên độ đó [NÓI, HÌNH][cite: 1].
- **Cách đọc Order Flow**: Ở `01:05 - 01:12`, màn hình hiển thị các con số khối lượng (Footprint) bên trong thân nến và tác giả nói "kết hợp thêm Order Flow", nhưng hoàn toàn không giải thích cần tìm dấu hiệu gì trong Order Flow (ví dụ: hấp thụ, mất cân bằng khối lượng hay Delta dương) [NÓI, HÌNH][cite: 1].
- **Quy tắc Entry, SL, TP cụ thể**: Lời nói không đề cập đặt Entry ở mép trên, giữa (CE - 50% FVG) hay mép dưới của FVG, cũng như không nói rõ quy tắc đặt SL (dưới FVG hay dưới râu quét thanh khoản) và TP. Các thông tin này chỉ xuất hiện qua hình vẽ khung lệnh ở `01:08 - 01:13` [NÓI, HÌNH][cite: 1].
- **Lỗi phụ đề tự động trên video**:
  - Ở `00:13 - 00:14`, giọng đọc nói "tạo ra một cụm ba cây nến có khoảng trống ở giữa", nhưng phụ đề trên màn hình hiển thị thiếu chữ thành "và cây nến khoảng trống ở giữa" [NÓI, HÌNH][cite: 1].
  - Ở `00:25`, phụ đề hiện số "4" dư thừa ở đầu câu ("4 nếu khoảng trống") [HÌNH][cite: 1].
  - Ở `00:56`, phụ đề viết không dấu cụm "quet stop loss" [HÌNH][cite: 1].
- **Câu hỏi cần làm rõ trước khi bot hóa**:
  1. Định nghĩa thuật toán chính xác để xác định Swing High và Swing Low của biên độ giá trên khung 15M là gì?
  2. Điều kiện định lượng của `Order Flow` để kích hoạt lệnh khi giá chạm FVG là gì?
  3. Đặt SL chuẩn là dưới đáy cây nến số 1 của FVG hay dưới râu nến quét thanh khoản (`LIQ taken >`)?

## 10. Thông tin khác
- **Kết quả/thống kê tác giả đưa ra (chưa được kiểm chứng)**:
  - Tác giả tuyên bố sau khi áp dụng bộ lọc này, "tỷ lệ thắng với FVG của mình đã tăng gấp đôi" [NÓI][cite: 1].
  - Ở `00:03 - 00:06`, màn hình hiển thị ảnh chụp thống kê: `Trade win %: 87.23%` với các con số `58` (xanh lá - thắng), `1` (xám - hòa), `7` (đỏ - thua) [HÌNH, SUY LUẬN: 58 / (58 + 7) = 89.23% hoặc 58 / (58 + 1 + 7) = 87.87%, giao diện giống bảng thống kê của phần mềm nhật ký giao dịch như TradeZella, chưa có bằng chứng kiểm toán độc lập][cite: 1].
- **Quảng cáo / Kêu gọi hành động (CTA)**: Banner cố định ở cuối màn hình suốt video ghi "Cộng đồng trade SMC - Link ở Bio" của kênh `Giải Mã SMC (@giaimasmc)` [HÌNH][cite: 1].
- **Trích dẫn nguyên văn đáng chú ý**:
  - "Khi bạn mua ở vùng giá đắt, bạn đang trở thành thanh khoản thoát lệnh cho một người thông minh hơn bạn." (`00:32 - 00:36`) [NÓI][cite: 1].
  - "Bởi vì nếu giá quét Stop Loss rồi sau đó tạo FVG tăng bên trong vùng Discount, thì đó không phải ngẫu nhiên, mà là một chuyển động có tính toán." (`00:56 - 01:02`) [NÓI][cite: 1].
- **Ghi chú của người trích xuất**:
  - [SUY LUẬN] Nội dung video là bản dịch/việt hóa ngắn gọn theo phong cách video ngắn (Shorts/Reels/TikTok) dựa trên các khái niệm cốt lõi của trường phái ICT / SMC (Premium & Discount array, Liquidity Sweep, Fair Value Gap) kết hợp với biểu đồ Footprint. Khi áp dụng thực tế cho chiều Bán (Short), toàn bộ quy tắc sẽ đảo ngược: chờ quét thanh khoản đỉnh (Buy-side Liquidity) và tìm FVG giảm nằm trong vùng Premium (trên mức 50% biên độ giá).