---
title: "Series 100 Entry Trade Vàng (Tập 9): 3 Kỹ Thuật Giao Dịch Bollinger Bands Kết Hợp SNR & Nguyên Tắc Vùng Cản"
source_author: "TradingMienTrung"
video_duration: "08:18"
video_type: ["Price Action / Key Level / Cấu trúc đỉnh đáy", "Indicator-based", "Review lệnh / Live trading / Backtest / Q&A / Kiến thức nền cho người mới", "Quản lý vốn, quản trị rủi ro, tâm lý giao dịch"]
markets: ["XAUUSD (Vàng)", "Chung"]
timeframes_htf: ["D1", "H4", "H1"]
timeframes_ltf: ["M30", "M15"]
tools: ["Bollinger Bands", "Hỗ trợ & Kháng cự (SNR / Key Level)", "RSI (nhắc tên)", "SMA (nhắc tên)"]
tags: ["Bollinger Bands", "SNR", "Scalping Gold", "Key Level", "Breakout Band", "Phản ứng Band", "Quét Band", "Quản trị rủi ro", "TradingMienTrung"]
extraction_confidence: "Cao – Trích xuất trực tiếp toàn bộ lời thoại, biểu đồ minh họa và slide chú thích trong video."
---

# Series 100 Entry Trade Vàng (Tập 9): 3 Kỹ Thuật Giao Dịch Bollinger Bands Kết Hợp SNR & Nguyên Tắc Vùng Cản

## 0. TL;DR
* Nguyên tắc cốt lõi của trader chuyên nghiệp: Tại một vùng cản, chỉ giao dịch tối đa 1 đến 2 lần; nếu giá quét thủng cản, bắt buộc phải cắt lỗ (Stop Loss) và chờ ở vùng cản tiếp theo, không gồng lỗ hay cố chấp [NÓI].
* Kỹ thuật 1 (Bắt phản ứng): Chờ giá chạm đường Band đồng thời hợp lưu chính xác với vùng cản SNR (khung H1, H4, D1) rồi mới vào lệnh [NÓI].
* Kỹ thuật 2 (Phá Band bám xu hướng): Khi Band M15/M30 co thắt rồi bung mở (mở rộng và chuối xuống/hướng lên), xác định mục tiêu Band khung lớn (H1, H4, D1), sau đó chờ giá hồi về test vùng SNR ở khung nhỏ để vào lệnh thuận xu hướng [NÓI].
* Kỹ thuật 3 (Quét Band đảo chiều): Thường xuất hiện ở D1 hoặc khi có tin tức mạnh (Non-Farm, FOMC, phiên Mỹ); giá đâm thủng Band và cản 1 để quét thanh khoản (quét SL), sau đó chạm vùng cản 2 (hợp lưu Band ngoài) rút râu đóng nến bên trên cản -> kích hoạt lệnh đảo chiều ăn nhịp hồi [NÓI].

## 1. Tổng quan
* **Mục tiêu / Vấn đề video giải quyết**: Giải quyết câu hỏi "Nếu giá quét qua cản/Band thì phải làm sao?" và hướng dẫn chi tiết cách kết hợp Bollinger Bands với các vùng SNR để scalping [NÓI].
* **Đối tượng phù hợp**: Phù hợp cho trader muốn bổ sung bài tủ scalping vàng hàng ngày, đặc biệt cảnh báo những anh em non kinh nghiệm hay vào lệnh vội vàng khi chưa có hợp lưu [NÓI].
* **Thị trường & Sản phẩm**: XAUUSD (Vàng) [HÌNH/NÓI].
* **Khung thời gian**:
  * Khung lớn (HTF): D1, H4, H1 [NÓI].
  * Khung nhỏ (LTF): M30, M15 [NÓI].
