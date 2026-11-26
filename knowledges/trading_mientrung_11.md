---
title: "Nhận diện Nến Thanh Khoản và Quét Thanh Khoản tại Swing High/Swing Low kết hợp vùng OTE (Tập 11 - Series 100 Entry Scalping Vàng)"
source_author: "TradingMienTrung"
video_duration: "04:50"
video_type: ["Price Action / Key Level / Cấu trúc đỉnh đáy", "SMC / ICT (Liquidity, OTE)", "Fibonacci"]
markets: ["XAUUSD"]
timeframes_htf: ["VIDEO KHÔNG ĐỀ CẬP"]
timeframes_ltf: ["VIDEO KHÔNG ĐỀ CẬP"]
tools: ["Fibonacci Retracement (tìm vùng OTE)"]
tags: ["Nến thanh khoản", "Quét thanh khoản", "Liquidity Sweep", "Swing High", "Swing Low", "OTE", "Fake Breakout", "Scalping Vàng", "XAUUSD"]
extraction_confidence: "Cao – Hình ảnh đồ họa minh họa và lời nói rõ ràng, nhưng thiếu thông số khung thời gian cụ thể và quy tắc trigger vào lệnh chi tiết."
---

# Nhận diện Nến Thanh Khoản và Quét Thanh Khoản tại Swing High/Swing Low kết hợp vùng OTE (Tập 11 - Series 100 Entry Scalping Vàng)[cite: 1]

## 0. TL;DR
- Giải quyết bài toán "Entry là SL" khi trader đánh máy móc theo công thức phá cản hồi lại (Sell tại kháng cự hoặc Buy ngay khi vừa phá đỉnh trong xu hướng giảm)[cite: 1].
- Bản chất chuyển động giá: Khi giá không đủ lực đi tiếp theo xu hướng, nó cần "quét thanh khoản" qua các mốc `Swing High` hoặc `Swing Low` để "lấy đà" trước khi di chuyển mạnh theo hướng ngược lại[cite: 1].
- Trong xu hướng giảm, cần xác định cấu trúc gồm `Swing Low` - `Swing High` - `Swing Low` và chờ giá quét qua `Swing High` để lấy thanh khoản phe Sell trước khi sập xuống[cite: 1].
- Nếu giá đã quét `Swing High` gần nhất và đạp xuống nhưng không phá được đáy (dập dìu đi lên lại), nghĩa là giá cần tìm vùng thanh khoản cao hơn tại vùng `OTE` (đo bằng Fibonacci Retracement của con sóng giảm lớn trước đó)[cite: 1].

---

## 1. Tổng quan
- **Mục tiêu / vấn đề video giải quyết**:
  - Khắc phục tình trạng vào lệnh bị quét Stop Loss ngay lập tức ("Entry là SL") khi giao dịch theo công thức truyền thống: thấy giá phá cản giảm xuống, đợi hồi lên kháng cự để Sell, hoặc thấy giá vừa phá cản trên liền canh hồi lại để Buy ngược xu hướng chính[cite: 1].
  - Bổ sung kiến thức về "nến thanh khoản" để tối ưu vị thế giao dịch, giúp trader tự tin gồng lệnh dài hạn theo xu hướng và hạn chế việc chốt non[cite: 1].
- **Đối tượng phù hợp**: Những người muốn "học trade mẹo, học trade cho nó gọi là nhanh có hiệu quả" [NÓI][cite: 1].
- **Thị trường, sản phẩm, khung thời gian, phiên giao dịch áp dụng**:
  - Thị trường / Sản phẩm: Vàng (`XAUUSD`) – thuộc "Series 100 Entry Scalping Vàng" [NÓI] / "Series 100 Entry Trade Vàng" [HÌNH][cite: 1]. (Các ví dụ trên chart hiển thị mức giá quanh vùng 2616 - 2690 [HÌNH] và ảnh chụp MT4/MT5 ở vùng 4063 - 4274 [HÌNH])[cite: 1].
  - Khung thời gian: VIDEO KHÔNG ĐỀ CẬP[cite: 1].
  - Phiên giao dịch: VIDEO KHÔNG ĐỀ CẬP[cite: 1].
- **Công cụ & thiết lập chỉ báo**:
  - Biểu đồ nến Nhật thuần (Price Action) kết hợp vẽ đường cấu trúc sóng và vùng cản [HÌNH][cite: 1].
  - Công cụ **Fibonacci Retracement** để xác định vùng `OTE` [NÓI, HÌNH][cite: 1]. Các mốc hiển thị trên công cụ Fibo trong video (tại 04:03): `0`, `0.5`, `0.618`, `0.705`, `0.79`, `1` [HÌNH][cite: 1]. Vùng `OTE` được tô màu cam nằm giữa mốc `0.618` và `0.79` [HÌNH][cite: 1].

---

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Luận điểm cốt lõi theo lời tác giả**:
  - Giá muốn giảm xuống thì cần phải "quét lên để lấy thêm lực mua thì nó mới giảm được" [NÓI][cite: 1].
  - Khi giá đi ngang hoặc di chuyển yếu ớt ("tăng mà nó tăng không nổi" hoặc "không giảm tiếp được, tạo đáy"), điều đó có nghĩa là thị trường đang "thiếu thanh khoản" để đi tiếp [NÓI][cite: 1].
  - Để có đủ lực ("lấy đà"), giá sẽ thực hiện hành vi quét qua các mốc `Swing Low` (quét thanh khoản phe Buy / tạo `Fake Breakout`) để lấy đà tăng lên, hoặc quét qua các mốc `Swing High` (quét thanh khoản phe Sell) để lấy đà giảm xuống [NÓI, HÌNH][cite: 1].
  - Nếu đã quét một vùng thanh khoản gần nhưng giá vẫn không giảm sâu được, nghĩa là vẫn "còn cái vùng thanh khoản ở phía trên cao hơn cần phải quét" (vùng `OTE` của sóng lớn) [NÓI][cite: 1].
