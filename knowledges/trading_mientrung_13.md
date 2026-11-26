---
title: "Review lệnh Buy Vàng theo MSNR, Tư duy Điểm Hội Tụ Kỹ Thuật và Giới thiệu Bot SNR System (Tập 13)"
source_author: "KHÔNG RÕ"
video_duration: "03:59"
video_type: ["Review lệnh", "Price Action / Key Level", "Hệ thống/EA/Bot", "Tâm lý giao dịch / Backtest", "Giới thiệu công cụ"]
markets: ["XAUUSD (Vàng / XAUUSDm)"]
timeframes_htf: ["H1"]
timeframes_ltf: ["VIDEO KHÔNG ĐỀ CẬP"]
tools: ["TradingView", "Bot SNR System (MetaTrader)", "Fibonacci Retracement (trên hình minh họa)"]
tags: ["XAUUSD", "MSNR", "SNR", "OTE", "S&R", "Key Level", "Điểm hội tụ kỹ thuật", "Backtest", "Bot SNR System", "Gồng lãi", "Review lệnh"]
extraction_confidence: "Trung bình – Âm thanh và hình ảnh rõ ràng, nhưng video chủ yếu review lệnh, chia sẻ tư duy chờ điểm hội tụ kỹ thuật và giới thiệu Bot SNR System; không hướng dẫn chi tiết quy tắc xác định vùng MSNR, điều kiện kích hoạt hay cách đặt SL/TP cụ thể."
---

# Review lệnh Buy Vàng theo MSNR, Tư duy Điểm Hội Tụ Kỹ Thuật và Giới thiệu Bot SNR System (Tập 13)

## 0. TL;DR
- Video là Tập 13 của series "100 Entry Scalping Vàng", giải quyết lỗi phổ biến khi trade vàng: vào Buy Limit quá sớm ở lưng chừng sóng điều chỉnh nên liên tục dính SL trước khi giá thật sự bật tăng [NÓI].
- Giải pháp tác giả nêu ra là kiên nhẫn chờ giá hồi về vùng Key Level quan trọng nơi phe Buy tập trung mạnh, được gọi là "điểm hội tụ kỹ thuật", áp dụng kỹ thuật MSNR [NÓI].
- Tác giả review lệnh thực tế trên `XAUUSDm` bắt bằng kỹ thuật MSNR (quét trên khung H1 thông qua Bot SNR System), tuyên bố gồng lãi 100 giá và cho thấy kết quả thả nổi khoảng `1,957.55 USD` trên tài khoản số dư `200.00 USD` (lưu ý có độ lệch giữa số liệu nói và ảnh chụp màn hình) [NÓI, HÌNH].
- Để tự làm chủ kỹ năng bắt điểm, cách duy nhất tác giả khuyến nghị là backtest lặp đi lặp lại trên TradingView để ghi nhớ cấu trúc sóng tăng mạnh rồi retest [NÓI].
- Nửa sau video giới thiệu công cụ miễn phí **Bot SNR System** (bán tự động, không phải bot auto) tích hợp 3 phương pháp MSNR, OTE và S&R để hỗ trợ quét entry, nhưng cảnh báo người hoàn toàn chưa có kỹ năng trading sẽ không sử dụng được [NÓI].

## 1. Tổng quan
- **Mục tiêu / vấn đề giải quyết:** Khắc phục tình trạng trader vàng muốn canh Buy theo sóng tăng mạnh nhưng đặt Buy Limit quá sớm, bị quét SL liên tục dẫn đến chán nản ngay trước khi giá tăng vượt đỉnh cũ [NÓI].
- **Đối tượng phù hợp:** Trader giao dịch vàng nói chung; phần giới thiệu Bot SNR System nhắm đến người mới chưa đủ kỹ năng tự đọc điểm hội tụ kỹ thuật, nhưng bắt buộc vẫn phải có kiến thức nền về trading [NÓI].
- **Thị trường, sản phẩm, khung thời gian, phiên giao dịch:**
  - Sản phẩm: Vàng (`XAU/USD`, tài khoản hiển thị mã `XAUUSDm`) [NÓI, HÌNH].
  - Khung thời gian: Tác giả chỉ rõ việc quét entry bằng Bot SNR System trên khung **H1** [NÓI]. Các khung thời gian khác không được nêu rõ.
  - Phiên giao dịch: VIDEO KHÔNG ĐỀ CẬP.
