---
title: "Hướng dẫn phân biệt và giao dịch Order Block chất lượng cao theo phương pháp Smart Money Concepts"
source_author: "Yoshi Smart Trading"
video_duration: "12:30"
video_type:
  - "SMC / ICT"
  - "Price Action / Key Level / Cấu trúc đỉnh đáy"
  - "Hệ thống/EA/Bot/Quant (backtest)"
  - "Quản lý vốn, quản trị rủi ro"
markets:
  - "EURUSD"
  - "Forex chung"
timeframes_htf:
  - "4H"
  - "1H"
  - "15m"
timeframes_ltf:
  - "15m"
  - "5m"
  - "1m"
tools:
  - "Biểu đồ nến kỹ thuật"
  - "Thước đo Fibonacci Retracement (các mức 0.618 và 0.786)"
  - "Phần mềm backtest TraderEdge"
tags:
  - "Order Block"
  - "Smart Money Concepts"
  - "SMC"
  - "Inefficiency"
  - "Liquidity Grab"
  - "CHOCH"
  - "BOS"
  - "Multi-timeframe"
  - "TraderEdge"
  - "EURUSD"
extraction_confidence: "Cao – Video có cấu trúc trình bày trực quan, thuyết minh chi tiết kèm số liệu backtest và biểu đồ minh họa rõ ràng từng quy tắc."
---

# Hướng dẫn phân biệt và giao dịch Order Block chất lượng cao

## 0. TL;DR
- Video định nghĩa Order Block (OB) hợp lệ thông qua 3 quy tắc cốt lõi: phải tạo ra sự mất cân bằng (Inefficiency/Gap), phải dẫn đến phá vỡ cấu trúc (BOS) hoặc đổi đặc tính xu hướng (CHOCH), và phải là vùng chưa được xử lý (Unmitigated) [NÓI].
- Thử nghiệm kiểm tra lại (backtest) 100 setup cơ bản trên EURUSD khung 1H với R:R cố định 1:2 mang lại tỷ lệ thắng 43.06%, lợi nhuận +47.33%, Drawdown tối đa 9.93% dù winrate dưới 50% [HÌNH, NÓI].
- Để tăng tỷ lệ thắng, tác giả đề xuất hệ thống tính điểm (+1 / -1 point) dựa trên cấu trúc thanh khoản: trừ điểm nếu dưới OB có khoảng trống và một OB khác; cộng điểm nếu OB được hình thành sau cú quét thanh khoản đáy/đỉnh bằng nhau (Equal Lows/Highs) hoặc tạo bẫy thanh khoản trước OB [HÌNH, NÓI].
- Lọc bối cảnh giao dịch: ưu tiên các ngày giữa tuần, phiên London và New York, đánh thuận xu hướng chính, ưu tiên các OB mới hình thành (Recently printed OB) và phải tính toán phần chênh lệch giá (Spread) [NÓI].
- Quy trình vào lệnh nâng cao đa khung thời gian: xác định OB trên khung lớn (HTF), chuyển xuống khung nhỏ hơn 2 cấp (LTF) chờ CHOCH xác nhận; vào lệnh theo OB nhỏ kèm Inefficiency hoặc vào lệnh tại vùng hồi quy Fibonacci 0.618 - 0.786 nếu không có Inefficiency [HÌNH, NÓI].

---

## 1. Tổng quan
- **Mục tiêu / Vấn đề giải quyết:** Giải thích tại sao nhiều Order Block bị thị trường phớt lờ và xuyên thủng; đưa ra bộ tiêu chí định lượng và chấm điểm để lọc ra các Order Block xác suất thắng cao [NÓI].
- **Đối tượng phù hợp:** Người giao dịch theo trường phái SMC / Smart Money / Price Action muốn hệ thống hóa quy tắc chọn vùng POI/OB [SUY LUẬN: tác giả diễn giải từ quy tắc nền tảng đến bộ lọc nâng cao].
- **Thị trường & Khung thời gian áp dụng:**
  - Thị trường áp dụng trong video: Forex (cặp EURUSD) [HÌNH, NÓI]. Tuy nhiên tác giả nêu quy tắc không giới hạn cho bất kỳ cặp tiền hay khung thời gian nào [NÓI].
  - Phiên giao dịch tốt nhất: Phiên London và New York [NÓI].
  - Thời điểm trong tuần tốt nhất: Giữa tuần (thứ Ba đến thứ Năm) do có độ biến động cao; hạn chế ngày đầu tuần và cuối tuần vì thanh khoản thấp [HÌNH, NÓI].
  - Cặp khung thời gian đa khung (HTF -> LTF): 4H -> 15m; 1H -> 5m; 15m -> 1m [HÌNH, NÓI].
