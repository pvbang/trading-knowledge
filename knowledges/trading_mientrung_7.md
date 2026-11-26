---
title: "Kỹ thuật nhận biết sớm đảo chiều và Entry Scalping Vàng sau khi quét thanh khoản (Tập 7)"
source_author: "TradingMienTrung"
video_duration: "00:49"
video_type:
  - Price Action / Key Level / Cấu trúc đỉnh đáy / Mô hình nến, mô hình giá
  - SMC / ICT (Liquidity, FVG/Imbalance, OB, Breaker, BOS/CHOCH, Inducement, Killzone, Premium/Discount)
  - Wyckoff / Elliott / Harmonic / Fibonacci / Gann / Chu kỳ
  - Review lệnh / Live trading / Backtest / Q&A / Kiến thức nền cho người mới
markets:
  - Vàng (XAUUSD)
timeframes_htf:
  - KHÔNG RÕ (Video không hiển thị nhãn khung thời gian cụ thể trên chart)
timeframes_ltf:
  - KHÔNG RÕ (Video không hiển thị nhãn khung thời gian cụ thể trên chart)
tools:
  - Trendline (đường xu hướng)
  - Horizontal Line (vùng kháng cự/hỗ trợ)
tags:
  - Scalping Vàng
  - Quét thanh khoản
  - Liquidity Sweep
  - Wyckoff Spring
  - Kháng cự chuyển hỗ trợ
  - Retest
  - Tin tức FED
  - Đảo chiều xu hướng
  - TradingMienTrung
extraction_confidence: "Cao – Nội dung video ngắn, trực quan, các bước vào lệnh và quy tắc xác nhận đảo chiều được giải thích và vẽ minh họa rõ ràng từng bước."
---

# Kỹ thuật nhận biết sớm đảo chiều và Entry Scalping Vàng sau khi quét thanh khoản (Tập 7)

## 0. TL;DR
- Nhận biết sớm khả năng đảo chiều từ giảm sang tăng của Vàng thông qua 2 yếu tố: cây nến biến động mạnh do tin tức (ví dụ tin FED lãi suất) và hành vi quét thanh khoản vùng đáy cũ (tương tự pha Spring trong Wyckoff).
- Không bắt đáy ngay tại râu quét thanh khoản; quy tắc cốt lõi là chờ xác nhận đảo chiều khi cụm nến xanh tăng vượt và bao phủ hoàn toàn cây nến đỏ giảm mạnh trước đó.
- Điểm vào lệnh (Entry Scalping): Chờ giá hồi test lại vùng kháng cự vừa bị phá vỡ (vùng đỉnh của nến đỏ/cản ngang vừa chuyển thành hỗ trợ).
- Tiếp tục nhồi lệnh/tìm thêm Entry bằng cách chờ giá phá đỉnh tạo cấu trúc tăng tiếp diễn rồi retest đỉnh cũ.

## 1. Tổng quan
- **Mục tiêu / vấn đề giải quyết:** Cách nhận biết sớm và giao dịch đảo chiều khi giá Vàng đang trong một xu hướng giảm rõ ràng [NÓI].
- **Đối tượng phù hợp:** Người giao dịch Scalping Vàng, người muốn nắm bắt sớm nhịp đảo chiều nhưng cần có xác nhận an toàn thay vì bắt dao rơi [SUY LUẬN].
- **Thị trường & sản phẩm áp dụng:** Vàng (Gold / XAUUSD) [NÓI].
- **Khung thời gian áp dụng:** VIDEO KHÔNG ĐỀ CẬP (không thấy nhãn Timeframe trên biểu đồ TradingView trong video).
- **Công cụ & Thiết lập chỉ báo:** Giao dịch hoàn toàn bằng biểu đồ nến trần (Price Action / SMC), kết hợp vẽ Trendline giảm và các mốc cản ngang (Key Level/Đỉnh/Đáy) [HÌNH].

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Cơ chế quét thanh khoản (Liquidity Sweep):** Thị trường giữ giá tại một vùng đáy nhất định, sau đó tạo một cú hồi ngắn rồi tin tức ra làm giá xả mạnh đâm thủng đáy cũ nhằm lấy hết thanh khoản (stop loss của phe Buy hoặc kích hoạt sell stop) [NÓI].
- **Hành vi giá sau quét thanh khoản:** Sau khi lấy thanh khoản, thị trường lập tức rút râu và bật tăng mạnh trở lại; đây là dấu hiệu cốt lõi của các pha đảo chiều dòng tiền lớn [NÓI].
- **Bản chất theo trường phái Wyckoff:** Tác giả liên hệ cú quét thanh khoản đáy này tương đồng với sự kiện **"Spring"** trong phương pháp Wyckoff tích lũy [NÓI].
- **Chuyển đổi vai trò Kháng cự - Hỗ trợ:** Khi lực cầu đủ mạnh đẩy giá vượt qua cây nến giảm mạnh trước đó, vùng kháng cự cũ bị đâm thủng lập tức chuyển đổi thành vùng hỗ trợ, có nhiệm vụ đỡ giá không cho giảm tiếp [NÓI].
- **Đặc tính sóng hồi của Vàng khi đảo chiều:** Khi Vàng vừa mới đảo chiều xu hướng, giá rất ít khi quét sâu về các vùng OTE (Optimal Trade Entry - vùng Fibonacci thoái lui sâu) mà thường chỉ hồi nhẹ về kiểm tra (retest) các vùng hỗ trợ gần nhất rồi tiếp tục tăng [NÓI].