- **Công cụ & thiết lập chỉ báo:**
  - **TradingView:** Dùng để backtest và luyện tập nhận diện điểm vào lệnh [NÓI].
  - **Bot SNR System:** Công cụ quét entry do bên tác giả tự code, tích hợp 3 phương pháp phối hợp là `MSNR`, `OTE`, `S&R` [NÓI, HÌNH].
  - **Chỉ báo xuất hiện trên màn hình (tác giả không giải thích):** Công cụ Fibonacci Retracement trên chart minh họa (00:41–00:47, 02:55–02:57) và một chỉ báo đường trung tâm kèm hai dải biên màu xanh lá (dạng Bollinger Bands/kênh giá) trên chart lệnh thực tế (01:18–01:55) [HÌNH]. Tham số các chỉ báo này: KHÔNG RÕ.

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Luận điểm cốt lõi:** Khi một con sóng tăng mạnh vừa được kích hoạt, giá thường có nhịp hồi (retest) trước khi tiếp diễn xu hướng [NÓI]. Thay vì mua đuổi hoặc rải lệnh sớm ở giữa sóng hồi, trader phải chờ giá quay về những vùng **Key Level quan trọng**, vì đó là nơi "phe Buy họ tập trung mạnh" [NÓI].
- **Tư duy tần suất vs. chất lượng lệnh:** Cơ hội xuất hiện điểm hội tụ kỹ thuật theo MSNR không thường xuyên, nhưng bù lại cho phép gồng lãi xa [NÓI]. Tác giả cho rằng nếu có khả năng gồng lãi thì việc giao dịch theo kiểu này sẽ nhẹ nhàng hơn rất nhiều so với scalping hàng ngày [NÓI].
- **Điều kiện thị trường phù hợp:** Khi vàng vừa khởi đầu một con sóng tăng mạnh và xuất hiện nhịp hồi (retest) về vùng Key Level [NÓI].
- **Điều kiện thị trường KHÔNG phù hợp:** VIDEO KHÔNG ĐỀ CẬP.
- **Giả định ngầm của phương pháp:** Giá sau một cú tăng mạnh sẽ có xu hướng quay lại kiểm tra (retest) vùng hội tụ kỹ thuật trước khi tiếp tục tăng phá đỉnh cũ [SUY LUẬN – rút ra từ mô tả sóng tăng rồi retest ở 00:57–01:11 và 02:29–02:40].

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
|---|---|---|
| Điểm hội tụ kỹ thuật | Điểm vào lệnh Buy đẹp khi vàng vừa khởi đầu một con sóng tăng, nơi có sự hội tụ về kỹ thuật để chờ vào lệnh thay vì vào sớm [NÓI]. | Trên hình minh họa (00:41–00:47, 02:55–02:57), tác giả vẽ một hộp chữ nhật màu cam nằm ở vùng hồi sâu của Fibonacci Retracement trùng với vùng cấu trúc đáy/đỉnh cũ bên trái [HÌNH]. Tác giả không giải thích quy tắc vẽ bằng lời. |
| Key Level | Vùng giá quan trọng nơi phe Buy tập trung mạnh [NÓI]. | Minh họa bằng hộp chữ nhật màu đỏ nằm ngang ở vùng đáy tích lũy phía dưới con sóng tăng mạnh (01:06) [HÌNH]. |
| MSNR | Một kỹ thuật giao dịch được tác giả gọi là "rất là nổi tiếng", dùng để bắt điểm vào lệnh theo vùng Key Level/SNR và có thể gồng lãi xa [NÓI]. | VIDEO KHÔNG ĐỀ CẬP quy tắc vẽ cụ thể bằng lời (chỉ nhắc đến tài liệu "MSNR THEORY" và tích hợp sẵn trong Bot SNR System) [NÓI, HÌNH]. |
| SNR / S&R | Nhắc đến tài liệu "SNR" và một trong 3 phương pháp tích hợp trong Bot SNR System (`S & R`) [NÓI, HÌNH]. | VIDEO KHÔNG ĐỀ CẬP định nghĩa hay cách vẽ chi tiết (trên giao diện bot có dòng chữ `Rải theo SNR / RBS`) [HÌNH]. |
| OTE | Một trong 3 phương pháp tích hợp trong Bot SNR System và xuất hiện trên tiêu đề Tập 10 (`ChoCH + OTE`) [NÓI, HÌNH]. | VIDEO KHÔNG ĐỀ CẬP định nghĩa cụ thể trong tập này. |
| Backtest | Quá trình tập đi tập lại nhiều lần việc bắt điểm trên TradingView bằng cách gợi nhớ các cú tăng mạnh rồi retest và lưu lại vị trí bắt điểm vào trí nhớ [NÓI]. | Quan sát dữ liệu quá khứ trên TradingView và đặt thử vùng/công cụ vị thế (Long/Short Position) (02:22–02:32) [HÌNH]. |
| Bot SNR System | Công cụ bán tự động (không phải bot auto) do tác giả phát triển, tự động quét ra các vùng/entry hội tụ kỹ thuật theo 3 phương pháp MSNR, OTE, S&R [NÓI]. | Bảng điều khiển giao dịch hiển thị trực tiếp trên biểu đồ MetaTrader với 3 cột bật/tắt `MSNR SYSTEM`, `OTE`, `S & R` và nút `RESCAN` [HÌNH]. |