- **Công cụ & Thiết lập chỉ báo:**
  - Biểu đồ nến thuần túy (Price Action).
  - Fibonacci Retracement với 2 mốc xác lập: 0.618 và 0.786 [HÌNH, NÓI].
  - Phần mềm hỗ trợ kiểm thử: TraderEdge [HÌNH, NÓI].

---

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Cơ chế cốt lõi của Order Block:** Cây nến cuối cùng trước một đợt sóng mạnh tạo ra sự mất cân bằng được gọi là "Decision Candle" (cây nến quyết định). Đây là nơi các quyết định quan trọng của dòng tiền lớn (Smart Money) được đưa ra [HÌNH, NÓI].
- **Nguyên lý thanh khoản (Liquidity):** Thị trường di chuyển để tìm kiếm và quét thanh khoản. Đám đông nhỏ lẻ thường đặt Stop Loss phía dưới/trên các vùng đáy/đỉnh bằng nhau (Equal Lows/Highs) hoặc đáy swing rõ ràng. Smart Money sẽ kích hoạt các lệnh quét thanh khoản (Liquidity Grab) trước khi đẩy giá đi theo xu hướng thực tế [HÌNH, NÓI].
- **Cơ chế giảm thiểu (Mitigation):** Order Block chỉ phản ánh lượng lệnh tồn đọng một lần duy nhất. Sau khi giá quay lại chạm vùng này lần đầu tiên, các vị thế đã được xử lý xong, do đó các lần chạm tiếp theo không còn giá trị bảo vệ [NÓI].
- **Cung cầu cạnh tranh theo thời gian:** Thị trường liên tục biến động. Nếu giá mất quá nhiều thời gian mới quay lại OB cũ, phe đối lập đã có đủ thời gian thiết lập quyền kiểm soát, khiến OB cũ rất dễ thất bại [NÓI].

---

## 3. Thuật ngữ & Định nghĩa
| Thuật ngữ | Định nghĩa theo tác giả trong video | Cách nhận diện trên biểu đồ |
| :--- | :--- | :--- |
| **Order Block (OB)** | Vùng giá chứa cây nến quyết định tạo ra sự mất cân bằng và phá vỡ cấu trúc [NÓI]. | Thân và bóng của cây nến cuối cùng ngay trước nến kích hoạt sự mất cân bằng [HÌNH]. |
| **Decision Candle** | Cây nến cuối cùng trực tiếp tạo ra sự mất cân bằng giá [HÌNH]. | Nến trước chuỗi nến thân lớn tạo Gap [HÌNH]. |
| **Inefficiency / Gap** | Sự mất cân bằng cung cầu do bước giá di chuyển quá mạnh một chiều [NÓI]. | Khoảng trống giá giữa râu nến thứ 1 và râu nến thứ 3 trong cụm 3 nến liên tiếp [HÌNH]. |
| **BOS (Break of Structure)** | Sự phá vỡ cấu trúc đỉnh/đáy hiện tại theo xu hướng [HÌNH, NÓI]. | Giá đóng cửa vượt qua đỉnh cũ (uptrend) hoặc đáy cũ (downtrend) [HÌNH]. |
| **CHOCH (Change of Character)** | Tín hiệu thay đổi đặc tính/đặc điểm xu hướng từ tăng sang giảm hoặc ngược lại [HÌNH, NÓI]. | Giá phá vỡ đỉnh dẫn đến đáy thấp nhất hoặc đáy dẫn đến đỉnh cao nhất của nhịp ngắn hạn [HÌNH]. |
| **Unmitigated** | Vùng Order Block còn nguyên vẹn, giá chưa từng chạm vào kể từ khi hình thành [NÓI]. | Vùng OB chưa có bất kỳ râu hay thân nến nào hồi về chạm tới [HÌNH]. |
| **Liquidity Grab** | Cú quét thanh khoản để lấy thanh khoản từ các lệnh dừng lỗ của nhà giao dịch nhỏ lẻ [HÌNH, NÓI]. | Râu nến đâm xuyên qua vùng đỉnh/đáy hoặc vùng hỗ trợ/kháng cự rồi nhanh chóng rút lại [HÌNH]. |
| **Equal Lows / Equal Highs** | Các mức đáy hoặc đỉnh bằng nhau tạo thành vùng hỗ trợ/kháng cự rõ ràng [HÌNH]. | Hai hoặc nhiều đáy/đỉnh tạo thành đường nằm ngang song song có nhãn "$ Liquidity $" [HÌNH]. |