* **Phiên giao dịch áp dụng**: Nhấn mạnh phiên Mỹ (thường có sóng mạnh, tin tức bão mạnh như Non-Farm, FOMC) [NÓI]; phiên Á và phiên Âu thường sideway, ít xuất hiện sóng bám trend mạnh [NÓI].
* **Công cụ & Chỉ báo**:
  * Bollinger Bands: Gồm Upper Band (Band trên), Middle Band (Band giữa / trục giữa), Lower Band (Band dưới). Chu kỳ và độ lệch chuẩn cụ thể: VIDEO KHÔNG ĐỀ CẬP (dùng mặc định trên giao diện chart TradingView) [HÌNH].
  * Các mức/vùng Hỗ trợ & Kháng cự (SNR / Key Levels) [NÓI].
  * Video có nhắc tên RSI, SMA nhưng nội dung chính tập trung hoàn toàn vào Bollinger Bands + SNR [NÓI].

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
* **Nguyên lý tương tác vùng cản**: Bất kể dùng hỗ trợ/kháng cự hay chỉ báo (Bollinger Bands, RSI, SMA...), tại mỗi vùng cản chỉ xảy ra 2 trường hợp [NÓI]:
  1. Cản mạnh: Giá phản ứng và bật ngược lại theo kỳ vọng [NÓI].
  2. Cản yếu: Giá đục thủng / quét qua cản. Khi đó cản đã mất hiệu lực, bắt buộc phải dừng lỗ và tìm cản kế tiếp [NÓI].
* **Cơ chế hợp lưu (Confluence)**: Chỉ dựa vào một đường Bollinger Bands thì xác suất thắng không cao. Khi đường Band nằm trùng hoặc rất gần một vùng SNR (Hỗ trợ/Kháng cự), xác suất giá phản ứng sẽ tăng lên đáng kể [NÓI].
* **Lực hút của Band khung lớn**: Khi giá phá vỡ xu hướng ở khung nhỏ, giá có xu hướng di chuyển tìm về các đường Band của khung thời gian lớn hơn (H1, H4, D1) [NÓI].
* **Cơ chế thanh khoản / Quét SL**: Thị trường thường tạo bẫy ở các vùng đáy/đỉnh có nhiều râu nến (vùng tích lũy thanh khoản). Khi tin tức ra hoặc phiên Mỹ mở cửa, giá thường quét thủng đáy/đỉnh cũ để lấy thanh khoản trước khi đảo chiều thật sự [NÓI].

## 3. Thuật ngữ & Định nghĩa
| Thuật ngữ | Định nghĩa theo tác giả trong video | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **SNR** | Viết tắt của Support & Resistance (Hỗ trợ và Kháng cự) [NÓI]. | Các đường/vùng đáy cũ, đỉnh cũ hoặc cấu trúc đảo chiều trên biểu đồ [HÌNH]. |
| **Hợp lưu (+SNR)** | Sự trùng khớp hoặc tiệm cận giữa đường Bollinger Bands và một mức cản SNR [NÓI]. | Đường Band đi qua đúng vùng đỉnh/đáy cản ngang [HÌNH]. |
| **Phá Band bám xu hướng** | Trạng thái dải Band co thắt (sideway) rồi mở bung ra, nến đóng bám sát dải ngoài để chạy một trend dài [NÓI]. | Hai dải Band mở rộng; trong uptrend giá nằm giữa Upper Band và Middle Band; trong downtrend giá nằm giữa Lower Band và Middle Band [NÓI/HÌNH]. |
| **Quét Band** | Cú đạp hoặc đẩy giá mạnh xuyên thủng dải Band (vượt Band một đoạn rất đậm) do biến động mạnh [NÓI]. | Một cây nến biên độ lớn phóng vượt ra ngoài dải Band rồi rút râu để lại bóng nến dài [HÌNH]. |
| **MSNR Key Levels** | Hệ thống các dạng cản hỗ trợ - kháng cự mẫu tác giả chiếu trên màn hình [HÌNH]. | Gồm các dạng: Classic A, Classic V, SBR (Support Becomes Resistance), RBS (Resistance Becomes Support), OCL, QML [HÌNH]. |