- **Điều kiện thị trường phù hợp**: Thị trường có xu hướng chính rõ ràng (ví dụ trong video là một `Trend Giảm` rõ ràng trước đó) [NÓI, HÌNH][cite: 1].
- **Giả định ngầm của phương pháp**: Các vùng đỉnh `Swing High` và đáy `Swing Low` là nơi tập trung thanh khoản (Stop Loss của các trader vào lệnh sớm hoặc lệnh chờ Breakout), và thị trường luôn di chuyển từ vùng thanh khoản này sang vùng thanh khoản khác để lấy nhiên liệu cho xu hướng chính [SUY LUẬN – dựa trên cách tác giả giải thích việc quét phe Buy/phe Sell để lấy đà][cite: 1].

---

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **Swing Low** | Đáy cấu trúc sóng nơi tập trung thanh khoản của phe Buy [NÓI, HÌNH][cite: 1]. | Điểm đảo chiều từ giảm sang tăng trên biểu đồ; được dùng làm mốc để quan sát hành vi quét râu hoặc phá vỡ giả bên dưới [HÌNH][cite: 1]. |
| **Swing High** | Đỉnh cấu trúc sóng hồi nơi tập trung thanh khoản của phe Sell [NÓI, HÌNH][cite: 1]. | Điểm đảo chiều từ tăng sang giảm trong nhịp hồi của xu hướng giảm; nơi các trader thường đặt kháng cự để canh Sell hoặc SL [HÌNH][cite: 1]. |
| **Nến thanh khoản / Nến quét thanh khoản** | Cây nến hoặc cụm nến thực hiện hành vi phá vỡ giả (`Fake Breakout`) qua `Swing High` hoặc `Swing Low` để "lấy đà" rồi đảo chiều ngay sau đó [NÓI, HÌNH][cite: 1]. | Nến đâm xuyên qua đường ngang vẽ từ `Swing High` hoặc `Swing Low` trước đó, sau đó giá lập tức đi ngược lại hướng vừa phá vỡ với lực rất mạnh [HÌNH][cite: 1]. |
| **Quét thanh khoản phe Buy** | Hành vi giá đạp xuống dưới `Swing Low` để lấy thanh khoản, tạo đà tăng lên [NÓI, HÌNH][cite: 1]. | Giá đi ngang không tăng nổi, sau đó nhúng xuống thủng đáy `Swing Low` gần nhất (tạo `Fake Breakout`) rồi bật tăng mạnh [NÓI, HÌNH][cite: 1]. |
| **Quét thanh khoản phe Sell** | Hành vi giá đẩy vượt lên trên `Swing High` để lấy thanh khoản, tạo đà giảm xuống [NÓI, HÌNH][cite: 1]. | Giá đẩy tăng vượt qua đỉnh `Swing High` gần nhất (khiến trader lầm tưởng là phá cản đi lên) rồi ngay lập tức sập mạnh xuống theo xu hướng giảm chính [NÓI, HÌNH][cite: 1]. |
| **OTE** | Vùng thanh khoản cao hơn được xác định bằng công cụ Fibonacci khi giá đã quét `Swing High` gần nhưng chưa giảm luôn được [NÓI, HÌNH] (Được tác giả nhắc là kiến thức ở bài số 10) [NÓI][cite: 1]. | Kéo Fibonacci từ đỉnh xuống đáy của nhịp giảm lớn trước đó; vùng `OTE` là hộp chữ nhật nằm trong khoảng từ mức Fibo `0.618` đến `0.79` (bao gồm mốc `0.705`) [HÌNH][cite: 1]. |

---

## 4. Hệ thống quy tắc

Video trình bày 2 kịch bản giao dịch chính dựa trên hành vi quét thanh khoản trong bối cảnh xu hướng giảm:
- **Chiến lược A**: Giao dịch theo nhịp quét thanh khoản cấu trúc `Swing High` / `Swing Low` cơ bản (và biến thể đánh đảo chiều tăng nếu giá đạp thẳng xuống lấy đà)[cite: 1].
- **Chiến lược B**: Giao dịch Sell tại vùng `OTE` khi nhịp giảm sau quét `Swing High` thất bại (giá dập dìu không giảm tiếp được)[cite: 1].

### 4.1 Điều kiện tiên quyết / Confluence (Checklist)
- [ ] Xác định được xu hướng chính trước đó (trong video lấy ví dụ là một `Trend Giảm` mạnh và rõ ràng) [NÓI, HÌNH][cite: 1].
- [ ] Xác định rõ 3 điểm cấu trúc sau nhịp giảm mạnh: một `Swing Low` (đáy thấp nhất của nhịp giảm), một `Swing High` (đỉnh nhịp hồi lên), và một `Swing Low` thứ hai (đáy nhịp chỉnh tiếp theo cao hơn đáy đầu tiên) [NÓI, HÌNH][cite: 1].
- [ ] Quan sát xem giá đã thực hiện hành vi "quét thanh khoản hay chưa và vùng thanh khoản đó nó nằm ở đâu" [NÓI][cite: 1].

### 4.2 Xác định bối cảnh & hướng (Bias)
- **Xu hướng chủ đạo (Bias chính)**: Canh **Sell Swing dài hạn theo xu hướng** giảm chính sau khi giá hoàn tất việc quét thanh khoản phía trên [NÓI][cite: 1].
- **Nhận diện quá trình tích lũy lấy đà trước khi sập**:
  1. Từ `Swing Low` thứ hai, nếu giá tăng lên nhưng "tăng không nổi" (đi ngang zíc zắc trong biên độ hẹp) -> báo hiệu đang thiếu thanh khoản [NÓI, HÌNH][cite: 1].
  2. Giá sẽ đạp xuống quét qua `Swing Low` thứ hai ("quét thanh khoản phe Buy" / tạo cú `Fake Breakout`) để lấy đà tăng mạnh lên [NÓI, HÌNH][cite: 1].
  3. Nhịp tăng mạnh này sẽ đâm xuyên lên trên đỉnh `Swing High` trước đó để "quét thanh khoản phe Sell" [NÓI, HÌNH][cite: 1].
  4. Sau khi quét xong `Swing High`, mục tiêu tiếp theo của giá là giảm rất mạnh xuống dưới để quét lại `Swing Low` bên dưới [NÓI, HÌNH][cite: 1].