---

## 4. Hệ thống quy tắc

### 4.1. Ba quy tắc xác thực một Order Block hợp lệ (Bắt buộc)
1. **Quy tắc 1: Phải tạo ra sự mất cân bằng (Must Create Inefficiency):** Đợt dịch chuyển từ nến quyết định phải tạo ra khoảng trống (Gap) rõ rệt giữa bóng nến nến 1 và nến 3 [HÌNH, NÓI].
2. **Quy tắc 2: Phải phá vỡ cấu trúc hoặc đổi xu hướng (Must break structure or CHOCH):** Sóng đẩy từ OB phải phá vỡ đỉnh/đáy cấu trúc gần nhất [HÌNH, NÓI].
3. **Quy tắc 3: Phải chưa được xử lý (It must be unmitigated):** OB chỉ có giá trị ở lần chạm đầu tiên (First touch). Nếu đã chạm một lần rồi bật lên, vùng đó coi như đã hết hiệu lực cho các lệnh sau [HÌNH, NÓI].

---

### 4.2. Hệ thống chấm điểm chất lượng Order Block (Hệ thống +1 / -1 Point)
- **Điểm trừ (-1 point):**
  - Xuất hiện khi bên dưới OB1 có một khoảng trống giá (Gap) và một OB hợp lệ thứ hai (OB2) nằm ngay phía dưới [HÌNH, NÓI].
  - Hành vi thị trường: Giá có xu hướng bỏ qua OB1 để quét thanh khoản bên dưới OB1 nhằm lấp đầy Gap và kích hoạt OB2 [HÌNH, NÓI].
  - *Lưu ý quan trọng:* Việc giá xuyên thủng OB1 trong trường hợp này là "Invalid CHOCH" (CHOCH giả), không đồng nghĩa với đảo chiều xu hướng mà chỉ là Liquidity Grab [HÌNH, NÓI].
- **Điểm cộng (+1 point) – Loại A:**
  - Nhịp tạo ra OB đã thực hiện quét thanh khoản (Liquidity Grab) của các đáy/đỉnh bằng nhau (Equal Lows / Equal Highs) trước đó [HÌNH, NÓI].
- **Điểm cộng (+1 point) – Loại B:**
  - Trước khi giá tiếp cận OB, thị trường tạo ra các đáy bằng nhau (hỗ trợ nhỏ lẻ) ngay phía trên OB [HÌNH, NÓI].
  - Hành vi thị trường: Giá quét qua các đáy bằng nhau này để khớp thanh khoản Stop Loss của đám đông rồi mới chạm OB để tăng vọt [HÌNH, NÓI].

---

### 4.3. Chiến lược 1: Thiết lập vào lệnh cơ bản (Dùng trong mẫu Backtest 100 lệnh)
- **Điều kiện:** Xác định OB hợp lệ theo 3 quy tắc ở mục 4.1 [NÓI].
- **Entry:** Đặt lệnh Limit tại mép đầu của vùng OB (beginning of the zone) [HÌNH, NÓI].
- **Stop Loss:** Đặt ở mép cuối của vùng OB (end of the zone) [HÌNH, NÓI].
- **Take Profit:** Cố định tỷ lệ R:R = 1:2 (khoảng cách TP gấp 2 lần khoảng cách SL) [HÌNH, NÓI].
- **Hủy lệnh:** Hủy lệnh nếu giá không hồi về khớp mà tiếp tục đi xa hoặc cấu trúc bị vô hiệu hóa [HÌNH, NÓI].