## 4. Hệ thống quy tắc

### Nguyên tắc chung về Vùng Cản (Bắt buộc)
* **Số lần giao dịch tại một cản**: Tối đa 1 đến 2 lần [NÓI].
* **Quy tắc vi phạm cản**: Khi giá quét qua cản, bắt buộc phải chấp nhận Stop Loss (thoát lệnh ngay), tuyệt đối không gồng và chỉ tìm kiếm cơ hội ở vùng cản tiếp theo [NÓI].

---

### Chiến lược 1: Bắt đỉnh/đáy phản ứng (Chạm Band + Hợp lưu SNR)
Thích hợp cho khung H1, H4, D1 [NÓI].

#### 4.1 Điều kiện tiên quyết (Checklist)
* [ ] Giá tiếp cận đường Bollinger Bands (Upper Band đối với lệnh Sell, Lower Band đối với lệnh Buy) [NÓI].
* [ ] Tại vị trí đường Band đó, PHẢI có một vùng cản SNR (Kháng cự/Hỗ trợ) rõ ràng nằm hợp lưu [NÓI].
* [ ] KHÔNG vào lệnh nếu giá chỉ mới chạm đường Band mà chưa chạm tới vùng cản SNR [NÓI].

#### 4.2 Entry
* Chờ giá chạm đồng thời cả đường Band và vùng SNR [NÓI].
* Nến phản ứng rút râu tại vùng hợp lưu [NÓI].
* Vào lệnh trực tiếp (Market) hoặc Limit tại vùng hợp lưu [SUY LUẬN từ biểu đồ minh họa].

#### 4.3 Stop Loss & Take Profit
* **Stop Loss**: Đặt phía trên vùng cản SNR (đối với Sell) hoặc phía dưới vùng cản SNR (đối với Buy) [HÌNH].
* **Take Profit**: VIDEO KHÔNG ĐỀ CẬP con số R:R hay mức giá cụ thể; trên hình minh họa TP hướng về phía dải Band đối diện / Middle Band [HÌNH].

---

### Chiến lược 2: Phá Band bám xu hướng (Trend Following Scalping)
Thường xảy ra ở M15, M30 và kéo dài lên H1 [NÓI].

#### 4.1 Điều kiện tiên quyết & Bối cảnh
* [ ] Khung lớn (H1, H4, D1): Xác định vị trí các dải Band khung lớn xem còn dư địa để giá chạy tới hay không (giá có xu hướng tìm về Band HTF) [NÓI].
* [ ] Khung nhỏ (M30): Dải Band trước đó co thắt, sau đó mở rộng và chúi xuống (đối với Downtrend) hoặc ngửa lên (đối với Uptrend) [NÓI].
* [ ] Nến đóng cửa nằm bám sát dải Band ngoài (ví dụ đóng nến sát Lower Band) [NÓI/HÌNH].
* [ ] Nhận diện vùng thanh khoản: Trước cú phá vỡ, có vùng tích lũy tạo nhiều râu nến [NÓI]. Khi giá quay lại quét lần 2, vùng này bị đục thủng [NÓI].

#### 4.2 Entry
* Sau khi giá phá đáy/thủng cản và mở Band, KHÔNG đuổi theo nến xả [SUY LUẬN].
* Chờ giá hồi (pullback) về test lại vùng cản SNR phía trên (ví dụ hỗ trợ vừa bị phá vỡ chuyển thành kháng cự - SBR) [NÓI].
* Kích hoạt lệnh Sell thuận xu hướng giảm [NÓI].

#### 4.3 Stop Loss & Take Profit
* VIDEO KHÔNG ĐỀ CẬP quy tắc đặt SL/TP cụ thể bằng số pip cho chiến lược này; chỉ nêu hướng vào lệnh thuận xu hướng giảm sau nhịp test cản [NÓI].

---