## 4. Hệ thống quy tắc

Video không trình bày quy trình vào lệnh thủ công đầy đủ từng bước. Các quy tắc thực tế trích xuất được chia thành 3 phần: quy trình tư duy chờ setup, quy trình luyện tập Backtest, và thông số công cụ Bot SNR System.

### 4.1 Quy trình tư duy chờ setup Buy theo sóng tăng (Quy tắc định hướng)
- [ ] Xác định vàng đang vừa khởi đầu một con sóng tăng mạnh [NÓI].
- [ ] Không vào Buy Limit sớm khi giá mới bắt đầu điều chỉnh [NÓI].
- [ ] Chờ giá hồi (retest) về đúng vùng Key Level quan trọng / "điểm hội tụ kỹ thuật" nơi phe Buy tập trung mạnh [NÓI].
- [ ] Vào lệnh Buy tại điểm hội tụ kỹ thuật (có thể quét tự động vùng chờ trên khung **H1** nếu dùng Bot SNR System) [NÓI].
- [ ] Gồng lãi theo sóng tăng tiếp diễn nếu có kỹ năng gồng lãi [NÓI].
- **Entry cụ thể, Stop Loss, Take Profit, Điều kiện hủy kèo:** VIDEO KHÔNG ĐỀ CẬP bằng lời.

### 4.2 Quy trình luyện tập Backtest (Kinh nghiệm tác giả)
1. Mở biểu đồ trên TradingView [NÓI].
2. Tìm lại các tình huống lịch sử khi giá xuất hiện một cú tăng mạnh rồi quay lại retest [NÓI].
3. Thực hành xác định vị trí bắt điểm cho từng lần như vậy [NÓI].
4. Lặp đi lặp lại nhiều lần để lưu mẫu hình vào trí nhớ, nhằm loại bỏ tâm lý vội vàng và sợ lỡ entry đẹp khi giao dịch thực tế [NÓI].