### 4.3 Tín hiệu kích hoạt (Trigger)
- **Với lệnh Sell ngay sau khi quét `Swing High` (Minh họa đầu video 00:18 - 00:38)**:
  - Xuất hiện "nến thanh khoản" đâm lên quét qua `Swing High`, sau đó đóng nến giảm mạnh quay ngược trở lại xuống dưới mức `Swing High` [HÌNH][cite: 1].
- **Với kịch bản tiếp diễn sau khi giá đã quét `Swing High` và đang đạp xuống (03:38 - 04:15)**:
  - **Trường hợp 1 (Canh Buy khi giá đạp thủng đáy lấy đà)**: Sau khi quét `Swing High` và đang đạp xuống rất đẹp, nếu giá "đạp luôn" (phá thủng qua cả vùng `Swing Low` thấp nhất trước đó để lấy đà) rồi "đi lên lại" -> Kích hoạt kịch bản canh Buy [NÓI, HÌNH][cite: 1].
  - **Trường hợp 2 (Canh Sell tại OTE khi giá không đạp xuống được)**: Nếu sau khi quét `Swing High` và đạp xuống lưng chừng, giá "không đạp được", chỉ giảm tới ngang vùng đáy phụ rồi "dập dìu nó lên lại" -> Nghĩa là còn vùng thanh khoản cao hơn chưa quét. Lúc này kéo Fibonacci trên con sóng giảm lớn trước đó để tìm vùng `OTE` phía trên `Swing High` và đợi giá quét lên vùng `OTE` này rồi mới đạp xuống [NÓI, HÌNH][cite: 1].

### 4.4 Entry (Loại lệnh & Vị trí)
- Video không nói bằng lời loại lệnh cụ thể (Market hay Limit), nhưng hiển thị qua công cụ vẽ vị thế Long/Short trên TradingView [HÌNH][cite: 1]:
  - **Entry Sell sau nến quét `Swing High` (tại 00:18 - 00:38)**: Đặt ngay sau khi cây nến giảm mạnh đóng cửa dưới `Swing High` vừa bị quét [HÌNH][cite: 1].
  - **Entry Buy sau nến quét `Swing Low` (tại 00:18 - 00:38)**: Đặt tại vùng đáy ngay sau khi nến quét qua `Swing Low` và rút chân/đóng nến bật lên [HÌNH][cite: 1].
  - **Entry Buy khi giá đạp thủng đáy lớn lấy đà đi lên lại (tại 03:48)**: Đặt ở nhịp bắt đầu vòng lên sau cú đạp sâu qua đáy [HÌNH][cite: 1].
  - **Entry Sell tại vùng `OTE` (tại 04:12)**: Đặt tại mép dưới của hộp `OTE` (tương ứng mức Fibo `0.618`, mức giá hiển thị trên hình là `2674.88`) khi giá tăng dập dìu lên chạm vùng này [HÌNH][cite: 1].

### 4.5 Stop Loss (Quy tắc đặt, khoảng cách)
- Video không phát biểu quy tắc bằng lời (VIDEO KHÔNG ĐỀ CẬP bằng lời nói), chỉ thể hiện qua hộp vị thế trên biểu đồ [HÌNH][cite: 1]:
  - **Với lệnh Sell sau khi quét `Swing High` (00:18)**: SL đặt phía trên đỉnh râu cao nhất của cụm nến vừa quét `Swing High` [HÌNH][cite: 1].
  - **Với lệnh Buy sau khi quét `Swing Low` (00:18)**: SL đặt phía dưới râu thấp nhất của cụm nến vừa quét `Swing Low` [HÌNH][cite: 1].
  - **Với lệnh Sell tại vùng `OTE` (04:12)**: SL đặt phía trên hộp `OTE` (quanh mức Fibo `0.79` - `0.85`, mức giá hiển thị trên hình là `2685.25`, tương ứng khoảng cách `10.37` giá / `1037` pip trên nhãn công cụ đo) [HÌNH][cite: 1].

### 4.6 Take Profit / Quản lý lệnh
- **Với lệnh Buy từ cú quét `Swing Low` lấy đà (00:18)**: TP đặt tại vùng đỉnh khi giá quét qua `Swing High` [HÌNH][cite: 1].
- **Với lệnh Sell sau khi quét `Swing High` (00:18)**: TP kéo dài xuống dưới đáy `Swing Low` thấp nhất bên dưới [HÌNH][cite: 1].
- **Với lệnh Sell tại vùng `OTE` (04:12)**: TP đặt tại vùng đáy thấp nhất của cấu trúc (`Swing Low` đầu tiên, mức giá hiển thị trên hình là `2616.53`, tương ứng khoảng cách `58.35` giá / `5835` pip, tỷ lệ R:R hiển thị là `5.63`) [HÌNH][cite: 1].
- **Quản lý lệnh (partial, breakeven, trailing)**: VIDEO KHÔNG ĐỀ CẬP[cite: 1].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo (Các bẫy cần tránh)
- **KHÔNG Sell sớm tại kháng cự thông thường** khi giá vừa phá cản đi xuống rồi hồi lên lần đầu mà chưa hiểu cấu trúc quét thanh khoản (vì rất dễ bị quét SL như ví dụ đầu video) [NÓI, HÌNH][cite: 1].
- **KHÔNG canh Buy khi thấy giá vừa phá lên trên `Swing High` (phá cản)** trong một xu hướng chính là `Trend Giảm`: Việc giá vượt `Swing High` thực chất chỉ là hành vi quét thanh khoản phe Sell để lấy đà sập mạnh xuống quét `Swing Low` bên dưới. Đợi hồi về cản đó để Buy sẽ bị dính SL liên tục [NÓI, HÌNH][cite: 1].
- **KHÔNG canh Sell đuổi khi giá vừa quét `Swing Low` (tạo `Fake Breakout`) và đang bật tăng mạnh**: Sau cú quét đáy để lấy đà đi lên quét đỉnh, lực tăng rất mạnh, "cứ Sell là SL, Sell là SL" [NÓI, HÌNH][cite: 1].
- **KHÔNG cố Sell ngay dưới thấp nếu sau khi quét `Swing High` mà giá không giảm tiếp được**: Khi giá ngừng giảm và dập dìu bò lên lại, phải chuyển sang đợi giá lên quét vùng thanh khoản cao hơn ở `OTE` [NÓI, HÌNH][cite: 1].