## 3. Thuật ngữ & Định nghĩa
| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **Quét thanh khoản (Liquidity Sweep)** | Hành động giá xả mạnh đâm thủng đáy cũ đã tạo trước đó rồi rút chân [NÓI]. | Giá thò đuôi nến hoặc thân nến vượt qua đáy trước nhưng nhanh chóng bật ngược lại [HÌNH]. |
| **Spring** | Khái niệm trong Wyckoff tương đương với hành động quét thanh khoản đáy [NÓI]. | Nhịp rũ bỏ phá vỡ giả cạnh dưới của vùng đi ngang tích lũy [HÌNH]. |
| **Nến tin tức (Cây nến FED)** | Cây nến biên độ lớn xuất hiện khi có sự kiện kinh tế lớn (FED công bố lãi suất) [NÓI]. | Nến có thân hoặc râu nến dài đột biến so với cấu trúc nến xung quanh [HÌNH]. |
| **Xác nhận đảo chiều (Confirm)** | Trạng thái lực tăng đã triệt tiêu hoàn toàn lực giảm trước đó [NÓI]. | Cụm nến xanh tăng vượt qua và bao phủ hoàn toàn cây nến đỏ giảm mạnh trước đó [NÓI, HÌNH]. |
| **Kháng cự hóa Hỗ trợ** | Mức đỉnh cản cục bộ bị nến xanh phá vỡ, chuyển thành vùng đỡ giá [NÓI]. | Kẻ đường nằm ngang qua đỉnh nến đỏ; khi giá vượt lên trên thì đường này đóng vai trò hỗ trợ [HÌNH]. |
| **OTE (Optimal Trade Entry)** | Vùng tối ưu để vào lệnh hồi quy (thường là vùng Fibo sâu) [NÓI]. | Vùng tác giả nhấn mạnh giá Vàng thường **bỏ qua** (không quét sâu về) khi vừa đảo chiều [NÓI]. |

## 4. Hệ thống quy tắc giao dịch (Setup Scalping Đảo Chiều Vàng)

### 4.1 Điều kiện tiên quyết / Confluence (Checklist)
- [ ] Thị trường trước đó đang nằm trong một xu hướng giảm rõ ràng (nhìn thấy đỉnh đáy thấp dần, tôn trọng trendline giảm) [NÓI, HÌNH].
- [ ] Xuất hiện một vùng đáy tích lũy đỡ giá tạm thời [HÌNH].
- [ ] Xuất hiện cây nến biến động mạnh do tin tức (như tin FED thay đổi lãi suất) [NÓI].
- [ ] Có hành vi quét thanh khoản: Giá xả xuống đâm thủng đáy cũ rồi lập tức rút râu tăng ngược trở lại [NÓI].

### 4.2 Xác định bối cảnh & Hướng (Bias)
- Sau khi giá quét thanh khoản đáy và rút râu, chuyển thiên hướng (bias) sang chuẩn bị canh Mua (Buy), nhưng **chưa được vào lệnh ngay** [NÓI].
- Chờ xác nhận chuyển đổi cấu trúc từ giảm sang tăng hoàn tất [NÓI].

### 4.3 Tín hiệu kích hoạt (Trigger)
- Tìm cây nến đỏ giảm mạnh cuối cùng tạo ra đỉnh cản gần nhất [HÌNH].
- Tín hiệu kích hoạt xảy ra khi: Toàn bộ cây nến đỏ này bị cụm nến xanh tăng vượt qua hoàn toàn (cụm nến xanh bao phủ hoàn toàn cây nến đỏ) [NÓI].
- Đỉnh của cây nến đỏ này được đánh dấu làm mốc kháng cự quan trọng vừa bị phá vỡ [HÌNH].