### Chiến lược 3: Bắt đảo chiều khi bị quét Band & Quét cản (Liquidity Sweep)
Thường xuất hiện ở D1 hoặc trong phiên Mỹ có tin mạnh (Non-Farm, FOMC) [NÓI].

#### 4.1 Kịch bản bẫy giá ban đầu
* Giá đang trong xu hướng tăng mạnh trước đó [NÓI].
* Giá hồi về chạm cản 1 (ví dụ hợp lưu Middle Band D1) và phản ứng nhẹ [NÓI].
* Nhiều trader vào lệnh Buy sớm tại cản 1 và đặt SL ngay dưới cản 1 [NÓI].
* Thị trường xuất hiện cú xả mạnh đâm thủng cản 1, vượt ra ngoài đường Band, quét sạch Stop Loss của phe Buy [NÓI].

#### 4.2 Điều kiện kích hoạt đảo chiều (Vào lại lệnh)
* [ ] Chấp nhận dính SL ở cản 1, không cố gỡ ngay tại chỗ [NÓI].
* [ ] Xác định vùng cản thứ 2 sâu hơn ở phía dưới [NÓI].
* [ ] Giá xả mạnh chạm hoặc tiệm cận dải Lower Band và chạm vùng cản thứ 2 [NÓI].
* [ ] Nến rút chân rút râu mạnh mẽ và có giá đóng cửa nằm PHÍA TRÊN vùng cản thứ 2 [NÓI].

#### 4.3 Entry, SL & TP
* **Entry**: Vào lệnh Buy ngay khi nến rút chân đóng cửa phía trên cản 2 [NÓI/HÌNH].
* **Stop Loss**: Đặt dưới đáy râu nến vừa quét thủng cản 2 [HÌNH].
* **Take Profit**: Đặt tại các vùng đỉnh cũ hoặc mục tiêu sóng tăng tiếp diễn [HÌNH].

## 5. Case Study / Ví dụ chart

### Ví dụ 1: Kỹ thuật 1 – Chạm Band H1 hợp lưu SNR Kháng cự
* **Mốc thời gian**: 02:30 – 03:53 [HÌNH].
* **Sản phẩm & Khung thời gian**: Vàng (XAUUSD), khung H1 [HÌNH/NÓI].
* **Hướng lệnh**: Sell [NÓI].
* **Bối cảnh**: Xu hướng trước đó đang giảm, sau đó giá xuất hiện một nhịp hồi tăng mạnh [NÓI].
* **Diễn biến chart**:
  * Dải Upper Band H1 đang có chiều hướng chúi xuống [NÓI].
  * Phía trên đường Band có một vùng cản kháng cự SNR [HÌNH/NÓI].
  * Người thiếu kinh nghiệm sẽ vội vào lệnh Sell ngay khi giá chạm dải Band đang chúi xuống [NÓI].
  * Tác giả kiên nhẫn đợi giá đẩy cao thêm một nhịp nữa để chạm đúng vùng hợp lưu giữa Upper Band H1 và vùng SNR [NÓI].
* **Entry / SL / TP**:
  * Entry: Tại điểm hợp lưu giữa dải Upper Band H1 và đường kháng cự SNR [HÌNH/NÓI].
  * SL: Đặt trên vùng kháng cự SNR [HÌNH].
  * TP: Đặt ở vùng đáy cũ phía dưới (vùng màu xanh trên chart) [HÌNH].
* **Kết quả**: Giá chạm đúng vùng hợp lưu, rút râu và sập mạnh xuống theo kỳ vọng [HÌNH].

---