---

### 4.4. Chiến lược 2: Thiết lập nâng cao đa khung thời gian (Confirmation Setups)
- **Bước 1 (Xác định bối cảnh HTF):**
  - Chờ giá hồi về chạm vào Order Block chưa xử lý trên khung lớn (4H, 1H hoặc 15m) [HÌNH, NÓI].
  - Đánh giá xu hướng: Chỉ ưu tiên đánh thuận xu hướng chính của thị trường [NÓI].
  - Đánh giá tuổi thọ OB: Ưu tiên các OB mới hình thành. Nếu là OB quá cũ và thị trường đã phá vỡ liên tiếp nhiều vùng Demand/Supply trên đường về, bắt buộc phải chờ xác nhận [HÌNH, NÓI].
- **Bước 2 (Chuyển xuống LTF):**
  - Chuyển xuống khung thời gian nhỏ hơn 2 cấp (4H -> 15m, 1H -> 5m, 15m -> 1m) [HÌNH, NÓI].
  - Chờ tín hiệu Thay đổi cấu trúc (Change of Character - CHOCH) xuất hiện trên LTF [HÌNH, NÓI].
- **Bước 3 (Vào lệnh theo 1 trong 2 kịch bản tại LTF):**
  - **Kịch bản A (Có Inefficiency trên LTF):**
    - Nhịp tạo CHOCH để lại khoảng trống mất cân bằng (Inefficiency) và tạo ra một LTF Order Block mới [HÌNH, NÓI].
    - *Entry:* Đặt lệnh mua/bán cách mép OB một khoảng bù trừ Spread (higher than OB by a spread range) [HÌNH, NÓI].
    - *Stop Loss:* Đặt cách đáy/đỉnh của vùng OB đó một vài pip [HÌNH, NÓI].
    - *Quản lý lệnh:* Dời Stop Loss về dưới các đáy cao hơn mới hình thành (Higher Lows) theo cấu trúc thị trường [HÌNH, NÓI].
    - *Take Profit:* Giữ lệnh cho đến khi giá chạm vào vùng Cung/Cầu đối diện ở khung thời gian lớn (Higher Timeframe Supply/Demand Zone) [HÌNH, NÓI].
  - **Kịch bản B (Không có Inefficiency trên LTF - Dùng Fibonacci):**
    - Nhịp tạo CHOCH đi mượt, không để lại khoảng trống Inefficiency [HÌNH, NÓI].
    - Kéo thước Fibonacci Retracement từ điểm bắt đầu nhịp CHOCH đến đỉnh kết thúc nhịp CHOCH [HÌNH, NÓI].
    - *Entry:* Đặt lệnh mua nằm ở giữa vùng hồi quy từ 0.618 đến 0.786 [HÌNH, NÓI].
    - *Stop Loss:* Đặt thấp hơn đáy swing (swing low) một vài pip [HÌNH, NÓI].
    - *Take Profit:* Đặt tại mức cấu trúc tiếp theo phía trước đường đi của giá [HÌNH, NÓI].

---

## 5. Case Study / Ví dụ chart

### 5.1. Ví dụ xác định đồng loạt các OB trên EURUSD M15
- **Mốc thời gian:** 01:54 – 02:16
- **Sản phẩm & Khung thời gian:** EURUSD – M15 [HÌNH, NÓI].
- **Bối cảnh:** Sóng tăng mạnh liên tục phá vỡ các đỉnh cấu trúc trước đó [HÌNH].
- **Phân tích:** Tác giả quét từ trái sang phải, xác định 5 cụm Inefficiency tương ứng với 5 cây nến quyết định. Cả 5 vùng đều thỏa mãn 3 điều kiện: có Inefficiency, tạo BOS/CHOCH và chưa bị chạm (Unmitigated) [HÌNH, NÓI].
- **Kết luận:** Đây là minh họa chuẩn cho việc lọc nến Order Block trên biểu đồ thời gian thực [NÓI].

---