---

## 5. Case Study / Ví dụ chart

### 5.1 Ví dụ 1: Tình huống "Entry là SL" khi Sell tại kháng cự thông thường
- **Mốc thời gian**: `00:00` – `00:16`[cite: 1].
- **Sản phẩm, khung thời gian, hướng lệnh**: Sản phẩm & Khung thời gian KHÔNG RÕ (biểu đồ nến trắng/xanh/đỏ); Hướng lệnh: **SHORT (Sell)** [HÌNH][cite: 1].
- **Bối cảnh trước setup**: Giá đang trong nhịp giảm, đi ngang tạo vùng đáy nhỏ rồi đạp mạnh xuống "phá cản" [NÓI, HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Vẽ vùng kháng cự màu vàng ngang qua đỉnh nhịp tích lũy trước khi giá phá đáy [HÌNH][cite: 1].
  - Giá giảm xuống rồi tăng "hồi lên lại" chạm đúng vùng kháng cự màu vàng [NÓI, HÌNH][cite: 1].
  - Trader áp dụng công thức máy móc: "giá giảm xuống, hồi lên, Sell tại kháng cự" [NÓI, HÌNH][cite: 1].
- **Entry / SL / TP cụ thể**: Đặt lệnh Sell ngay tại vùng kháng cự màu vàng, SL đặt ngay phía trên vùng vàng, TP kỳ vọng về lại đáy cũ [HÌNH][cite: 1]. (Không hiện mức giá cụ thể).
- **Kết quả và bài học tác giả rút ra**: Cây nến xanh tăng thẳng xuyên qua vùng kháng cự và chạm SL ngay lập tức ("Entry là SL") [NÓI, HÌNH][cite: 1]. Đây là phản ví dụ mở đầu để chỉ ra sai lầm phổ biến khi không nhận diện được việc giá hồi lên để quét thanh khoản[cite: 1].

### 5.2 Ví dụ 2: Phân tích cấu trúc Quét Thanh Khoản `Swing Low` và `Swing High` trong Trend Giảm
- **Mốc thời gian**: `00:17` – `02:23`[cite: 1].
- **Sản phẩm, khung thời gian, hướng lệnh**: Cùng một đoạn biểu đồ được dùng xuyên suốt để giải thích cả chiều Buy ngắn hạn (lấy đà) và Sell theo xu hướng chính [HÌNH][cite: 1].
- **Bối cảnh trước setup**: Trước đó là một `Trend Giảm` rất mạnh và rõ ràng [NÓI, HÌNH][cite: 1]. Sau nhịp giảm mạnh, giá tạo đáy `Swing Low` thứ nhất, hồi lên tạo `Swing High`, rồi giảm điều chỉnh tạo `Swing Low` thứ hai (cao hơn `Swing Low` thứ nhất) [NÓI, HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  1. Từ `Swing Low` thứ hai, giá đi zíc zắc trong một hộp màu đỏ với chú thích "tăng không nổi" -> do thiếu thanh khoản để giảm tiếp [NÓI, HÌNH][cite: 1].
  2. Giá đạp xuống xuyên qua `Swing Low` thứ hai (vùng gạch đỏ "quét thanh khoản phe buy") để lấy đà [NÓI, HÌNH][cite: 1]. Tại `00:18`, tác giả minh họa một lệnh Buy ngay tại điểm quét đáy này ("nến thanh khoản") ăn lên tới đỉnh [HÌNH][cite: 1].
  3. Từ cú quét đáy đó, giá bật tăng vọt lên vượt qua đỉnh `Swing High` ("quét thanh khoản phe sell") [NÓI, HÌNH][cite: 1].
  4. Tác giả chỉ ra sai lầm tại `01:55`: Nhiều người thấy giá vượt `Swing High` thì tưởng là "phá cản" nên đặt lệnh Buy khi giá hồi về vùng `Swing High` đó [NÓI, HÌNH][cite: 1].
- **Entry / SL / TP cụ thể**:
  - **Lệnh sai lầm (Phản ví dụ tại 01:57 & 02:13)**: Đặt lệnh Buy tại mức ngang `Swing High` vừa bị phá, SL dưới vùng cản đó -> Bị cây nến đỏ dài đâm thủng SL ngay lập tức [HÌNH][cite: 1].
  - **Lệnh đúng theo phương pháp (Thuận ví dụ tại 00:18 - 00:38)**:
    - Lệnh 1 (Buy): Entry ngay sau nến quét `Swing Low` thứ hai, SL dưới râu nến quét, TP tại vùng trên `Swing High` [HÌNH][cite: 1].
    - Lệnh 2 (Sell): Entry ngay sau khi cụm "nến thanh khoản" quét xong `Swing High` và đóng nến đỏ sập xuống lại dưới `Swing High`, SL trên đỉnh râu quét, TP kéo sâu xuống dưới `Swing Low` thấp nhất [HÌNH][cite: 1].
- **Kết quả và bài học tác giả rút ra**: Sau khi quét `Swing High`, giá sập thẳng một mạch qua luôn cả `Swing Low` bên dưới ("quét Swing Low, giảm rất là mạnh") [NÓI, HÌNH][cite: 1]. Bài học: Phải luôn chú ý (1) các vùng `Swing High` - `Swing Low` và (2) xu hướng chính trước đó là `Trend Giảm` [NÓI][cite: 1].

### 5.3 Ví dụ 3: Quét đáy `Fake Breakout` khi không giảm tiếp được & Kịch bản kết hợp vùng `OTE`
- **Mốc thời gian**: `02:24` – `04:17`[cite: 1].
- **Sản phẩm, khung thời gian, hướng lệnh**: Vàng (`XAUUSD` – mức giá hiển thị từ `2616.53` đến `2690.07` ở giây `04:03` - `04:14`), khung thời gian KHÔNG RÕ [HÌNH][cite: 1].
- **Bối cảnh trước setup**: Giá đã có nhịp giảm mạnh đầu tiên, hồi lên quét thanh khoản ở phía trên `Swing High` và đạp mạnh xuống tạo `Swing Low` [NÓI, HÌNH][cite: 1].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - **Giai đoạn 1 (`02:31` – `03:05` - Quét đáy lấy đà tăng)**:
    - Sau khi đạp xuống, giá đi ngang zíc zắc trong hộp đỏ ("không giảm tiếp được, tạo đáy") [NÓI, HÌNH][cite: 1].
    - Trước khi quay lên lấy đà, giá làm một cú rích xuống dưới đáy hộp tạo `Fake Breakout` ("Nến Quét Thanh Khoản" / "quét thanh khoản của phe buy") [NÓI, HÌNH][cite: 1].
    - Ngay sau cú quét đáy này, "lực tăng nó mạnh quá, cứ Sell là SL, Sell là SL" (trên hình vẽ minh họa một lệnh Sell bị dính SL trong vùng mũi tên xanh "Lực Tăng Mạnh") [NÓI, HÌNH][cite: 1].
  - **Giai đoạn 2 (`03:06` – `03:37` - Quét đỉnh nhưng chưa giảm sâu được)**:
    - Nhịp tăng mạnh đó đẩy giá lên quét qua đỉnh `Swing High` phía trên rồi bắt đầu đạp xuống [NÓI, HÌNH][cite: 1].
  - **Giai đoạn 3 (`03:38` – `04:15` - Hai kịch bản xử lý và đo `OTE`)**:
    - *Kịch bản giả định 1 (`03:43` - `03:48`)*: Nếu nhịp đạp xuống này "đạp luôn" xuyên thủng đáy thấp nhất bên dưới để lấy đà rồi vòng lên lại -> sẽ có một lệnh Buy rất đẹp [NÓI, HÌNH][cite: 1].
    - *Kịch bản thực tế / giả định 2 (`03:49` - `04:15`)*: Giá "không đạp được", chỉ giảm tới ngang vùng đáy phụ ở giữa rồi "dập dìu nó lên lại" [NÓI, HÌNH][cite: 1]. Điều này chứng tỏ còn vùng thanh khoản cao hơn ở phía trên cần quét [NÓI][cite: 1].
    - Tác giả kéo công cụ Fibonacci từ đỉnh cao nhất bên trái (`2690.07` - mức `1`) xuống đáy thấp nhất (`2616.53` - mức `0`) để xác định vùng `OTE` nằm phía trên `Swing High` vừa quét [NÓI, HÌNH][cite: 1].
- **Entry / SL / TP cụ thể (Cho lệnh Sell tại vùng `OTE` ở `04:12`)**:
  - **Hướng lệnh**: **SHORT (Sell)** [HÌNH][cite: 1].
  - **Entry**: `2674.88` (ngay mép dưới vùng `OTE` / mức Fibo `0.618`) [HÌNH][cite: 1].
  - **Stop Loss**: `2685.25` (phía trên hộp `OTE` / trên mức Fibo `0.79`, rủi ro `10.37` giá / `1037` pip) [HÌNH][cite: 1].
  - **Take Profit**: `2616.53` (tại đáy `Swing Low` mức Fibo `0`, lợi nhuận mục tiêu `58.35` giá / `5835` pip, tỷ lệ `R:R = 5.63`) [HÌNH][cite: 1].
- **Kết quả và bài học tác giả rút ra**: Đây là biểu đồ đang chạy/vẽ kịch bản dự phóng về tương lai để minh họa cách kết hợp kiến thức quét thanh khoản (Bài 11) và vùng `OTE` (Bài 10) nhằm xác định điểm giá sẽ quét lên tới đâu trước khi sập thật sự [NÓI, HÌNH][cite: 1].

### 5.4 Ví dụ 4 & 5: Ảnh chụp màn hình kết quả gồng lời thực tế (Show lệnh)
- **Mốc thời gian**: `04:19` – `04:23`[cite: 1].
- **Chi tiết hiển thị trên màn hình**:
  - **Ảnh 1 (`04:20` - `04:21`)**: Biểu đồ trên điện thoại, lệnh `BUY 1` có lãi `+9,656.00 USD`, điểm vào lệnh quanh vùng đáy `4063.840`, giá hiện tại đang ở `4159.108` [HÌNH][cite: 1].
  - **Ảnh 2 (`04:21` - `04:22`)**: Biểu đồ trên điện thoại có kẻ Fibonacci mở rộng (`0.0`, `23.6`, `38.2`, `50.0`, `61.8`, `100.0`, `161.8`, `261.8`, `423.6`), lệnh `BUY 2` có lãi `+19,969.00 USD`, điểm vào lệnh ở vùng đáy `4080.939`, giá tăng vọt qua mốc `261.8` (`4274.578`) [HÌNH][cite: 1].
- **Mục đích của tác giả**: Minh họa việc áp dụng công thức quét thanh khoản giúp gồng được những lệnh rất xa, đồng thời khẳng định với người xem đây là lệnh đã từng show trên kênh chứ không phải backtest hay demo [NÓI][cite: 1].

---

## 6. Tips, Tricks & Cảnh báo
- **Dấu hiệu nhận biết thị trường thiếu thanh khoản**:
  - Trong xu hướng giảm, nếu giá hồi lên mà "tăng không nổi" (cứ đi zíc zắc ngang) nghĩa là đang thiếu thanh khoản -> Cẩn thận giá sẽ nhúng xuống quét `Swing Low` trước để lấy đà bật tăng lên quét `Swing High` [NÓI, HÌNH][cite: 1].
  - Ngược lại, sau khi đã quét `Swing High` và đạp xuống nhưng giá "không giảm tiếp được, tạo đáy" đi ngang -> Cẩn thận giá sẽ làm một cú `Fake Breakout` quét xuống dưới đáy đó để lấy đà tăng rất mạnh lên trên [NÓI, HÌNH][cite: 1].
- **Bẫy chết người khi đánh Breakout / Phá cản**:
  - Thấy giá vừa phá lên qua `Swing High` trong một `Trend Giảm` thì tuyệt đối không vội canh hồi về cản để Buy, vì đó thường chỉ là cú quét thanh khoản phe Sell trước khi sập mạnh về đáy cũ [NÓI, HÌNH][cite: 1].
- **Bẫy chặn tàu sau cú quét đáy (`Fake Breakout`)**:
  - Khi giá vừa làm cú `Fake Breakout` quét qua `Swing Low` để lấy đà đi lên tìm thanh khoản phía trên, lực tăng sẽ cực kỳ mạnh -> Tuyệt đối không nhảy vào cản đường Sell lưng chừng vì "cứ Sell là SL" [NÓI, HÌNH][cite: 1].
- **Cách xử lý khi giá đã quét `Swing High` nhưng vẫn không sập sâu được**:
  - Đừng cố chấp giữ kỳ vọng giá sập ngay nếu thấy nó giảm nửa vời rồi dập dìu bò lên lại. Hãy hiểu rằng thanh khoản ở `Swing High` vừa rồi chưa đủ và giá đang đi tìm vùng thanh khoản cao hơn tại `OTE` (đo bằng Fibo của nhịp giảm lớn trước đó) [NÓI, HÌNH][cite: 1].

---

## 7. Quản trị rủi ro & Tâm lý
- **Tâm lý gồng lời**: Hiểu rõ vị trí các vùng thanh khoản (`Swing High`, `Swing Low`, `OTE`) và việc giá đã quét thanh khoản hay chưa sẽ giúp trader có vị thế đẹp, từ đó "tự tin gồng lệnh và hạn chế được cái việc chốt non" [NÓI][cite: 1].
- **Các quy tắc quản lý vốn định lượng (Risk % mỗi lệnh, cách tính lot, giới hạn lỗ ngày/tuần)**: VIDEO KHÔNG ĐỀ CẬP[cite: 1].

---

## 8. Đặc tả logic cho LLM / Bot

Dưới đây là cấu trúc hóa các quy tắc nhận diện và vào lệnh được trình bày trong video (chủ yếu cho bối cảnh **Trend Giảm**; chiều **Trend Tăng** không được trình bày trong video nên ghi nhận theo đúng dữ liệu gốc):

- **ĐIỀU KIỆN BỐI CẢNH (CONTEXT)**:
  - `Primary_Trend == DOWNTREND` (`SUBJECTIVE:` Một nhịp giảm mạnh và dài rõ ràng trước đó trên chart)[cite: 1].
  - Sau nhịp giảm mạnh, giá hình thành 3 mốc cấu trúc tuần tự:
    - `Swing_Low_1`: Đáy thấp nhất kết thúc nhịp giảm mạnh đầu tiên[cite: 1].
    - `Swing_High_1`: Đỉnh của nhịp hồi tăng từ `Swing_Low_1` (`Swing_High_1 < Đỉnh bắt đầu sóng giảm lớn`)[cite: 1].
    - `Swing_Low_2`: Đáy của nhịp giảm điều chỉnh từ `Swing_High_1` (`Swing_Low_2 > Swing_Low_1`)[cite: 1].

- **KỊCH BẢN 1: QUÉT THANH KHOẢN CẤU TRÚC CƠ BẢN (SWING LOW -> SWING HIGH -> SELL THEO TREND)**:
  - **ĐIỀU KIỆN LỌC (PHA TÍCH LŨY & LẤY ĐÀ)**:
    - **IF** sau khi tạo `Swing_Low_2`, giá tăng yếu (`SUBJECTIVE:` "tăng không nổi", đi ngang zíc zắc dưới `Swing_High_1`)[cite: 1]:
      - **THEN** kỳ vọng giá đạp xuống dưới `Swing_Low_2` (`Low < Swing_Low_2` nhưng `Low > Swing_Low_1`) để "quét thanh khoản phe Buy" (`Fake_Breakout_Low == TRUE`)[cite: 1].
    - **IF** `Fake_Breakout_Low == TRUE` **AND** xuất hiện nến rút chân/đảo chiều tăng đóng cửa lại phía trên `Swing_Low_2`:
      - **CẢNH BÁO LỌC NHIỄU**: `DO_NOT_SELL == TRUE` trong suốt nhịp tăng này (vì giá đang lấy đà tăng mạnh lên quét `Swing_High_1`)[cite: 1].
      - **TÙY CHỌN LỆNH BUY NGẮN HẠN (như hình 00:18)**:
        - `Entry_Long` = Giá đóng cửa của nến quét đáy `Swing_Low_2`[cite: 1].
        - `SL_Long` = Dưới mức `Low` thấp nhất của cụm nến quét `Swing_Low_2`[cite: 1].
        - `TP_Long` = Vùng phía trên `Swing_High_1`[cite: 1].
  - **TRIGGER & ENTRY LỆNH SELL CHÍNH (SAU KHI QUÉT SWING HIGH)**:
    - **IF** nhịp tăng lấy đà đẩy giá vượt lên trên `Swing_High_1` (`High > Swing_High_1` -> `Liquidity_Sweep_High == TRUE`)[cite: 1]:
      - **CẢNH BÁO LỌC NHIỄU**: `DO_NOT_BUY_BREAKOUT == TRUE` (Không canh Buy khi giá hồi về `Swing_High_1` vì đây là quét thanh khoản trong `DOWNTREND`, không phải phá cản đảo chiều)[cite: 1].
      - **TRIGGER SHORT**: Xuất hiện "nến thanh khoản" (nến quét lên trên `Swing_High_1` sau đó xuất hiện nến giảm mạnh đóng cửa trở lại bên dưới `Swing_High_1`)[cite: 1].
      - `Entry_Short_1` = Sau khi đóng cây nến giảm xác nhận dưới `Swing_High_1` (`Order_Type = UNSPECIFIED_IN_VIDEO`)[cite: 1].
      - `SL_Short_1` = Phía trên đỉnh `High` cao nhất của cụm nến vừa quét `Swing_High_1`[cite: 1].
      - `TP_Short_1` = Kéo xuống dưới `Swing_Low_2` và hướng về/vượt qua `Swing_Low_1`[cite: 1].

- **KỊCH BẢN 2: XỬ LÝ SAU KHI GIÁ ĐÃ QUÉT SWING HIGH VÀ ĐẠP XUỐNG (OTE HOẶC ĐẢO CHIỀU)**:
  - **BỐI CẢNH TIẾP DIỄN**: Giả sử `Liquidity_Sweep_High == TRUE` và giá đã có một nhịp sập mạnh từ trên `Swing_High_1` xuống[cite: 1].
  - **NHÁNH 2A – GIÁ ĐẠP THỦNG ĐÁY LỚN LẤY ĐÀ ĐI LÊN (03:43 - 03:48)**:
    - **IF** nhịp giảm đâm thủng luôn qua đáy thấp nhất (`Low < Swing_Low_1`) để lấy đà **AND** sau đó giá vòng tăng ngược trở lại[cite: 1]:
      - **THEN** kích hoạt lệnh **LONG**:
        - `Entry_Long_2` = Khi giá vòng lên lại sau cú đạp thủng đáy (` Exact_Trigger = UNSPECIFIED_IN_VIDEO`)[cite: 1].
        - `SL_Long_2` = Dưới đáy thấp nhất vừa tạo[cite: 1].
        - `TP_Long_2` = Vùng đỉnh `Swing_High` phía trên[cite: 1].
  - **NHÁNH 2B – GIÁ KHÔNG ĐẠP XUỐNG ĐƯỢC MÀ DẬP DÌU ĐI LÊN -> TÌM VÙNG OTE (03:49 - 04:15)**:
    - **IF** sau khi quét `Swing_High_1`, nhịp giảm chững lại (không phá được `Swing_Low_1`, chỉ giảm tới ngang vùng đáy phụ rồi "dập dìu đi lên lại")[cite: 1]:
      - **THEN** kết luận còn vùng thanh khoản cao hơn phía trên `Swing_High_1` cần phải quét[cite: 1].
      - **CÔNG THỨC TÍNH VÙNG OTE**:
        - Xác định đỉnh bắt đầu con sóng giảm lớn (`Major_High` - mức Fibo `1.0`) và đáy thấp nhất của con sóng đó (`Major_Low` / `Swing_Low_1` - mức Fibo `0.0`)[cite: 1].
        - `Range = Major_High - Major_Low`[cite: 1].
        - `OTE_Lower_Bound = Major_Low + 0.618 * Range`[cite: 1].
        - `OTE_Mid_Level = Major_Low + 0.705 * Range`[cite: 1].
        - `OTE_Upper_Bound = Major_Low + 0.790 * Range`[cite: 1].
      - **THIẾT LẬP LỆNH SELL TẠI OTE**:
        - `Entry_Short_OTE` = `OTE_Lower_Bound` (mức Fibo `0.618`, đặt lệnh chờ hoặc đợi giá chạm vùng `OTE`)[cite: 1].
        - `SL_Short_OTE` = Phía trên `OTE_Upper_Bound` (trên mức Fibo `0.790`, cách một khoảng đệm nhỏ nhưng dưới `Major_High`)[cite: 1].
        - `TP_Short_OTE` = `Major_Low` (mức Fibo `0.0` - đáy `Swing_Low_1`)[cite: 1].

---

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Thiếu khung thời gian (Timeframe)**: Video hoàn toàn không nhắc đến việc đang phân tích trên khung thời gian nào (M1, M5, M15 hay H1...), mặc dù tiêu đề series là "Scalping Vàng" nhưng trong lời nói ở `03:14` lại dùng cụm từ "lệnh Sell Swing dài hạn theo xu hướng" [NÓI][cite: 1].
- **Cách định nghĩa và xác định "Nến thanh khoản" chưa có quy tắc định lượng**: Ở đầu video (`00:18` - `00:38`), tác giả khoanh tròn vào một cây nến rút chân/đảo chiều tại vùng quét `Swing High` và `Swing Low` rồi gọi đó là "nến thanh khoản" (và ở `02:48` gọi cụm nến `Fake Breakout` là "nến quét thanh khoản"). Tuy nhiên, trong phần lời giảng, tác giả chỉ tập trung giải thích **hành vi quét thanh khoản** qua đỉnh/đáy chứ không đưa ra tiêu chí cụ thể về hình dáng nến (tỷ lệ râu nến, thân nến, hay phải đợi nến đóng cửa bên trong lại mức cản mới được tính)[cite: 1].
- **Mơ hồ giữa kịch bản Quét Đáy để Tăng luôn và Quét Đáy -> Quét Đỉnh -> Sập**:
  - Ở `02:45` - `03:10`: Giá quét `Swing Low` (tạo `Fake Breakout`) để lấy đà tăng lên quét `Swing High`, rồi từ `Swing High` mới đạp xuống theo xu hướng giảm[cite: 1].
  - Ở `03:43` - `03:48`: Sau khi đã quét `Swing High` và đang đạp xuống, nếu giá đạp thủng luôn đáy lớn để "lấy đà" rồi vòng lên thì tác giả lại bảo canh Buy một lệnh rất đẹp lên tận đỉnh trên[cite: 1].
  - Video không đưa ra điều kiện phân biệt rõ ràng khi nào một cú phá đáy là sự tiếp diễn của `Trend Giảm` chính (như ở `02:08`), và khi nào cú phá đáy đó lại là "đạp luôn lấy đà đi lên lại" để canh Buy ngược xu hướng giảm (như ở `03:44`)[cite: 1].
- **Thiếu điều kiện xác nhận tại vùng `OTE`**: Ở `04:12`, tác giả đặt thẳng khung lệnh Sell tại mép dưới vùng `OTE` (mức Fibo `0.618`) ngay trên biểu đồ dự phóng mà không nói rõ là đặt lệnh `Sell Limit` trực tiếp tại `0.618` hay phải chờ xuất hiện phản ứng giá / nến thanh khoản bên trong vùng `OTE` rồi mới vào lệnh[cite: 1].
- **Câu hỏi cần làm rõ trước khi áp dụng / bot hóa**:
  1. Khung thời gian chuẩn để xác định `Trend Giảm` và các mốc `Swing High` / `Swing Low` là khung nào? Có cần đa khung thời gian không?
  2. Điều kiện chính xác để xác nhận một cú vượt `Swing High` hoặc thủng `Swing Low` là "quét thanh khoản" thay vì "phá vỡ thật (BOS)" là gì (ví dụ: số lượng nến được phép đóng cửa ngoài cản, hay bắt buộc chỉ quét bằng râu nến)?
  3. Tại vùng `OTE`, vào lệnh trực tiếp bằng Limit tại `0.618` hay chờ tín hiệu xác nhận (CHoCH / nến đảo chiều)?

---

## 10. Thông tin khác
- **Kênh / Tác giả & Series**:
  - Tên kênh kêu gọi theo dõi ở cuối video: **TradingMienTrung** [NÓI, HÌNH][cite: 1].
  - Tên Series: **Series 100 Entry Scalping Vàng** [NÓI] / **Series 100 Entry Trade Vàng** [HÌNH] – Tập 11[cite: 1].
  - Tập liên quan được nhắc tới: **Bài số 10** nói về **OTE** [NÓI][cite: 1].
- **Kết quả / Thống kê tác giả khoe**:
  - Tác giả hiển thị 2 ảnh chụp màn hình lệnh giao dịch Vàng trên nền tảng MT4/MT5 điện thoại ở `04:20` - `04:22` với mức lợi nhuận đang chạy là `+9,656.00 USD` (lệnh `BUY 1`, khối lượng 1 lot hoặc tương đương bị che một phần) và `+19,969.00 USD` (lệnh `BUY 2`), kèm lời khẳng định đã từng đăng các lệnh này cho người theo dõi xem nên không phải là backtest hay demo [NÓI, HÌNH][cite: 1]. *(Lưu ý: Thông tin do tác giả tự công bố trên video, chưa được kiểm chứng độc lập).*
- **Kêu gọi hành động (CTA)**: Kêu gọi người xem lưu video, tải về, thả tim, bình luận, chia sẻ và Follow kênh `TradingMienTrung` để đón xem các tập tiếp theo trong series [NÓI, HÌNH][cite: 1].
- **Trích dẫn nguyên văn đáng giữ**:
  - *"Trong trường hợp mà giá nó muốn giảm xuống thì cứ nhớ cho mình nè: đó là nó sẽ cần phải quét lên để lấy thêm lực mua thì nó mới giảm được."* (`01:07` – `01:16`) [NÓI][cite: 1].
  - *"Giá mà nó tăng mà nó tăng không nổi á, nghĩa là nó đang thiếu thanh khoản để mà giảm tiếp."* (`01:28` – `01:33`) [NÓI][cite: 1].
  - *"Trong trường hợp mà thấy quét thanh khoản rồi mà giá nó không xuống được, nghĩa là còn cái vùng thanh khoản ở phía trên cao hơn cần phải quét."* (`03:23` – `03:31`) [NÓI][cite: 1].
- **Ghi chú của người trích xuất**:
  - [SUY LUẬN] Bản chất mô hình trong video là sự kết hợp giữa khái niệm **Inducement (IDM) / Internal Range Liquidity** và **Optimal Trade Entry (OTE)** trong phương pháp ICT/SMC: Các đỉnh `Swing High` và đáy `Swing Low` nằm bên trong một biên độ sóng lớn đóng vai trò là thanh khoản nội khu (Internal Liquidity). Giá thường quét đáy nội khu (dụ phe Sell đuổi hoặc quét SL phe Buy sớm) để lấy lực đẩy lên quét đỉnh nội khu (`Swing High` / Inducement), hoặc đẩy sâu hơn lên vùng `OTE` (`0.618` – `0.79` của sóng lớn) trước khi tiếp diễn xu hướng giảm chính[cite: 1].