### Ví dụ 2: Kỹ thuật 2 – Phá Band M30 bám xu hướng giảm
* **Mốc thời gian**: 03:54 – 06:00 [HÌNH].
* **Sản phẩm & Khung thời gian**: Vàng (XAUUSD), khung M30 [HÌNH].
* **Hướng lệnh**: Sell theo xu hướng [NÓI].
* **Bối cảnh & Phân tích HTF**:
  * Kiểm tra Band khung D1, H4, H1: Thấy dải Band khung lớn còn ở sâu bên dưới, giá có xu hướng bị hút về đó [NÓI].
  * Ở M30: Vùng đáy cũ có nhiều râu nến (chứa thanh khoản). Khi giá quay lại quét lần 2, đáy này bị xuyên thủng [NÓI].
  * Nến M30 đóng cửa bám sát dải Band dưới; dải Band M30 mở rộng và chúc xuống rõ rệt [NÓI].
* **Thao tác lệnh**: Tác giả không đuổi theo cây nến xả, mà vẽ đường SNR phía trên và hướng dẫn chờ giá hồi (pullback) về vùng SNR này để thực hiện lệnh Sell bồi xuống [NÓI/HÌNH].

---

### Ví dụ 3: Kỹ thuật 3 – Quét thủng Middle Band D1 và đảo chiều tại cản 2
* **Mốc thời gian**: 06:14 – 07:47 [HÌNH].
* **Sản phẩm & Khung thời gian**: Vàng (XAUUSD), khung D1 [HÌNH/NÓI].
* **Hướng lệnh**: Buy đảo chiều sau cú quét SL [NÓI].
* **Bối cảnh**:
  * Xu hướng D1 trước đó là một trend tăng rất mạnh [NÓI].
  * Giá điều chỉnh về chạm Middle Band (trục giữa) D1 hợp lưu cản 1 -> có phản ứng nến xanh nhẹ [NÓI].
  * Nhiều người nhảy vào Buy tại cản 1 và đặt SL ngay dưới đáy đó [NÓI].
* **Cú quét (Trap)**: Một cây nến đỏ xả rất đậm, xuyên thủng Middle Band và đâm qua cản 1, quét sạch toàn bộ SL của phe Buy [NÓI].
* **Hành vi xử lý**:
  * Tác giả chỉ ra vùng cản thứ 2 nằm sâu hơn bên dưới, gần sát dải Lower Band D1 [NÓI/HÌNH].
  * Giá lao xuống cản 2, chạm gần Lower Band rồi rút râu dài, đóng cửa quay trở lại nằm trên cản 2 [NÓI].
  * Thực hiện lệnh Buy tại đây với SL dưới râu nến rút chân [HÌNH/NÓI].
* **Kết quả**: Giá đảo chiều bật tăng cực mạnh trở lại [HÌNH].

## 6. Tips, Tricks & Cảnh báo
* **Không sell/buy non khi chưa có hợp lưu**: Thấy dải Band chúc xuống không có nghĩa là đè ra sell ngay; phải xem phía trên có cản SNR đỡ hay không [NÓI].
* **Đặc tính khung thời gian của Band**: Cứ mỗi một cây nến đóng (ví dụ mỗi 1 tiếng ở H1), đường Band sẽ thay đổi vị trí, nhưng xét tổng thể cấu trúc thì vẫn giữ nguyên giá trị sử dụng [NÓI].
* **Đặc tính các phiên**: Sóng phá Band bám trend mạnh thường nổ ra ở phiên Mỹ; phiên Á và Âu đa số sideway, tránh áp dụng cứng nhắc kỹ thuật bám trend ở phiên Á/Âu [NÓI].
* **Đừng sợ bị quét SL**: Khi giá đã xuyên thủng cản, việc dính SL là bình thường. Cắt lỗ giúp bảo toàn vốn để canh cản thứ 2, tuyệt đối không trung bình giá hay dời SL [NÓI].