### 5.2. Ví dụ 1 về cấu trúc: Trừ điểm OB vì có Gap và OB2 phía dưới
- **Mốc thời gian:** 04:40 – 05:24
- **Dạng biểu đồ:** Mô hình đồ họa minh họa [HÌNH].
- **Bối cảnh:** Giá tạo OB1 và bật lên tạo BOS. Tuy nhiên ngay dưới đáy OB1 có một vùng Gap và một OB2 hợp lệ [HÌNH].
- **Hành động giá:** Giá hồi về không giữ được OB1, đâm thủng tạo râu quét thanh khoản (Liquidity Grab), lấp Gap rồi phản ứng tại OB2 trước khi tăng vọt [HÌNH].
- **Đánh giá quy tắc:** OB1 bị gán nhãn `-1 point`. Hiện tượng thủng OB1 được gắn nhãn `Invalid ChoCh` [HÌNH].

---

### 5.3. Ví dụ 2 & 3 về cấu trúc: Cộng điểm OB nhờ quét thanh khoản
- **Mốc thời gian:** 05:25 – 06:09
- **Dạng biểu đồ:** Mô hình đồ họa minh họa [HÌNH].
- **Trường hợp 1 (05:25):** Đợt tạo sóng của OB đã quét qua cụm đáy bằng nhau (Equal Lows). Gán nhãn `+1 point` [HÌNH].
- **Trường hợp 2 (05:48):** Trước khi giá chạm vào OB, thị trường sideway tạo một đáy hỗ trợ có nhãn `$Liquidity$`. Sau đó nến làm một cú đâm xuống quét sạch thanh khoản rồi chạm OB đi lên. Gán nhãn `+1 point` [HÌNH].

---

### 5.4. Ví dụ thực tế: Cặp EURUSD 1H (Thủng OB trên để về OB dưới)
- **Mốc thời gian:** 06:11 – 06:40
- **Sản phẩm & Khung thời gian:** EURUSD – 1H [HÌNH, NÓI].
- **Bối cảnh:** Xu hướng tăng. Có một OB phía trên kèm Inefficiency và BOS [HÌNH].
- **Chi tiết chart:** Bên dưới OB trên có một vùng hỗ trợ tích tụ thanh khoản, tiếp theo là một khoảng trống Gap và một OB hợp lệ thứ hai nằm dưới đáy [HÌNH].
- **Kết quả:** Giá xuyên thủng hoàn toàn vùng OB thứ nhất, quét toàn bộ thanh khoản của vùng hỗ trợ, lấp đầy Gap, chạm chính xác vào OB thứ hai rồi mới tiếp tục xu hướng tăng mạnh [HÌNH, NÓI].

---

### 5.5. Ví dụ thực tế: Cặp EURUSD 1H (Bẫy thanh khoản trước OB)
- **Mốc thời gian:** 06:41 – 07:13
- **Sản phẩm & Khung thời gian:** EURUSD – 1H [HÌNH, NÓI].
- **Bối cảnh:** Nhịp tăng tạo BOS và để lại OB có Inefficiency [HÌNH].
- **Chi tiết chart:** Trước khi về tới OB, giá tạo cụm đáy bằng nhau ($ Liquidity $). Một nhịp giảm đâm thủng đáy này khiến nhiều trader tưởng là đảo chiều giảm (tín hiệu giảm giả), nhưng thực chất là Liquidity Grab chạm đúng vào OB rồi đảo chiều tăng vọt [HÌNH, NÓI].

---

### 5.6. Ví dụ xu hướng giảm: EURUSD 1H
- **Mốc thời gian:** 07:14 – 07:45
- **Sản phẩm & Khung thời gian:** EURUSD – 1H [HÌNH, NÓI].
- **Bối cảnh:** Xu hướng giảm rõ ràng (Down Trend) [HÌNH, NÓI].
- **Phân tích:** OB hình thành kèm Inefficiency và BOS đáy. Điểm mấu chốt là đỉnh của OB này xuất phát từ một cú quét thanh khoản đỉnh cũ (`Liquidity Grab`). Đạt điều kiện cộng điểm `+1 point` [HÌNH, NÓI].
- **Kết quả:** Giá hồi chạm mép OB và sập mạnh theo xu hướng chính [HÌNH].

---