### 4.3 Tham số hiển thị của Bot SNR System [HÌNH 01:37–01:45, 03:07–03:21, 03:44–03:48]
Lưu ý: Các thông số dưới đây được ghi nhận hoàn toàn từ giao diện hiển thị trên màn hình ở hai thời điểm quay khác nhau trong video (cảnh 01:38 và cảnh 03:16–03:44), tác giả không giải thích từng ô tham số.
- **Tên giao diện phụ (góc trên bên trái ở 01:43):** `AUTO OTE / LIMIT GRID` [HÌNH].
- **Trạng thái & điều khiển chung:** `BUY READY | SELL READY`, nút `PAUSE`, `DELETE PENDING BUY`, `DELETE PENDING SELL`, `RESCAN`, `APPLY SETTINGS` [HÌNH].
- **Thông số chung (thay đổi giữa 2 cảnh quay):**
  - Khối lượng (Lot): `0.01` (ở 01:38) và `10.00` (ở 03:16) [HÌNH].
  - `RR`: `2.000` (ở 01:38) và `5.000` (ở 03:16) [HÌNH].
  - `Cách giá`: `1.500` (ở 01:38) và `11.000` (ở 03:16) [HÌNH].
- **Module 1 – `MSNR SYSTEM: ON`:**
  - `Pending`: `10 / 10` (01:38) hoặc `9 / 10` (03:16) [HÌNH].
  - `Max pending`: `10` [HÌNH].
  - Mô tả trên giao diện: `Rải theo SNR / RBS`, `Giới hạn tổng BUY + SELL` [HÌNH].
  - Dòng ghi chú nhỏ bên dưới: `Single: SL -> Nửa [KHÔNG RÕ chữ cuối do bị mờ]` [HÌNH].
- **Module 2 – `OTE: ON` và Module 3 – `S & R: ON` (hiển thị cùng bộ tham số ở cảnh 03:16):**
  - `Chế độ`: `Single` [HÌNH].
  - `Khoảng DCA`: `1.000` (01:38) và `3.000` (03:16) [HÌNH].
  - `Kiểu tăng lot`: `Cấp cộng` [HÌNH].
  - `Lot cộng thêm`: `0.000` (01:38) và `0.010` (03:16) [HÌNH].
  - `Hệ số nhân`: `2.000` [HÌNH].
  - `Max lệnh DCA`: `5` [HÌNH].
  - `Trailing`: `200/100/15/20` (01:38) và `300/150/15/20` (03:16) [HÌNH].
- **Thông báo nhật ký (Log) trên màn hình:** `Rescan complete. Valid levels placed; see Journal for skipped !` [HÌNH].

## 5. Case Study / Ví dụ chart