### 4.4 Quy tắc Entry
- **Loại lệnh:** Chờ giá hồi về kiểm tra (Limit hoặc Market khi giá chạm vùng) [SUY LUẬN].
- **Entry 1 (Vị trí chính):** Đặt lệnh Buy khi giá quay trở lại retest vùng kháng cự vừa bị phá (đỉnh nến đỏ chuyển thành hỗ trợ) [NÓI, HÌNH].
- **Entry 2+ (Quy tắc thêm lệnh / Scale-in):** 
  - Đợi giá phá vỡ đỉnh cao gần nhất vừa tạo ra [NÓI].
  - Chờ giá hồi về retest lại đỉnh vừa phá để tiếp tục Buy Scalping theo xu hướng tăng mới [NÓI, HÌNH].

### 4.5 Stop Loss (SL)
- VIDEO KHÔNG ĐỀ CẬP quy tắc đặt số pip hay vị trí đặt SL cụ thể trong video này.
- [SUY LUẬN]: Dựa theo hình minh họa slide trong video (00:01 và 00:30), SL thường được kéo về dưới râu nến quét thanh khoản hoặc dưới đáy cây nến bật tăng gần nhất.

### 4.6 Take Profit (TP) / Quản lý lệnh
- VIDEO KHÔNG ĐỀ CẬP tỷ lệ R:R hay số pips chốt lời cụ thể.
- Tác giả nêu định hướng: Trong xu hướng tăng tiếp theo chỉ tập trung canh Buy scalping theo các nhịp phá vỡ đỉnh và retest [NÓI].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- Không bắt đáy mua ngay tại thời điểm cây nến tin tức vừa quét đáy rút râu (tránh rủi ro đoán đáy sớm khi chưa có confirm) [NÓI].
- Nếu giá không tạo được cụm nến xanh vượt qua đỉnh cây nến đỏ giảm mạnh, không tiến hành giao dịch Buy [SUY LUẬN].

## 5. Case Study / Ví dụ chart

### Ví dụ chính trong video: Cấu trúc đảo chiều Vàng
- **Mốc thời gian:** 00:00 – 00:49
- **Sản phẩm:** Vàng (XAUUSD) [NÓI].
- **Khung thời gian:** KHÔNG RÕ [HÌNH].
- **Hướng lệnh:** BUY (Scalping) [NÓI].
- **Bối cảnh trước setup:** 
  - Thị trường đang ở xu hướng giảm thể hiện rõ qua đường trendline dốc xuống nối các đỉnh giảm dần [00:25].
  - Giá tạo một vùng đáy đi ngang tạm thời [01:14].
- **Diễn biến & Thao tác của tác giả:**
  - Tin FED ra mắt, xuất hiện cây nến đỏ xả cực mạnh quét xuyên qua vùng đáy trước đó [00:50 - 01:24].
  - Giá rút râu mạnh từ vùng dưới đáy cũ, đóng nến đẩy ngược lên [01:33]. Tác giả giải thích đây là hành vi quét thanh khoản (hoặc Spring theo Wyckoff).
  - Tiếp theo, một chuỗi nến xanh tăng mạnh xuất hiện, vượt qua hoàn toàn đỉnh của cây nến đỏ giảm mạnh trước đó [02:58]. Tác giả kẻ một đường ngang qua đỉnh nến đỏ này và ghi nhận kháng cự đã bị đâm thủng [03:26].
  - Giá hồi nhẹ về đúng đường ngang này (quét nhẹ qua râu nến cũ) rồi bật tăng tiếp [03:38].
  - Tác giả vẽ sơ đồ mũi tên: Chờ giá phá tiếp đỉnh swing high bên trên, test lại đỉnh để mở thêm các vị thế Buy scalping tiếp theo [04:01].
- **Entry / SL / TP cụ thể:** Không hiển thị mức giá số liệu cụ thể trên trục giá.
- **Bài học rút ra:** Không cần vội vã bắt đáy khi giá vừa quét râu; chờ nhịp bao phủ xác nhận rồi đánh nhịp pullback test cản sẽ an toàn và có xác suất cao hơn [NÓI].

## 6. Tips, Tricks & Cảnh báo
- **Không vội bắt đáy sớm:** "Cái đoạn quét thanh khoản hồi nãy là mình chưa trade nhá" – cần đợi thị trường xác nhận thực sự đảo chiều mới vào lệnh [NÓI].
- **Đặc điểm biên độ hồi của Vàng:** Đừng chờ giá Vàng hồi sâu về OTE khi đảo chiều, vì động lượng Vàng khi đổi chiều thường rất mạnh, giá chỉ test các vùng cản gần (kháng cự hóa hỗ trợ) là đã bay tiếp [NÓI].
- **Tập trung vào 1 chiều:** Khi xác nhận đảo chiều thành công sang xu hướng tăng, quy tắc là chỉ tập trung canh Buy, không đánh ngược chiều [NÓI].