### 5.7. Phản ví dụ: OB cũ bị đâm thủng khi phe Cung kiểm soát
- **Mốc thời gian:** 09:22 – 09:43
- **Bối cảnh:** Một vùng OB mua được hình thành từ rất lâu trước đó [HÌNH].
- **Hành động giá:** Khi giá hồi về, trên đường rơi xuống nó liên tục tạo các vùng Demand mới nhưng đều bị phá vỡ dễ dàng [HÌNH, NÓI].
- **Kết quả:** Phe Bán (Supply) đã hoàn toàn làm chủ thị trường, OB cũ bị đâm thủng thẳng cánh mà không có phản ứng bật tăng. Video ghi chú: "Trade with Confirmation Only" (Chỉ giao dịch khi có tín hiệu xác nhận) [HÌNH, NÓI].

---

### 5.8. Minh họa Setup xác nhận LTF: EURUSD (Kịch bản Inefficiency & Kịch bản Fibonacci)
- **Mốc thời gian:** 10:38 – 12:20
- **Kịch bản A (10:38 - 11:45):**
  - Giá chạm HTF OB.
  - Trên LTF xuất hiện CHOCH tạo Inefficiency và OB mới.
  - Đặt Limit mua cách mép OB một khoảng Spread, SL cách đáy vài pip.
  - Giá tăng, trader dời SL theo các Higher Low cho tới khi chạm HTF Supply zone [HÌNH, NÓI].
- **Kịch bản B (11:46 - 12:08):**
  - Giá chạm HTF OB, xuất hiện CHOCH nhưng không có Inefficiency (No Inefficiency).
  - Kéo Fibonacci Retracement cho nhịp tăng CHOCH.
  - Đặt lệnh mua Limit ở vùng giữa Fib 0.618 và 0.786. SL dưới Swing Low vài pip. TP tại đỉnh cấu trúc kế tiếp [HÌNH, NÓI].

---

## 6. Tips, Tricks & Cảnh báo
- **Xử lý Spread:** Thị trường thường phản ứng với OB chỉ trong phạm vi 1 pip. Nếu giao dịch cặp có Spread giãn, lệnh Limit đặt sát mép có thể không khớp (bỏ lỡ lệnh thắng) hoặc dính SL sớm trước khi giá chạm mức SL thực tế. Luôn cộng thêm Spread vào điểm Entry khi Mua [NÓI].
- **Bộ lọc ngày trong tuần:** Hầu hết lệnh thắng xảy ra vào giữa tuần (thứ Ba, Tư, Năm). Tránh hoặc cẩn trọng vào thứ Hai và thứ Sáu do thị trường thường mỏng thanh khoản [HÌNH, NÓI].
- **Ưu tiên độ mới của OB:** Luôn ưu tiên các OB mới hình thành (Recently printed OB). OB tồn tại quá lâu thường mất đi lực đỡ do dòng tiền đã tái phân phối [NÓI].
- **Cảnh báo CHOCH giả (Invalid CHOCH):** Khi một OB bị đâm thủng nhưng ngay phía dưới còn một OB hợp lệ khác kèm Gap, việc thủng đó thường chỉ là Liquidity Grab chứ không phải là đảo chiều xu hướng [HÌNH, NÓI].
- **Tâm lý khi thua lỗ:** Mỗi khi dính lệnh thua, điều đó không đồng nghĩa với việc phân tích bị sai; không có phương pháp nào đạt tỷ lệ thắng 100% vì trader không thể kiểm soát thị trường [HÌNH, NÓI].

---