### Ví dụ 1: Phản ví dụ – Vào Buy Limit quá sớm ở lưng chừng sóng hồi
- **Mốc thời gian:** 00:09–00:16, 00:24, 00:57–01:06, 02:49–02:53.
- **Sản phẩm, khung thời gian, hướng lệnh:** Vàng (minh họa), khung thời gian KHÔNG RÕ, hướng BUY [NÓI, HÌNH].
- **Bối cảnh trước setup:** Giá có một nhịp tăng mạnh phá lên cao, sau đó bắt đầu điều chỉnh giảm [NÓI, HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart:**
  - Rải liên tiếp 3 đến 4 lệnh `BUY 0.1` ở vùng lưng chừng khi giá đang hồi xuống (các mức âm hiển thị lần lượt `-93.89 USD`, `-63.89 USD`, `-33.89 USD` ở 00:09; và `-126.88 USD`, `-96.88 USD`, `-66.88 USD`, `-36.88 USD` ở 00:12) [HÌNH].
  - Giá tiếp tục giảm mạnh quét hết SL ở vùng đáy (00:15) [HÌNH].
  - Đến 01:06, tác giả vẽ một hộp chữ nhật màu đỏ nằm ngang tại vùng đáy tích lũy phía dưới (Key Level), cho thấy giá chỉ thực sự bật tăng và phá đỉnh sau khi chạm về vùng này [HÌNH, NÓI].
- **Entry / SL / TP cụ thể:** Không hiển thị mức giá cụ thể trên trục giá [HÌNH].
- **Kết quả & bài học:** Bị quét SL liên tục trước khi giá chạy đúng hướng; minh họa hậu quả của việc không chờ giá về Key Level quan trọng [NÓI].
- **Liên kết quy tắc:** Phản ví dụ cho mục 4.1.

### Ví dụ 2: Minh họa trực quan "Điểm hội tụ kỹ thuật" với Fibonacci & vùng hộp màu cam
- **Mốc thời gian:** 00:41–00:47 và lặp lại ở 02:55–02:57.
- **Sản phẩm, khung thời gian, hướng lệnh:** Vàng (minh họa, vùng giá quanh `3,919`–`3,965`), khung thời gian KHÔNG RÕ, hướng BUY [HÌNH].
- **Bối cảnh trước setup:** Giá tăng mạnh tạo một con sóng đẩy từ vùng đáy `3,919.90` lên đỉnh `3,964.83`, sau đó hồi xuống [HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart (chỉ hiện trên hình, không thuyết minh chi tiết):**
  - Kéo Fibonacci Retracement từ đáy `1 (3,919.90)` lên đỉnh `0 (3,964.83)`, thấy các mốc `0.5 (3,942.40)` và các mốc hồi sâu bên dưới (`0.618`, `0.886` – phần số giá chi tiết bị mờ) [HÌNH].
  - Vẽ hộp chữ nhật màu cam tại vùng hồi sâu phía dưới mức `0.5`, trùng với vùng cấu trúc đỉnh/đáy cũ bên trái [HÌNH].
  - Đặt công cụ Long Position với điểm vào nằm trong hộp màu cam và SL nằm dưới đáy hộp/đáy con sóng [HÌNH].
- **Entry / SL / TP cụ thể trên công cụ TradingView [HÌNH]:**
  - Ở 00:44: Target `16.61 (0.399%)` / `1,661`, Stop `8.77 (0.240%)` / `877` (R:R khoảng `1.89`).
  - Ở 00:45–00:47: Kéo Target lên cao hơn thành `37.51 (0.955%)` / `3,751`, Stop `9.68 (0.246%)` / `968` (R:R khoảng `3.88`).
- **Kết quả & bài học:** Giá hồi về hộp màu cam, đi ngang tích lũy rồi bật tăng mạnh vượt đỉnh cũ, đạt TP [HÌNH]. Minh họa hình ảnh cho khái niệm "điểm hội tụ kỹ thuật" ở mục 4.1 [NÓI, HÌNH].
- **Liên kết quy tắc:** Ví dụ thuận cho mục 4.1.

### Ví dụ 3: Review lệnh thực chiến XAUUSDm theo MSNR (quét bằng Bot SNR System khung H1)
- **Mốc thời gian:** 00:00, 01:12–01:25, 01:40–01:45, 01:52–02:05.
- **Sản phẩm, khung thời gian, hướng lệnh:** `XAUUSDm`, quét entry trên khung **H1** [NÓI, HÌNH], hướng BUY.
- **Bối cảnh trước setup:** Trên biểu đồ (01:18, 01:52, 01:55), giá vàng đang trong nhịp giảm sâu rồi rút chân mạnh tại vùng `3890`–`3898` trước khi bật tăng thẳng lên vùng `3961`–`3964` [HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart và thông số lệnh:**
  - **Trên biểu đồ MT5 (01:18–01:19, 01:41, 01:52, 01:55) [HÌNH]:**
    - 1 lệnh đang khớp: `BUY 0.1` tại mức giá `3898.628` (lợi nhuận thả nổi hiển thị từ `+638.48 USD` đến `+669.42 USD`).
    - 1 lệnh chờ chưa khớp bên dưới: `BUY LIMIT 0.1` tại `3890.575`.
    - Không thấy hiển thị đường SL hay TP trên khung hình biểu đồ.
  - **Trên ảnh chụp màn hình ứng dụng giao dịch (00:00, 01:23–01:25, 01:42, 02:01, 02:04) [HÌNH]:**
    - Tài khoản có Số dư: `200.00 USD`, Tiền ký quỹ: `58.47 USD`.
    - Gồm 3 lệnh `XAUUSDm buy 0.1`:
      - Lệnh 1: mở tại `3898.308`
      - Lệnh 2: mở tại `3898.232`
      - Lệnh 3: mở tại `3898.232`
    - Giá hiện tại trên ảnh chụp di chuyển từ `3960.624` đến `3963.509`.
    - Tổng lợi nhuận thả nổi cao nhất hiển thị: `1 957.55 USD` (Vốn: `2 157.55 USD`, Ký quỹ dư: `2 099.08 USD`, Mức ký quỹ: `3 690.01%`), mỗi lệnh lãi `652.01 USD` và `652.77 USD` (x2).
- **Kết quả & bài học:** Tác giả tuyên bố bắt được điểm Buy và gồng lãi được `+100 giá` [NÓI, HÌNH 01:22], khẳng định việc gồng lãi từ điểm hội tụ kỹ thuật giúp giao dịch nhẹ nhàng hơn scalping hàng ngày [NÓI]. (Xem mục 9 về sai lệch giữa tuyên bố `+100 giá` và mức `+65.2 giá` trên ảnh chụp màn hình).
- **Liên kết quy tắc:** Ví dụ thuận cho mục 4.1 và ứng dụng Bot SNR System ở mục 4.3.

## 6. Tips, Tricks & Cảnh báo
- **Tránh tâm lý sợ lỡ kèo (FOMO):** Nguyên nhân vào lệnh quá sớm thường là do vội vàng và sợ mất entry đẹp; cần luyện backtest nhiều để tự tin chờ giá về đúng điểm hội tụ kỹ thuật [NÓI].
- **Tư duy gồng lãi vs. tần suất lệnh:** Kỹ thuật MSNR không cho tín hiệu liên tục hàng ngày, nên hãy tận dụng lợi thế gồng lãi thay vì ép bản thân scalping liên tục [NÓI].
- **Cách rèn kỹ năng đọc chart:** Tác giả nhấn mạnh "chỉ có một cách duy nhất" để tự bắt được các điểm như vậy là tập backtest lặp đi lặp lại trên TradingView và lưu lại các tình huống tăng mạnh rồi retest vào trí nhớ [NÓI].
- **Cảnh báo khi dùng Bot SNR System:** Con bot này **không phải bot auto** (tự động chạy không cần người) [NÓI]. Nếu trader hoàn toàn không có kỹ năng về trading thì sẽ **không thể nào sử dụng được** con bot này [NÓI].
- **Khuyến nghị kiểm chứng:** Nên trải nghiệm Bot SNR System trên tài khoản **demo** trước để tự đánh giá tính hiệu quả [NÓI].

## 7. Quản trị rủi ro & Tâm lý
- **Risk % mỗi lệnh, cách tính lot, giới hạn lỗ ngày/tuần, số lệnh tối đa:** VIDEO KHÔNG ĐỀ CẬP quy tắc quản trị vốn.
- **Dữ liệu thực tế quan sát được (không phải quy tắc tác giả dạy):** Trong ảnh chụp màn hình review lệnh, tài khoản có số dư `200.00 USD` nhưng vào tổng cộng `0.3 lot` vàng (`3 lệnh buy 0.1`), tiền ký quỹ `58.47 USD` [HÌNH].
- **Tâm lý giao dịch:** Nhấn mạnh việc khắc phục tâm lý nản chí sau chuỗi SL liên tiếp và loại bỏ sự vội vàng/sợ mất cơ hội thông qua luyện tập backtest để rèn kỷ luật chờ đợi [NÓI].

## 8. Đặc tả logic cho LLM / Bot
Video không cung cấp đủ quy tắc để mã hóa thành thuật toán.

Các thông tin cốt lõi còn thiếu trong video:
- Không có định nghĩa toán học hoặc quy tắc hành động giá để xác định "sóng tăng mạnh" (ví dụ: số nến, biên độ giá, phá cấu trúc/BOS/ChoCH).
- Không có quy tắc xác định chính xác vùng `Key Level`, vùng `MSNR`, `SNR / RBS`, `OTE`, hay "điểm hội tụ kỹ thuật" (các yếu tố nào hội tụ với nhau).
- Không có điều kiện lọc (filter) và tín hiệu kích hoạt (trigger) để biết khi nào đặt lệnh Limit hay chờ nến xác nhận (Market).
- Không có quy tắc đặt `Stop Loss` (khoảng cách point/pip, đặt dưới râu nến hay đáy cấu trúc) và `Take Profit` (mục tiêu R:R cố định, vùng cản hay cơ chế gồng lãi/trailing cụ thể).
- Không có quy tắc xác định khối lượng lệnh, cách chia nhiều lệnh (như 3 lệnh `0.1` trong ảnh chụp), hay điều kiện hủy lệnh chờ khi cấu trúc bị phá vỡ.

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Mâu thuẫn về mức gồng lãi (`+100 giá` vs. `~65.2 giá`):** Tác giả nói và chèn chữ "+100 GIÁ" [NÓI, HÌNH 01:22], nhưng tất cả ảnh chụp màn hình tài khoản hiển thị lệnh đang chạy chỉ cho thấy giá đi từ `3898.232`/`3898.308` lên cao nhất `3963.509` (tương đương khoảng `65.2` giá) [HÌNH 00:00, 01:24, 02:04]. Video không chiếu bằng chứng đóng lệnh ở mức +100 giá.
- **Không đồng nhất giữa chart MT5 và ảnh chụp app điện thoại:** Trên chart MT5 (01:18, 01:41, 01:52) chỉ hiển thị 1 lệnh `BUY 0.1` tại `3898.628` (kèm 1 lệnh `BUY LIMIT 0.1` tại `3890.575`), trong khi ảnh chụp app điện thoại hiển thị 3 lệnh `buy 0.1` tại `3898.308` và `3898.232` [HÌNH].
- **Sự khác biệt về tên series và định hướng:** Lời nói gọi là series "100 Entry Scalping Vàng" / "100 Entry Scalping Gold" nhưng nội dung tập 13 lại khuyên gồng lãi dài để nhẹ nhàng hơn so với scalping hàng ngày; ngoài ra ảnh bìa Tập 10 ở 00:51 ghi là "Series 100 Entry Trade Vàng" [NÓI, HÌNH].
- **Thông tin bị mờ trên màn hình:** Các mức giá chi tiết ở các mốc Fibonacci trung gian (`0.618`, `0.886`) ở 00:41 và 02:56, cũng như dòng ghi chú nhỏ cuối bảng Bot SNR System (`Single: SL -> Nửa ...` và dòng chữ xám cuối cùng dưới log) bị mờ không đọc được đầy đủ [HÌNH].
- **Khung thời gian của chart thực tế không rõ:** Tác giả nói quét entry bằng bot ở khung H1 [NÓI], nhưng đồng hồ đếm ngược nến trên chart lệnh thực tế (01:18, 01:41, 01:52) hiển thị `02:28:46` và `02:38:02` (hơn 2 tiếng, gợi ý đang xem ở khung H4) [HÌNH, SUY LUẬN].
- **Quy tắc tác giả ngầm hiểu nhưng không giải thích:** Tác giả giả định người xem đã xem các tập trước (như Tập 10 `ChoCH + OTE`) hoặc đọc tài liệu `MSNR THEORY` nên không giải thích cách vẽ MSNR, OTE hay S&R trong video này [NÓI, HÌNH].
- **Câu hỏi cần làm rõ trước khi áp dụng/bot hóa:**
  1. Tiêu chí định lượng để xác định vùng MSNR, S&R và OTE trong Bot SNR System là gì?
  2. Điểm hội tụ kỹ thuật yêu cầu kết hợp cụ thể những yếu tố nào (ví dụ: Key Level + Fibonacci OTE)?
  3. Quy tắc đặt Stop Loss, phân bổ khối lượng (tại sao vào 3 lệnh 0.1 trên tài khoản 200 USD) và chiến lược gồng lãi/trailing cụ thể ra sao?

## 10. Thông tin khác
- **Tài liệu & Series được nhắc tới:**
  - Series "100 Entry Scalping Vàng" / "100 Entry Trade Vàng" (nhắc đến Tập 10 `ChoCH + OTE` và video hiện tại là Tập 13) [NÓI, HÌNH].
  - Tài liệu `MSNR THEORY` (hình 00:54 hiển thị 4 phần `01`, `02`, `03`, `04`) [NÓI, HÌNH].
- **Kết quả/thống kê tác giả chia sẻ (CHƯA ĐƯỢC KIỂM CHỨNG ĐỘC LẬP):**
  - Tuyên bố gồng lãi `+100 giá` trên lệnh Buy vàng tuần vừa rồi [NÓI, HÌNH].
  - Ảnh chụp màn hình tài khoản `XAUUSDm` số dư `200.00 USD`, lãi thả nổi `1,957.55 USD` (gần x10 số dư) với 3 lệnh `buy 0.1` [HÌNH].
  - Tuyên bố Bot SNR System nhận được rất nhiều feedback tốt từ cộng đồng trong tháng vừa qua [NÓI].
- **Giới thiệu sản phẩm / Quảng cáo (tách riêng khỏi kiến thức):**
  - Tác giả quảng bá **Bot SNR System** do đội ngũ của mình nghiên cứu và phát triển, tuyên bố cung cấp **hoàn toàn miễn phí**, không thu phí và cho phép chạy thử trên tài khoản demo; kêu gọi người xem trải nghiệm và gửi feedback [NÓI].
- **Trích dẫn nguyên văn đáng giữ:**
  - "Ở trong tập này mình sẽ hướng dẫn anh em cái cách để mà tìm một cái điểm buy đẹp khi mà vàng nó vừa khởi đầu của một con sóng tăng. Mình gọi đó là điểm hội tụ kỹ thuật." [NÓI]
  - "Khi mà một cái con sóng tăng nó kích hoạt thì để mà có một cái entry đẹp chúng ta phải chờ cho nó về những cái vùng key level quan trọng, về những cái vùng mà ở đó phe buy họ tập trung mạnh." [NÓI]
  - "Và nó không phải là một con bot auto và nếu như anh em hoàn toàn không có kỹ năng về trading thì anh em cũng không thể nào mà sử dụng được con bot này." [NÓI]
- **Ghi chú của người trích xuất:**
  - [SUY LUẬN] Dù tác giả không giải thích chi tiết trên lời nói, hình ảnh minh họa ở 00:41–00:47 và 02:55–02:57 cho thấy cách tiếp cận "điểm hội tụ kỹ thuật" của tác giả có sử dụng sự hợp lưu giữa vùng hồi sâu của Fibonacci Retracement (khu vực dưới `0.5`, quanh `0.618`–`0.886`) với vùng cấu trúc giá/hỗ trợ cũ bên trái.
  - [SUY LUẬN] Giao diện Bot SNR System có chứa các tham số liên quan đến DCA (`Khoảng DCA`, `Kiểu tăng lot`, `Hệ số nhân`, `Max lệnh DCA`) và `Rải theo SNR / RBS` với `Max pending: 10`, cho thấy bên cạnh chế độ `Single`, công cụ này còn có cơ chế rải lệnh chờ hoặc DCA tùy cấu hình người dùng.