## 7. Quản trị rủi ro & Tâm lý
* **Quy tắc dừng lỗ dứt khoát**: Bị quét qua cản là bắt buộc phải thoát lệnh (STOP LOSS) [NÓI].
* **Giới hạn số lần thử**: Chỉ trade tối đa 1 đến 2 lần trên một vùng cản [NÓI]. Nếu thất bại 2 lần, vùng cản đó xem như vô hiệu, không được cố chấp bấm lệnh lần 3 [NÓI/SUY LUẬN].
* **Tâm lý chấp nhận kịch bản quét**: Cú xả đầu tiên sau một trend tăng mạnh bao giờ cũng sẽ có nhịp hồi kỹ thuật, do đó sau khi bị quét SL không nên hoảng loạn mà hãy bình tĩnh quan sát cản tiếp theo [NÓI].
* Con số Risk % tài khoản cụ thể cho mỗi lệnh: VIDEO KHÔNG ĐỀ CẬP [NÓI].

## 8. Đặc tả logic cho LLM / Bot

* ĐIỀU KIỆN CHUNG: QUẢN LÝ VÙNG CẢN
  * Gán biến `Trade_Count_At_Zone` = số lần đã vào lệnh tại vùng cản hiện tại.
  * `IF` `Trade_Count_At_Zone` >= 2:
    * `THEN` KHÔNG_MỞ_LỆNH_MỚI tại vùng cản này.
  * `IF` Giá đóng cửa vượt qua biên ngoài của vùng cản (xuyên thủng cản):
    * `THEN` ĐÓNG_TOÀN_BỘ_LỆNH (Hit SL), HỦY_VÙNG_CẢN hiện tại, chuyển sang tìm kiếm `Zone_Next`.

* LOGIC SETUP 1: REVERSAL TẠI VÙNG HỢP LƯU (BAND + SNR)
  * Khung thời gian áp dụng: `Timeframe` IN (`H1`, `H4`, `D1`).
  * ĐIỀU KIỆN BỐI CẢNH (SELL):
    * Xu hướng trước đó: Có nhịp tăng hồi phục mạnh.
    * Tồn tại vùng kháng cự `SNR_Resistance` phía trên.
    * Đường `Upper_Band` tiệm cận hoặc trùng khớp với `SNR_Resistance` (Hợp lưu).
  * TRIGGER & ENTRY (SELL):
    * `IF` `High` của nến chạm vào vùng hợp lưu (`Upper_Band` AND `SNR_Resistance`)
    * AND Nến xuất hiện râu từ chối giá (rút râu trên)
    * `THEN` Kích hoạt `ENTRY_SELL` (Market hoặc Limit tại mép cản).
  * STOP LOSS:
    * `SL_Price` = Mép trên của `SNR_Resistance` + `Buffer_Unspecified`.
  * TAKE PROFIT:
    * `TP_Price` = `UNSPECIFIED_IN_VIDEO` (Khuyến nghị hướng về `Middle_Band` hoặc đáy cũ).

* LOGIC SETUP 2: PHÁ BAND BÁM XU HƯỚNG (SELL TREND-FOLLOWING)
  * Khung thời gian phân tích: `HTF` IN (`H1`, `H4`, `D1`), `LTF` = `M30`.
  * ĐIỀU KIỆN LỌC:
    * Phiên giao dịch = `US_Session` (Phiên Mỹ).
    * Khoảng cách từ giá hiện tại đến `Lower_Band_HTF` còn rộng (còn dư địa giảm).
  * ĐIỀU KIỆN BỐI CẢNH (M30):
    * Trước đó dải Band co thắt sideway và hình thành đáy có nhiều râu nến (`Liquidity_Low`).
    * Dải `Lower_Band_M30` mở rộng và dốc xuống.
    * Nến M30 đâm thủng `Liquidity_Low` và đóng cửa nằm sát/ngoài `Lower_Band_M30`.
  * TRIGGER & ENTRY:
    * `IF` Giá xuất hiện nhịp hồi phục (`Pullback`) quay lại kiểm tra `Liquidity_Low` (bây giờ là Kháng cự SBR)
    * `THEN` Kích hoạt `ENTRY_SELL`.
  * SL & TP:
    * `SL_Price` = `UNSPECIFIED_IN_VIDEO`.
    * `TP_Price` = Vùng `Lower_Band_HTF`.