## 7. Quản trị rủi ro & Số liệu Backtest
Tác giả công bố bảng kết quả chi tiết kiểm thử trên phần mềm TraderEdge [HÌNH, NÓI]:
- **Kích thước tài khoản ban đầu:** $10,000 [HÌNH, NÓI].
- **Rủi ro mỗi lệnh (Risk per trade):** 2% tài khoản ($200 ở lệnh đầu) [HÌNH, NÓI].
- **Mục tiêu lợi nhuận mỗi lệnh (Target Profit):** 4% tài khoản (tỷ lệ R:R cố định 1:2) [HÌNH, NÓI].
- **Số lượng setup kiểm tra:** 100 setup trên cặp EURUSD khung 1H [HÌNH, NÓI].
- **Số lệnh hủy / Không kích hoạt:** 28 setup (chiếm 28%) [HÌNH, NÓI].
- **Tổng số lệnh thực thi:** 72 lệnh [HÌNH, NÓI].
- **Số lệnh thắng / thua:** 31 Thắng (Win) / 41 Thua (Loss) [HÌNH, NÓI].
- **Tỷ lệ thắng (Winrate):** 43.06% [HÌNH, NÓI].
- **Tỷ lệ hòa vốn lý thuyết:** 34% (với R:R 1:2) [NÓI].
- **Tỷ số lợi nhuận / thua lỗ (Profit Factor):** 1.51 [HÌNH].
- **Chỉ số Edge Score:** 82.27 [HÌNH].
- **Mức sụt giảm tài khoản tối đa (Max Drawdown):** 9.93% (làm tròn 10% trong lời nói) [HÌNH, NÓI].
- **Lợi nhuận ròng (Net PnL):** +47.33% (tương đương +$4,733.37, số dư đạt $14,733.37) [HÌNH, NÓI].
- **Chuỗi lệnh:** Thắng liên tiếp nhiều nhất (Consecutive Wins) = 3 lệnh; Thua liên tiếp nhiều nhất (Consecutive Losses) = 5 lệnh [HÌNH].

---

## 8. Đặc tả logic cho LLM / Bot

Quy tắc logic cho kịch bản MUA (LONG) với thiết lập xác nhận đa khung thời gian:
(Quy tắc BÁN / SHORT được áp dụng đối xứng hoàn toàn)

- ĐIỀU KIỆN BỐI CẢNH (HTF):
  - `HTF_Timeframe` thuộc danh sách [`4H`, `1H`, `15m`].
  - `LTF_Timeframe` tương ứng là [`15m`, `5m`, `1m`].
  - `Market_Trend` trên `HTF_Timeframe` == `BULLISH`.
  - Tồn tại một vùng `HTF_OB` thỏa mãn đồng thời:
    - `Has_Inefficiency` == `TRUE` (tồn tại khoảng trống giữa nến 1 và nến 3).
    - `Break_Structure` == `TRUE` (tạo BOS đỉnh gần nhất).
    - `Is_Unmitigated` == `TRUE` (chưa từng bị giá chạm sau khi tạo thành).
    - `Is_Recent` == `TRUE` (không phải OB tồn tại quá nhiều chu kỳ nến).

- ĐIỀU KIỆN LỌC THANH KHOẢN (Chấm điểm OB):
  - Gán `Score` = 0.
  - IF có khoảng trống `Gap` và một `Valid_OB_2` nằm ngay dưới `HTF_OB`:
    - `Score` = `Score` - 1.
    - Đặt trạng thái `HTF_OB` là `HIGH_RISK_LIQUIDITY_RUN`.
  - IF `HTF_OB` được tạo ra sau cú quét qua `Equal_Lows`:
    - `Score` = `Score` + 1.
  - IF xuất hiện cụm `Equal_Lows` tích lũy ngay phía trên `HTF_OB`:
    - `Score` = `Score` + 1.
  - Lọc ngày và phiên:
    - `Day_Of_Week` thuộc [`Tuesday`, `Wednesday`, `Thursday`].
    - `Session` thuộc [`London_Session`, `New_York_Session`].

- TRIGGER (Kích hoạt trên LTF):
  - Giá trên `LTF_Timeframe` chạm vào vùng `HTF_OB` lần đầu tiên.
  - Chờ xuất hiện `LTF_CHOCH` (giá phá vỡ đỉnh swing ngắn hạn gần nhất tạo tín hiệu tăng).

- ENTRY:
  - Trường hợp 1: Nhịp tăng tạo `LTF_CHOCH` có để lại `LTF_Inefficiency`:
    - Xác định vùng `LTF_OB` tại cây nến quyết định.
    - `Entry_Price` = `LTF_OB.High` + `Current_Spread`.
    - `SL_Price` = `LTF_OB.Low` - `Buffer_Pips` (với `Buffer_Pips` = `UNSPECIFIED_IN_VIDEO`, thường là 1-3 pips).
  - Trường hợp 2: Nhịp tăng tạo `LTF_CHOCH` không có Inefficiency (`Has_LTF_Inefficiency` == `FALSE`):
    - Kéo Fibonacci Retracement từ đáy nhịp CHOCH đến đỉnh nhịp CHOCH.
    - `Entry_Price` = Giá trị trung bình nằm giữa mức `Fib_0.618` và `Fib_0.786`.
    - `SL_Price` = `Swing_Low` - `Buffer_Pips`.