## 7. Quản trị rủi ro & Tâm lý
- VIDEO KHÔNG ĐỀ CẬP (Video thuộc dạng Short/Reel tập trung vào kỹ thuật nhận diện cấu trúc và entry, không đề cập số % rủi ro, lot size hay quản lý vốn).

## 8. Đặc tả logic cho LLM / Bot

Quy tắc logic cho kịch bản BUY đảo chiều (mô hình quét thanh khoản + hấp thụ nến giảm):

- `ĐIỀU KIỆN BỐI CẢNH:`
  - `Trend_HTF` == `DOWNTREND` (xác định qua cấu trúc đỉnh/đáy thấp dần hoặc dưới trendline giảm)
  - Tồn tại vùng hỗ trợ đáy gần nhất `Support_Level`
- `ĐIỀU KIỆN LỌC (THANH KHOẢN):`
  - Xuất hiện nến giảm mạnh đâm thủng `Support_Level` (`Low` < `Support_Level`)
  - Giá không duy trì dưới `Support_Level` mà rút chân đóng nến tạo râu quét thanh khoản (`Liquidity_Swept` == `TRUE`)
- `TRIGGER (XÁC NHẬN ĐẢO CHIỀU):`
  - Xác định cây nến đỏ giảm mạnh chịu trách nhiệm trước cú quét: `Red_Candle_High`
  - Cụm nến xanh tăng trưởng phá vỡ hoàn toàn đỉnh nến đỏ: `Close_Current` > `Red_Candle_High`
  - Chuyển trạng thái thị trường: `Resistance_To_Support` = `Red_Candle_High`
- `ENTRY:`
  - `Entry_Type` = `LIMIT_OR_MARKET_ON_TOUCH`
  - `Entry_Price` = `Resistance_To_Support` (chờ giá pullback kiểm tra lại mức đỉnh nến đỏ cũ)
- `ENTRY BỔ SUNG (SCALE-IN):`
  - Khi giá tạo đỉnh cao mới `New_High` > `Previous_High`
  - Chờ giá hồi về: `Entry_Add_Price` = `New_High`
- `STOP LOSS (SL):`
  - `SL_Price` = `UNSPECIFIED_IN_VIDEO` (tác giả không đưa quy tắc SL cụ thể; gợi ý logic theo hình: đặt dưới đáy râu nến quét thanh khoản `Swing_Low`)
- `TAKE PROFIT (TP):`
  - `TP_Price` = `UNSPECIFIED_IN_VIDEO`
- `ĐIỀU KIỆN HỦY KÈO:`
  - Giá quay trở lại đóng nến nằm hoàn toàn dưới `Resistance_To_Support` mà không có phản ứng rút râu đẩy lên.

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Khung thời gian:** Biểu đồ che khuất nhãn timeframe (không rõ là M1, M5, M15 hay H1). Do tác giả nhắc tới từ khóa "Scalping Vàng" và "tin tức FED", nhiều khả năng áp dụng trên khung nhỏ (M1 - M15), nhưng video không xác nhận chính thức.
- **Stop Loss và Take Profit:** Video hoàn toàn không đề cập vị trí đặt SL, điểm TP mục tiêu hay tỷ lệ Risk:Reward cho lệnh.
- **Tài liệu tham khảo nội bộ:** Tác giả có nhắc đến tài liệu "SNR của bên TradingMienTrung", nhưng không trình bày chi tiết nội dung tài liệu này trong video.

## 10. Thông tin khác
- **Kênh phát hành:** TradingMienTrung [NÓI, HÌNH].
- **Series:** "Series 100 Entry Scalping Vàng" – Video là Tập 7 [NÓI, HÌNH].
- **Tài liệu được giới thiệu:** Tài liệu "SNR - TradingMienTrung" (hướng dẫn về các cặp nến tạo hỗ trợ/kháng cự và cách nến đóng cửa vượt qua cản) [HÌNH, NÓI].
- **Quảng cáo / Kêu gọi hành động:** Kêu gọi bình luận để nhận tài liệu SNR và bấm follow kênh TradingMienTrung để theo dõi các tập tiếp theo của series [NÓI].
- **Trích dẫn đáng chú ý:**
  - *"Quét thanh khoản là yếu tố cốt lõi của những cái pha đảo chiều."* [01:40]
  - *"Khi mà giá Vàng nó vừa mới đảo chiều á thì rất là ít khi mà Vàng nó quét về sâu để mà nó test những cái vùng như là OTE..."* [04:13]