* LOGIC SETUP 3: BẮT ĐẢO CHIỀU SAU CÚ QUÉT THANH KHOẢN (SWEEP TRAP)
  * Khung thời gian áp dụng: `D1` (hoặc phiên Mỹ có tin `Non-Farm`, `FOMC`).
  * ĐIỀU KIỆN BỐI CẢNH (BUY):
    * Xu hướng chính trước đó = `Uptrend` mạnh.
    * Giá hồi về cản 1 (`Middle_Band_D1` hoặc `Support_1`), tạo phản ứng bật nhẹ rồi bị phá vỡ mạnh.
    * Xác định vùng cản thứ 2 sâu hơn (`Support_2`) nằm gần `Lower_Band_D1`.
  * TRIGGER & ENTRY (BUY):
    * `IF` Giá đâm xuyên thủng `Support_1` quét SL
    * AND Giá chạm / tiệm cận `Support_2` (hợp lưu gần `Lower_Band_D1`)
    * AND Nến đóng cửa rút chân với `Close` > Mép trên của `Support_2`
    * `THEN` Kích hoạt `ENTRY_BUY`.
  * STOP LOSS:
    * `SL_Price` = `Low` của cây nến vừa quét thủng `Support_2`.
  * TAKE PROFIT:
    * `TP_Price` = Đỉnh cũ trước cú xả [HÌNH].

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
* **Tham số chỉ báo**: Video hoàn toàn không đề cập đến chu kỳ (Period) và độ lệch (Deviation) của Bollinger Bands (mặc định phổ biến thường là 20, 2 nhưng video không xác nhận) [VIDEO KHÔNG ĐỀ CẬP].
* **Quy chuẩn nhận diện SNR**: Tác giả dùng các mức cản trực quan trên chart và slide "MSNR Key Levels" nhưng không định nghĩa chi tiết công thức xác định biên độ dày mỏng của vùng cản [VIDEO KHÔNG ĐỀ CẬP].
* **Khoảng cách hợp lưu**: Thế nào là "gần đường cản" hay "chạm cùng lúc" chưa được định lượng bằng số pip cụ thể, đòi hỏi sự quan sát chủ quan (SUBJECTIVE) bằng mắt [VIDEO KHÔNG ĐỀ CẬP].
* **Tỷ lệ R:R / Quản lý lệnh**: Không đưa ra quy tắc chốt lời từng phần (partial close) hay dời SL về hòa vốn (breakeven) [VIDEO KHÔNG ĐỀ CẬP].

## 10. Thông tin khác
* **Kênh phát hành**: Kênh YouTube / TikTok "TradingMienTrung" [HÌNH/NÓI].
* **Series**: "Series 100 Entry Trade Vàng", đây là Tập thứ 9 [HÌNH/NÓI].
* **Tài liệu tham khảo được nhắc tới**: Slide bảng mẫu "MSNR KEY LEVELS" (gồm Classic A, Classic V, SBR, RBS, OCL, QML) tác giả nhắc người xem xem lại các video cũ để hiểu rõ cách vẽ SNR [HÌNH/NÓI].
* **Quảng cáo / Kêu gọi**: Kêu gọi người xem bấm Like, Share, Follow kênh TradingMienTrung để theo dõi trọn bộ series 100 thế đánh vàng [NÓI].
* **Trích dẫn đáng chú ý**:
  * "Khi chúng ta trade tại những cái vùng cản, chúng ta chỉ trade từ 1 cho đến 2 lần... bắt buộc chúng ta phải thoát và chúng ta sẽ đợi ở vùng cản tiếp theo." [NÓI]
  * "Đường Band cộng với hợp lưu hỗ trợ hoặc kháng cự sẽ tăng cho chúng ta cái xác suất mà giá nó sẽ phản ứng nhiều hơn các bạn ha." [NÓI]
  * "Cái này nó là bài tủ của mình." [NÓI]