- QUẢN LÝ LỆNH & TRAILING SL:
  - Khi giá di chuyển theo hướng dự đoán và tạo thành một `New_Higher_Low` rõ ràng trên cấu trúc:
    - Dời `SL_Price` về ngay dưới đáy của `New_Higher_Low` đó.
  - Lặp lại quy trình trailing theo mỗi đáy cao dần mới tạo.

- TAKE PROFIT:
  - Đối với setup cơ bản: `TP_Price` = `Entry_Price` + 2 * (`Entry_Price` - `SL_Price`).
  - Đối với setup nâng cao có Confirmation:
    - Kịch bản 1: Đóng toàn bộ lệnh khi giá chạm vùng `HTF_Supply_Zone`.
    - Kịch bản 2 (dùng Fib): Đóng lệnh tại mức đỉnh cấu trúc kế tiếp (`Next_Structure_Resistance`).

- ĐIỀU KIỆN HỦY:
  - Giá xuyên thủng hoàn toàn vùng `HTF_OB` mà không hình thành bất kỳ tín hiệu `LTF_CHOCH` nào.
  - Lệnh chờ Limit không được khớp và giá đã tăng chạm mục tiêu TP trước khi hồi về.

---

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Khoảng cách đệm của Stop Loss:** Tác giả nói đặt SL cách mép OB "a few pips" (vài pip) để trừ hao spread và trượt giá, nhưng không quy định số pip cụ thể là 1, 2 hay 5 pip [NÓI].
- **Độ mới của Order Block:** Tác giả nhấn mạnh nên chọn "Recently printed Order Blocks" và tránh OB quá cũ, nhưng không đưa ra con số định lượng cụ thể (ví dụ: trong vòng bao nhiêu cây nến hay bao nhiêu phiên) [NÓI].
- **Mức chênh lệch điểm (Score threshold):** Hệ thống tính điểm có quy tắc cộng 1 điểm (+1) và trừ 1 điểm (-1), nhưng không công bố ngưỡng điểm tối thiểu để được phép vào lệnh (ví dụ: đạt bao nhiêu điểm thì được phép vào Limit trực tiếp, khi nào bắt buộc phải chờ Confirmation) [SUY LUẬN: tác giả chỉ minh họa logic tăng giảm xác suất chứ chưa đóng gói thành bảng tính điểm hoàn chỉnh].
- **Quy tắc dời SL chi tiết:** Trong phần trailing stop, tác giả hướng dẫn dời SL dưới "higher low", nhưng không nêu tiêu chí cụ thể để xác nhận một swing low đã hoàn tất (ví dụ: cần nến đóng cửa vượt đỉnh cũ hay chỉ cần râu nến) [NÓI].

---

## 10. Thông tin khác
- **Công cụ phần mềm được nhắc tới:** Phần mềm TraderEdge (trang web Traderedge.com) dùng để lưu trữ nhật ký và backtest dữ liệu giao dịch [HÌNH, NÓI].
- **Kết quả kiểm chứng:** Kết quả backtest 100 lệnh đạt lợi nhuận +47.33% với Max Drawdown 9.93% được thực hiện bởi chính tác giả trên phần mềm TraderEdge với cặp EURUSD, chưa có bên thứ ba độc lập kiểm chứng [HÌNH, NÓI].
- **Lời kêu gọi hành động:** Tác giả kêu gọi người xem nhấn nút Like và Subscribe cho kênh Yoshi Smart Trading ở giữa và cuối video [HÌNH, NÓI].
- **Trích dẫn đáng chú ý:**
  - *"Every time you encounter a losing trade, it does not necessarily mean a certain error in your analysis. Remember that no strategy works all the time because we cannot control the market."* [HÌNH, NÓI]