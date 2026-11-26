---
title: "Phương pháp giao dịch phiên London kết hợp bộ EMA (5, 9, 13, 21, 200) và FVG của Tyler (TG Capital)"
source_author: "Safe Trade (S TRADE - SAFE TRADING) / Tác giả phương pháp gốc: Tyler (TG Capital)"
video_duration: "11:52 (712.5 giây)"
video_type: ["SMC / ICT", "Indicator-based", "Price Action / Key Level / Mô hình nến", "Backtest / Review hệ thống"]
markets: ["EURUSD", "XAUUSD", "Forex", "Chung"]
timeframes_htf: ["M30"]
timeframes_ltf: ["VIDEO KHÔNG ĐỀ CẬP"]
tools: ["EMA 5", "EMA 9", "EMA 13", "EMA 21", "EMA 200", "Fair Value Gap (FVG)"]
tags: ["Tyler", "TG Capital", "London Session", "FVG", "Fair Value Gap", "EMA Stacking", "EMA 200", "Rejection Candle", "Swing Trading", "M30"]
extraction_confidence: "Cao – Video trình bày rõ ràng từng bước quy tắc, thông số chỉ báo, khung giờ và có 2 ví dụ biểu đồ thực tế kèm hình ảnh trực quan"
---

# Phương pháp giao dịch phiên London kết hợp bộ EMA (5, 9, 13, 21, 200) và FVG của Tyler (TG Capital)

## 0. TL;DR
- Phương pháp của Tyler (TG Capital) kết hợp bộ 5 đường trung bình động `EMA 5, 9, 13, 21, 200` với vùng mất cân bằng giá `FVG` và hành động giá (nến từ chối + nến xác nhận) trên khung thời gian `M30` [NÓI, HÌNH].
- Chỉ tìm kiếm cơ hội trong khung giờ thanh khoản phiên London từ `03:00 - 06:30` theo giờ New York, tương đương `15:00 - 18:30` giờ Việt Nam vào mùa đông hoặc `14:00 - 17:30` giờ Việt Nam vào mùa hè [NÓI, HÌNH].
- Chỉ giao dịch thuận xu hướng khi toàn bộ 5 đường EMA xếp chồng đúng thứ tự (`EMA 5 > 9 > 13 > 21 > 200` cho lệnh Mua; ngược lại cho lệnh Bán), đồng hướng và không đan chéo nhau [NÓI, HÌNH].
- Điểm vào lệnh yêu cầu 3 bước tại vùng FVG: giá hồi về FVG -> xuất hiện cây nến từ chối giá có râu dài -> cây nến tiếp theo đóng cửa nhưng KHÔNG được vượt qua đỉnh (với lệnh Mua) của cây nến từ chối giá [NÓI, HÌNH].
- Không đặt Take Profit cố định mà gồng lệnh theo cấu trúc EMA xếp chồng; chỉ thoát lệnh khi các đường EMA thu hẹp khoảng cách, co cụm và đan xen vào nhau [NÓI, HÌNH].
- Tần suất xuất hiện rất thấp (khoảng `10 setup/năm` cho mỗi cặp tiền theo lời Tyler), hướng tới các lệnh giữ dài (Hold/Swing) có tỷ lệ R:R lớn thay vì giao dịch liên tục mỗi ngày [NÓI].

## 1. Tổng quan
- **Mục tiêu / Vấn đề video giải quyết**: Bóc tách chi tiết bộ quy tắc giao dịch của Tyler (TG Capital) – người tuyên bố có tỷ lệ thắng khoảng `90%` và tỷ lệ lợi nhuận từ `20R` trở lên – đồng thời kiểm chứng thực tế (backtest) trên biểu đồ các thị trường khác nhau để đánh giá khách quan điểm mạnh, điểm yếu và rủi ro tiềm ẩn [NÓI, HÌNH].
- **Đối tượng phù hợp**:
  - Phù hợp với những trader hướng tới các lệnh Swing/Hold có tỷ lệ lợi nhuận lớn, kiên nhẫn và không muốn nhìn biểu đồ quá nhiều [NÓI].
  - Không phù hợp với người thích giao dịch liên tục (Scalp/Overtrade) hoặc cần cảm giác vào lệnh mỗi ngày để thấy mình đang làm việc [NÓI].
- **Thị trường và sản phẩm áp dụng**: Các cặp tiền Forex và Vàng (trong video minh họa trực tiếp trên `EURUSD` và `XAUUSD`) [NÓI, HÌNH].
- **Khung thời gian**: Khung `30 phút (M30)` [NÓI, HÌNH]. Video không sử dụng đa khung thời gian.
- **Phiên giao dịch áp dụng**:
  - Chỉ giao dịch trong **Vùng thanh khoản London (Phiên London)**: từ `03:00 đến 06:30 sáng` theo giờ New York [NÓI, HÌNH].
  - Quy đổi giờ Việt Nam: `15:00 đến 18:30` vào mùa đông [NÓI, HÌNH] và `14:00 đến 17:30` vào mùa hè [HÌNH].
  - Khung giờ vàng trong phiên: Các mô hình nến xuất hiện vào lúc `02:30`, `03:00` và `03:30` sáng theo giờ New York (trên màn hình ghi chú tương ứng `14h30, 15h, 15h30` giờ Việt Nam) thường là những cây nến cực mạnh và cực sạch [NÓI, HÌNH].
- **Công cụ & thiết lập chỉ báo**:
  - Bộ 5 đường trung bình động hàm mũ (EMA) với các chu kỳ: `5`, `9`, `13`, `21`, và `200` [NÓI, HÌNH]. (Lưu ý: Trong lời nói tác giả đôi lúc gọi tắt là `MA`, nhưng chữ hiển thị trên màn hình và phần thuyết minh sau xác nhận là `EMA`).
  - Công cụ vẽ vùng `Fair Value Gap (FVG)` [NÓI, HÌNH].

## 2. Lý thuyết & Cơ chế (Tại sao nó hoạt động)
- **Tư duy "Chất lượng hơn số lượng"**:
  - Tyler cho biết mỗi cặp tiền chỉ có khoảng `10 setup` chất lượng trong cả năm [NÓI].
  - `10 lệnh Hold` với lợi nhuận `20R/lệnh` trong một năm có thể tạo ra kết quả vượt trội mà `200 lệnh Scalp` (với mức `1R/lệnh`) không làm được [NÓI, HÌNH].
- **Tại sao thời gian quan trọng hơn hành động giá (Ưu tiên phiên London)**:
  - Phiên London (`03:00 - 06:30` NY) là thời điểm dòng tiền thực sự bắt đầu đổ vào thị trường khi các ngân hàng lớn và tổ chức tài chính tại Châu Âu tham gia [NÓI].
  - Thanh khoản tăng mạnh giúp biến động giá trở nên rõ ràng hơn, sớm bộc lộ phe đang nắm quyền kiểm soát (phe mua hoặc phe bán) [NÓI].
  - Qua hơn `6 năm` backtest và thống kê dữ liệu thực tế, Tyler nhận thấy những vùng `FVG` xuất hiện trong giai đoạn này có xác suất dẫn đến nhịp tiếp diễn xu hướng cao hơn đáng kể so với các thời điểm khác trong ngày [NÓI].
- **Cơ chế của bộ EMA xếp chồng (EMA Stacking)**:
  - Xác nhận xu hướng hiện tại thực sự được dẫn dắt bởi dòng tiền lớn chứ không phải biến động ngẫu nhiên [NÓI].
  - Khi cả 5 đường EMA (`5, 9, 13, 21, 200`) xếp chồng đúng thứ tự, đồng hướng và tách rời nhau, động lực thị trường đang rất mạnh và hoàn toàn nằm dưới sự kiểm soát của một phe [NÓI].
  - Khi các đường EMA đan chéo hoặc đổi vị trí liên tục, lực mua và lực bán đang cân bằng, thị trường thiếu định hướng rõ ràng nên xác suất bị quét thanh khoản hoặc đảo chiều bất ngờ sẽ rất cao [NÓI].
- **Cơ chế hồi về FVG và Nến từ chối giá**:
  - Sau một cú tăng/giảm mạnh tạo ra `FVG` (khoảng trống giá do dòng tiền lớn đẩy giá đi quá nhanh), thị trường thường có xu hướng quay lại lấp một phần khoảng trống trước khi tiếp tục xu hướng chính [NÓI].
  - Cây nến râu dưới dài tại FVG (trong xu hướng tăng) chứng tỏ phe bán đã cố gắng tấn công đẩy giá xuống thấp hơn nhưng thất bại vì phe mua lập tức tham gia kéo giá ngược lên, giành lại quyền kiểm soát [NÓI].
- **Cơ chế của Nến xác nhận không vượt đỉnh nến từ chối**:
  - Theo thống kê backtest nhiều năm của Tyler trong xu hướng tăng, những setup mà cây nến ngay sau nến từ chối giá đóng cửa vượt lên trên đỉnh của nến từ chối thường dẫn đến việc thị trường sớm quay đầu đảo chiều [NÓI].
  - Do đó, chỉ chọn trường hợp nến tiếp theo đóng cửa KHÔNG vượt đỉnh nến từ chối để lọc ra các cơ hội có xác suất thắng dài hạn cao nhất [NÓI].

## 3. Thuật ngữ & Định nghĩa

| Thuật ngữ | Định nghĩa theo cách tác giả dùng | Cách nhận diện trên chart |
| :--- | :--- | :--- |
| **Vùng thanh khoản London** | Khung giờ dòng tiền từ các ngân hàng và tổ chức tài chính Châu Âu đổ vào thị trường [NÓI]. | Khung thời gian từ `03:00 - 06:30` giờ New York (`15:00 - 18:30` giờ VN mùa đông; `14:00 - 17:30` giờ VN mùa hè) trên biểu đồ `M30` [NÓI, HÌNH]. |
| **Bộ EMA xếp chồng (EMA Stacking)** | Trạng thái 5 đường EMA (`5, 9, 13, 21, 200`) sắp xếp theo đúng thứ tự từ nhỏ đến lớn (hoặc ngược lại), phản ánh động lực xu hướng mạnh [NÓI, HÌNH]. | Xu hướng tăng: `EMA 5 > EMA 9 > EMA 13 > EMA 21 > EMA 200`. Xu hướng giảm: `EMA 5 < EMA 9 < EMA 13 < EMA 21 < EMA 200`. Các đường cùng dốc theo một hướng và không cắt nhau [NÓI, HÌNH]. |
| **Fair Value Gap (FVG)** | Khoảng trống giá hình thành khi thị trường di chuyển quá nhanh và mạnh khiến một phần giá bị bỏ qua, gần như không có giao dịch khớp ở giữa [NÓI]. | Cụm 3 nến cùng chiều đẩy mạnh; vẽ từ điểm cao nhất (High) của cây nến thứ nhất đến điểm thấp nhất (Low) của cây nến thứ ba (đối với FVG tăng) [NÓI]. |
| **Nến từ chối giá (Rejection Candle)** | Cây nến phản ứng tại vùng FVG cho thấy phe ngược xu hướng tấn công thất bại và phe thuận xu hướng chiếm lại quyền kiểm soát [NÓI]. | Với lệnh Mua: Cây nến chạm vào (hoặc râu xuyên thủng qua) vùng FVG và rút chân tạo phần râu dưới rất dài; lý tưởng nhất là thân nến nhỏ hoặc đóng cửa phía trên/trong vùng FVG [NÓI, HÌNH]. |
| **Nến xác nhận (Confirmation Candle)** | Cây nến xuất hiện ngay sau cây nến từ chối giá, dùng làm tín hiệu lọc cuối cùng và là điểm vào lệnh [NÓI, HÌNH]. | Với lệnh Mua: Cây nến ngay sau nến từ chối giá có mức giá đóng cửa (Close) KHÔNG vượt lên trên mức giá cao nhất (High) của cây nến từ chối giá [NÓI, HÌNH]. |

## 4. Hệ thống quy tắc

### 4.1 Điều kiện tiên quyết / Confluence (Checklist)
- [ ] Biểu đồ đang ở khung thời gian `30 phút (M30)` [NÓI, HÌNH].
- [ ] Thời gian hiện tại nằm trong phiên thanh khoản London: `03:00 - 06:30` giờ New York (`15:00 - 18:30` giờ VN mùa đông / `14:00 - 17:30` giờ VN mùa hè) [NÓI, HÌNH].
- [ ] Đã bật đủ 5 đường trung bình động: `EMA 5`, `EMA 9`, `EMA 13`, `EMA 21` và `EMA 200` [NÓI, HÌNH].
- [ ] Các đường EMA xếp chồng đúng thứ tự, đồng hướng và tách biệt, không đan chéo nhau [NÓI, HÌNH].
- [ ] Xuất hiện vùng `FVG` hợp lệ được tạo bởi nhịp đẩy mạnh trong phiên [NÓI, HÌNH].

### 4.2 Xác định bối cảnh & hướng (Bias)
- **Trục chính `EMA 200`**:
  - Giá nằm bên trên `EMA 200`: Chỉ tìm lệnh **Mua (Long)** [NÓI, HÌNH].
  - Giá nằm bên dưới `EMA 200`: Chỉ tìm lệnh **Bán (Short)** [NÓI, HÌNH].
- **Xác nhận bằng trật tự bộ EMA**:
  - **Bias Mua (Bullish)**: `EMA 5` nằm trên `EMA 9`, `EMA 9` nằm trên `EMA 13`, `EMA 13` nằm trên `EMA 21`, và `EMA 21` nằm trên `EMA 200` (`EMA 5 > EMA 9 > EMA 13 > EMA 21 > EMA 200`), tất cả cùng hướng lên [NÓI, HÌNH].
  - **Bias Bán (Bearish)**: Thứ tự đảo ngược hoàn toàn (`EMA 5 < EMA 9 < EMA 13 < EMA 21 < EMA 200`), tất cả cùng hướng xuống [NÓI, HÌNH].

### 4.3 Tín hiệu kích hoạt (Trigger)
Quy trình kích hoạt gồm 3 bước tuần tự (chi tiết cho lệnh Mua; lệnh Bán suy luận đối xứng ngược lại [SUY LUẬN - do tác giả nêu quy tắc đối xứng nhưng cả 2 ví dụ trên hình đều là lệnh Mua]):
1. **Hình thành FVG**: Chờ một nhịp tăng mạnh tạo ra vùng `FVG` (vẽ từ đỉnh cây nến thứ 1 đến đáy cây nến thứ 3) [NÓI, HÌNH].
2. **Giá hồi về FVG và tạo Nến từ chối giá**:
   - Kiên nhẫn chờ giá quay lại kiểm định (lấp một phần) vùng `FVG` [NÓI].
   - Xuất hiện một cây nến từ chối giá rõ ràng tại vùng FVG với phần **râu dưới dài** [NÓI, HÌNH].
   - Râu nến của cây nến từ chối được phép xuyên thủng qua cạnh dưới của vùng FVG [NÓI].
3. **Nến xác nhận hợp lệ**:
   - Quan sát cây nến tiếp theo ngay sau cây nến từ chối giá [NÓI, HÌNH].
   - Cây nến tiếp theo này **KHÔNG được đóng cửa vượt lên trên đỉnh (High) của cây nến từ chối giá** vừa xuất hiện [NÓI, HÌNH].

### 4.4 Entry (Điểm vào lệnh)
- **Loại lệnh**: Vào lệnh trực tiếp (Market Execution) ngay khi cây nến xác nhận (cây nến thứ hai sau khi chạm FVG) đóng cửa thỏa mãn điều kiện ở mục 4.3 [NÓI, HÌNH].
- **Vị trí chính xác**: Mức giá đóng cửa (Close) của cây nến xác nhận [HÌNH].

### 4.5 Stop Loss (SL)
- **Quy tắc đặt**: Đặt ngay phía dưới đáy (Low) của cây nến từ chối giá (đối với lệnh Mua) [NÓI, HÌNH].
- **Khoảng cách đệm (Buffer)**: Video không đề cập số pip cộng thêm cụ thể; trên biểu đồ đặt sát ngay dưới râu dưới của cây nến từ chối giá [HÌNH].

### 4.6 Take Profit / Quản lý lệnh
- **Mục tiêu chốt lời (TP)**: Không sử dụng mức chốt lời cố định [NÓI].
- **Quy tắc giữ lệnh (Hold)**:
  - Tiếp tục nắm giữ lệnh miễn là hệ thống các đường EMA (`5, 9, 13, 21, 200`) vẫn duy trì trạng thái xếp chồng đúng thứ tự và chưa xuất hiện dấu hiệu suy yếu [NÓI].
  - Nếu giá có nhịp điều chỉnh giảm sâu ngược lại vào vùng FVG nhưng **chưa chạm Stop Loss** và **cấu trúc xếp chồng của bộ EMA vẫn giữ nguyên**, tuyệt đối không đóng lệnh sớm mà tiếp tục gồng lệnh [NÓI, HÌNH].
- **Quy tắc thoát lệnh chủ động (Exit)**:
  - **Dấu hiệu từ chỉ báo EMA**: Đóng lệnh khi các đường EMA ngắn hạn (`5, 9, 13, 21`) bắt đầu thu hẹp khoảng cách, co cụm và đan xen (cắt) vào nhau [NÓI, HÌNH].
  - **Dấu hiệu từ cấu trúc giá (kết hợp)**: Khi các đường EMA bắt đầu đan xen đồng thời giá đi ngang tạo ra một vùng mua/hỗ trợ bị kiểm tra lặp đi lặp lại nhiều lần (ví dụ: 4 đáy liên tiếp đi qua cùng một vùng giá), chủ động thoát lệnh vì vùng giá bị kiểm tra càng nhiều lần thì xác suất bị phá vỡ càng cao [NÓI, HÌNH].

### 4.7 Điều kiện KHÔNG vào lệnh / Hủy kèo
- Thời gian nằm ngoài khung giờ phiên London (`03:00 - 06:30` giờ New York) [NÓI, HÌNH].
- Các đường EMA đan chéo nhau, đi ngang hoặc liên tục đổi vị trí dù nhìn bằng mắt thường giá có vẻ đang trong xu hướng tăng/giảm [NÓI, HÌNH].
- Giá hồi về FVG nhưng không tạo được cây nến từ chối giá có râu dài rõ ràng [NÓI].
- Cây nến ngay sau cây nến từ chối giá đóng cửa **vượt lên trên đỉnh** của cây nến từ chối giá (bỏ qua setup này vì xác suất thị trường sớm quay đầu cao) [NÓI, HÌNH].

## 5. Case Study / Ví dụ chart

### 5.1 Ví dụ 1: Giao dịch Mua (Long) cặp EURUSD trên khung M30
- **Mốc thời gian trong video**: `02:48 - 07:58` [NÓI, HÌNH].
- **Sản phẩm, khung thời gian, hướng lệnh**:
  - Sản phẩm: `EURUSD` [NÓI, HÌNH].
  - Khung thời gian: `30 phút (M30)` [NÓI, HÌNH].
  - Hướng lệnh: **Mua (Long)** [NÓI, HÌNH].
  - Thời điểm trên biểu đồ: Con trỏ chuột trên màn hình chỉ vào cây nến lúc `Tue 07 Apr '20 15:00` (tức ngày 07/04/2020 lúc 15:00) [HÌNH], tuy nhiên trong lời nói tác giả đọc nhầm thành "15 giờ ngày mùng 7 tháng 4 năm 2026" [NÓI].
- **Bối cảnh trước setup**:
  - Trước 15:00, các đường EMA còn bó hẹp và giao cắt nhau [HÌNH].
  - Khi bước vào phiên London lúc `15:00`, xuất hiện các cây nến tăng mạnh đẩy giá vọt lên trên `EMA 200` và kéo toàn bộ các đường `EMA 5, 9, 13, 21, 200` xếp chồng đúng thứ tự `EMA 5 > 9 > 13 > 21 > 200`, dốc lên rõ rệt [NÓI, HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Đánh dấu khung chữ nhật màu trắng ở đoạn các đường EMA cắt nhau trước phiên để minh họa vùng cần tránh nếu EMA rối loạn (`03:56`) [NÓI, HÌNH].
  - Vẽ vùng `FVG` màu tím tạo bởi nhịp tăng mạnh đầu phiên London (`04:16 - 04:36`) [NÓI, HÌNH].
  - Chỉ mũi tên màu cam vào cây nến đỏ lúc `16:30` hồi về vùng FVG và rút chân tạo râu dưới rất dài (nến từ chối giá) (`05:08`) [NÓI, HÌNH].
  - Chỉ vào cây nến tiếp theo lúc `17:00` (một cây nến đỏ nhỏ có râu trên) đóng cửa bên dưới đỉnh của cây nến từ chối giá lúc `16:30`, xác nhận đủ điều kiện vào lệnh (`05:56 - 06:32`) [NÓI, HÌNH].
- **Entry / SL / TP cụ thể**:
  - **Entry**: Vào lệnh Mua ngay khi đóng cây nến xác nhận lúc `17:00` [NÓI, HÌNH].
  - **SL**: Đặt ngay dưới râu dưới của cây nến từ chối giá lúc `16:30` [NÓI, HÌNH].
  - **TP (Thoát lệnh)**: Không đặt TP cố định ban đầu; sau đó đóng lệnh tại vùng mà các đường EMA bắt đầu thu hẹp khoảng cách, đan xen vào nhau (được khoanh khung chữ nhật trắng ở `07:12`) đồng thời xuất hiện vùng hỗ trợ ngang đi qua 4 đáy liên tiếp (vẽ bằng hộp chữ nhật đỏ ở `07:28`) [NÓI, HÌNH].
- **Kết quả và bài học tác giả rút ra**:
  - Giao dịch đạt lợi nhuận khoảng `8R` (trên công cụ Long Position hiển thị tỷ lệ R:R xấp xỉ `7.98`) [NÓI, HÌNH].
  - Bài học quản lý lệnh: Một vùng giá (hỗ trợ/vùng mua) càng bị kiểm tra nhiều lần (4 đáy liên tiếp) kèm theo EMA bắt đầu đan xen thì khả năng vùng đó bị phá vỡ càng cao, nên cần chủ động chốt lời thay vì cố giữ thêm [NÓI].
- **Minh họa quy tắc**: Ví dụ thuận chuẩn mực cho toàn bộ quy trình 3 bước vào lệnh và quy tắc thoát lệnh khi EMA đan xen kết hợp cấu trúc giá ở mục 4.

### 5.2 Ví dụ 2: Giao dịch Mua (Long) cặp XAUUSD (Vàng) trên khung M30
- **Mốc thời gian trong video**: `07:59 - 10:30` [NÓI, HÌNH].
- **Sản phẩm, khung thời gian, hướng lệnh**:
  - Sản phẩm: `XAUUSD` (Vàng/USD) [NÓI, HÌNH].
  - Khung thời gian: `30 phút (M30)` [NÓI, HÌNH].
  - Hướng lệnh: **Mua (Long)** [NÓI, HÌNH].
  - Thời điểm trên biểu đồ: Khoảng `16:00` ngày `28/08/2025` (`Thu 28 Aug '25 16:00` trên biểu đồ), nằm trong phiên thanh khoản London (`15:00 - 18:30` giờ Việt Nam) [NÓI, HÌNH].
- **Bối cảnh trước setup**:
  - Hệ thống `EMA 5, 9, 13, 21, 200` đang xếp chồng rõ ràng theo cùng một hướng tăng, giá nằm hoàn toàn trên `EMA 200`, xác nhận dòng tiền lớn đang đổ vào phe mua [NÓI, HÌNH].
- **Những gì tác giả chỉ/vẽ trên chart và lý do**:
  - Vẽ vùng `FVG` màu tím từ đỉnh cây nến `15:00` đến đáy cây nến `16:00` (do cây nến tăng mạnh lúc `15:30` tạo ra) (`08:32`) [NÓI, HÌNH].
  - Chỉ mũi tên màu cam vào cây nến lúc `16:30` hồi về vùng FVG: cây nến này có râu dưới khá dài xuyên qua FVG, nhưng **thân nến đỏ vẫn tương đối lớn và đóng cửa gần phía dưới vùng FVG**, cho thấy phe bán vẫn còn tạo áp lực nhất định (`08:40 - 09:00`) [NÓI, HÌNH].
  - Quan sát cây nến tiếp theo lúc `17:00`: xuất hiện một cây nến xanh nhỏ đóng cửa không vượt lên trên đỉnh của cây nến từ chối giá trước đó, hoàn tất đủ 5 điều kiện hội tụ (`09:08 - 09:32`) [NÓI, HÌNH].
- **Entry / SL / TP cụ thể**:
  - **Entry**: Vào lệnh Mua tại giá đóng cửa của cây nến xanh xác nhận lúc `17:00` ngày `28/08/2025` [NÓI, HÌNH].
  - **SL**: Đặt phía dưới đáy (Low) của cây nến từ chối giá lúc `16:30` [NÓI, HÌNH].
  - **Diễn biến gồng lệnh & Thoát lệnh**: Ngay sau khi vào lệnh vài nến, giá có một nhịp giảm rất mạnh xuyên sâu lại vào vùng FVG (`09:56`), nhưng chưa chạm điểm SL và cấu trúc các đường EMA vẫn giữ nguyên thứ tự xếp chồng nên tiếp tục giữ lệnh [NÓI, HÌNH]. Giá sau đó bật tăng mạnh cho đến khoảng `03:30 - 04:00` sáng ngày hôm sau (`Fri 29 Aug '25`), khi các đường EMA bắt đầu co cụm và đan xen vào nhau (khoanh khung trắng ở `10:16`) thì chủ động đóng lệnh [NÓI, HÌNH].
- **Kết quả và bài học tác giả rút ra**:
  - Giao dịch đạt lợi nhuận khoảng `5R` (trên công cụ Long Position hiển thị R:R khoảng `5.38`) [NÓI, HÌNH].
  - Bài học 1: Khi cây nến từ chối giá có thân nến ngược chiều (đỏ) khá lớn đóng cửa sát mép dưới FVG, cần thận trọng hơn và không kỳ vọng giữ lệnh quá xa như các setup lý tưởng [NÓI].
  - Bài học 2: Kỷ luật giữ lệnh khi có nhịp rũ bỏ mạnh nhưng chưa chạm SL và cấu trúc EMA chưa bị phá vỡ [NÓI].
- **Minh họa quy tắc**: Ví dụ thuận có biến thể (nến từ chối thân lớn và nhịp rũ sâu sau khi vào lệnh), minh họa cách đánh giá chất lượng nến từ chối và kỷ luật quản lý lệnh ở mục 4.

## 6. Tips, Tricks & Cảnh báo
- **Thời gian quan trọng hơn hành động giá**: Tuyệt đối chỉ săn lệnh trong khung giờ thanh khoản London (`03:00 - 06:30` giờ New York), đặc biệt chú ý các nến lúc `02:30`, `03:00` và `03:30` sáng giờ New York vì đây thường là các nến rất mạnh và sạch [NÓI, HÌNH].
- **Chi tiết dễ bị bỏ sót nhất ở Bước 3**: Đa số người xem phương pháp của Tyler thường vào lệnh ngay sau cây nến râu dài từ chối tại FVG mà quên mất điều kiện cây nến tiếp theo KHÔNG được đóng cửa vượt đỉnh nến từ chối; nếu vượt đỉnh, xác suất giá sớm quay đầu rất cao nên phải kiên quyết bỏ qua [NÓI].
- **Đánh giá độ mạnh yếu của Nến từ chối giá**: Dù có râu dưới dài, nếu cây nến từ chối có thân đỏ lớn đóng cửa gần cạnh dưới vùng FVG thì áp lực bán vẫn còn mạnh; nếu vào lệnh phải thận trọng và giảm kỳ vọng gồng xa [NÓI].
- **Không bị đánh lừa bởi vùng hỗ trợ nhiều đáy**: Khi đang gồng lệnh mua mà thấy giá chững lại tạo một vùng mua đi qua 4 đáy liên tiếp kèm EMA co cụm, đừng nghĩ đó là hỗ trợ mạnh để giữ tiếp; vùng giá bị test càng nhiều lần thì nguy cơ thủng càng cao, hãy dùng đó làm tín hiệu thoát lệnh [NÓI, HÌNH].
- **Chấp nhận tần suất giao dịch cực thấp**: Việc hội tụ đầy đủ mọi điều kiện (đúng giờ London + EMA xếp chồng chuẩn + có FVG + nến từ chối + nến xác nhận không vượt đỉnh) rất hiếm khi xảy ra liên tiếp trên một cặp tiền; cần tránh tâm lý ép lệnh hoặc giao dịch quá mức (overtrade) [NÓI, HÌNH].

## 7. Quản trị rủi ro & Tâm lý
- **Tư duy phân bổ tần suất & kỳ vọng lợi nhuận**:
  - Chuyển dịch từ tư duy đánh nhiều lệnh thắng ngắn (`200 lệnh Scalp` kiếm `1R/lệnh`) sang chọn lọc cực kỹ những cơ hội chất lượng cao (`10 setup/năm` trên mỗi cặp tiền với kỳ vọng lợi nhuận lớn như `5R`, `8R` đến `20R/lệnh`) [NÓI, HÌNH].
- **Yêu cầu tâm lý**:
  - Cần sự kiên nhẫn cao độ để chờ đúng setup vì không có nhiều cơ hội mỗi tuần [NÓI, HÌNH].
  - Tâm lý phải đủ vững để giữ lệnh trong thời gian dài và chịu được những nhịp giá giật ngược về vùng FVG khi chưa chạm SL và EMA chưa gãy cấu trúc [NÓI, HÌNH].
- **Risk % mỗi lệnh, công thức tính lot, giới hạn lỗ ngày/tuần**: VIDEO KHÔNG ĐỀ CẬP.

## 8. Đặc tả logic cho LLM / Bot

Lưu ý: Quy tắc cho lệnh `LONG` được trích xuất trực tiếp từ lời nói và biểu đồ trong video [NÓI, HÌNH]. Quy tắc cho lệnh `SHORT` được suy luận đối xứng hoàn toàn theo nguyên tắc đảo ngược thứ tự EMA và hướng giá mà tác giả nêu ở Bước 1 [NÓI, SUY LUẬN].

- **THAM SỐ HỆ THỐNG (PARAMETERS)**:
  - `TIMEFRAME` = `M30`
  - `SESSION_NY_START` = `03:00`
  - `SESSION_NY_END` = `06:30`
  - `EMA_PERIODS` = `[5, 9, 13, 21, 200]`
  - `SL_BUFFER_PIPS` = `0` (hoặc `UNSPECIFIED_IN_VIDEO`)

- **LOGIC CHO LỆNH MUA (LONG SETUP)**:
  - **ĐIỀU KIỆN BỐI CẢNH (CONTEXT)**:
    - IF `current_time_NY` >= `03:00` AND `current_time_NY` <= `06:30`
    - AND `Close` > `EMA_200`
    - AND `EMA_5` > `EMA_9` > `EMA_13` > `EMA_21` > `EMA_200`
    - AND `SUBJECTIVE: Tất cả các đường EMA (5, 9, 13, 21, 200) cùng dốc lên và không đan chéo nhau`
  - **ĐIỀU KIỆN VÙNG GIÁ (FVG DETECTION)**:
    - IF xuất hiện cụm 3 nến tăng mạnh tạo `Bullish_FVG`
    - WHERE `FVG_Bottom` = `Candle[i-2].High` AND `FVG_Top` = `Candle[i].Low` (với `FVG_Top` > `FVG_Bottom`)
  - **ĐIỀU KIỆN LỌC & KÍCH HOẠT (TRIGGER - BƯỚC 2 & BƯỚC 3)**:
    - WAIT cho giá hồi về vùng `Bullish_FVG` tại cây nến `Candle[r]` (Nến từ chối giá):
      - `Candle[r].Low` <= `FVG_Top` (Lưu ý: `Candle[r].Low` được phép < `FVG_Bottom`)
      - AND `SUBJECTIVE: Candle[r] có râu dưới rất dài (long lower wick) thể hiện sự từ chối giảm giá rõ ràng`
    - EVALUATE cây nến ngay tiếp theo `Candle[r+1]` (Nến xác nhận):
      - IF `Candle[r+1].Close` <= `Candle[r].High`
      - AND điều kiện `EMA_5 > EMA_9 > EMA_13 > EMA_21 > EMA_200` vẫn duy trì
      - THEN kích hoạt tín hiệu `VALID_LONG_ENTRY` khi `Candle[r+1]` đóng cửa.
  - **ĐIỀU KIỆN HỦY KÈO (INVALIDATION)**:
    - IF `Candle[r+1].Close` > `Candle[r].High` THEN hủy setup (`CANCEL_SETUP`).
    - OR IF các đường EMA đan chéo nhau trước khi vào lệnh THEN hủy setup (`CANCEL_SETUP`).
  - **VÀO LỆNH & DỪNG LỖ (ENTRY & SL)**:
    - `Entry_Price` = `Candle[r+1].Close` (Lệnh Market ngay khi đóng nến `Candle[r+1]`)
    - `Stop_Loss` = `Candle[r].Low`
  - **QUẢN LÝ LỆNH & THOÁT LỆNH (EXIT / TP)**:
    - `Take_Profit` = `NONE` (Không đặt TP cố định)
    - WHILE lệnh đang mở (`Position == OPEN`):
      - IF `Low` <= `Stop_Loss` THEN đóng lệnh tại `Stop_Loss`.
      - ELSE IF các đường `EMA_5, EMA_9, EMA_13, EMA_21` thu hẹp khoảng cách và cắt nhau (mất trật tự `EMA_5 > EMA_9 > EMA_13 > EMA_21`)
        - OR `SUBJECTIVE: Giá đi ngang tạo vùng hỗ trợ bị kiểm tra từ 4 đáy liên tiếp trở lên kèm EMA co cụm`
        - THEN đóng toàn bộ lệnh theo giá thị trường (`CLOSE_LONG_MARKET`).
      - ELSE (ngay cả khi giá giảm sâu lại vào vùng `Bullish_FVG` nhưng `Low` > `Stop_Loss` và trật tự EMA vẫn giữ nguyên):
        - THEN tiếp tục giữ lệnh (`HOLD_POSITION`).

- **LOGIC CHO LỆNH BÁN (SHORT SETUP - ĐỐI XỨNG)**:
  - **ĐIỀU KIỆN BỐI CẢNH (CONTEXT)**:
    - IF `current_time_NY` >= `03:00` AND `current_time_NY` <= `06:30`
    - AND `Close` < `EMA_200`
    - AND `EMA_5` < `EMA_9` < `EMA_13` < `EMA_21` < `EMA_200`
    - AND `SUBJECTIVE: Tất cả các đường EMA (5, 9, 13, 21, 200) cùng dốc xuống và không đan chéo nhau`
  - **ĐIỀU KIỆN VÙNG GIÁ (FVG DETECTION)**:
    - IF xuất hiện cụm 3 nến giảm mạnh tạo `Bearish_FVG`
    - WHERE `FVG_Top` = `Candle[i-2].Low` AND `FVG_Bottom` = `Candle[i].High` (với `FVG_Top` > `FVG_Bottom`)
  - **ĐIỀU KIỆN LỌC & KÍCH HOẠT (TRIGGER)**:
    - WAIT cho giá hồi lên vùng `Bearish_FVG` tại cây nến `Candle[r]` (Nến từ chối giá):
      - `Candle[r].High` >= `FVG_Bottom` (Lưu ý: `Candle[r].High` được phép > `FVG_Top`)
      - AND `SUBJECTIVE: Candle[r] có râu trên rất dài (long upper wick) thể hiện sự từ chối tăng giá rõ ràng`
    - EVALUATE cây nến ngay tiếp theo `Candle[r+1]` (Nến xác nhận):
      - IF `Candle[r+1].Close` >= `Candle[r].Low`
      - AND điều kiện `EMA_5 < EMA_9 < EMA_13 < EMA_21 < EMA_200` vẫn duy trì
      - THEN kích hoạt tín hiệu `VALID_SHORT_ENTRY` khi `Candle[r+1]` đóng cửa.
  - **ĐIỀU KIỆN HỦY KÈO (INVALIDATION)**:
    - IF `Candle[r+1].Close` < `Candle[r].Low` THEN hủy setup (`CANCEL_SETUP`).
  - **VÀO LỆNH & DỪNG LỖ (ENTRY & SL)**:
    - `Entry_Price` = `Candle[r+1].Close`
    - `Stop_Loss` = `Candle[r].High`
  - **QUẢN LÝ LỆNH & THOÁT LỆNH (EXIT / TP)**:
    - Đóng lệnh khi các đường `EMA_5, EMA_9, EMA_13, EMA_21` co cụm và cắt nhau mất trật tự `EMA_5 < EMA_9 < EMA_13 < EMA_21` hoặc tạo vùng kháng cự bị kiểm tra nhiều đỉnh liên tiếp.

## 9. Điểm mơ hồ, Mâu thuẫn & Thông tin thiếu
- **Mâu thuẫn cách gọi tên chỉ báo `MA` và `EMA`**:
  - Trong phần lời nói ở Ví dụ 1 (`02:42 - 03:55`), tác giả liên tục đọc là "MA" (`MA 5, 9, 13, 21 và 200`), nhưng đến `04:02` lại nói "khi EMA rối loạn", và toàn bộ chữ hiển thị trên màn hình (`02:40`, `03:08`, `03:16`, `03:28`, `03:48`, `09:20`) cũng như lời nói ở Ví dụ 2 (`08:16`, `09:20`, `09:45`) đều ghi/nói là `EMA`.
- **Mâu thuẫn quy đổi múi giờ New York sang giờ Việt Nam**:
  - Ở `01:44`, màn hình ghi rõ: `3:00 - 6:30 theo giờ New York` tương đương `15:00 đến 18:30 theo giờ Việt Nam (Mùa Đông)` và `14:00 đến 17:30 theo giờ Việt Nam (Mùa Hè)` [HÌNH].
  - Tuy nhiên ở `01:56`, màn hình ghi: `2:30, 3:00 và 3:30 New York (14h30, 15h, 15h30 Việt Nam)` [HÌNH] – đây là mức quy đổi theo giờ Mùa Đông (UTC-5, chênh 12 tiếng so với UTC+7).
  - Thêm vào đó, trong cả hai ví dụ biểu đồ (tháng 4 và tháng 8 đều thuộc giờ Mùa Hè EDT của Mỹ, tức 3:00 NY = 14:00 VN), tác giả vẫn dùng cố định khung giờ `15:00 đến 18:30` trên trục thời gian biểu đồ và gọi đó là phiên London [NÓI, HÌNH].
- **Mâu thuẫn năm của dữ liệu biểu đồ ở Ví dụ 1**:
  - Ở `02:56`, tác giả nói "cây nến hiện tại đang vào lúc 15 giờ ngày mùng 7 tháng 4 năm 2026" [NÓI], nhưng nhãn thời gian dưới trục ngang của TradingView hiển thị rõ là `Tue 07 Apr '20 15:00` (tức thứ Ba ngày 07/04/2020) [HÌNH].
- **Mâu thuẫn nhỏ giữa lý thuyết vẽ FVG và cách kẻ hộp FVG trong Ví dụ 1**:
  - Ở `04:31`, tác giả nêu quy tắc chuẩn: vẽ FVG "từ điểm cao nhất của cây nến thứ nhất đến điểm thấp nhất của cây nến thứ ba" [NÓI].
  - Tuy nhiên trên biểu đồ Ví dụ 1 (`04:16 - 04:36`), hộp FVG được kẻ bao quanh vùng thân/râu của cụm nến tăng lúc `14:30 - 15:30` mà cạnh trên kéo ngang qua vùng giá đóng cửa/mở cửa của nến `15:00 - 15:30` thay vì đúng đáy của cây nến thứ ba [HÌNH]. Ngược lại, ở Ví dụ 2 (`08:32`), hộp FVG được vẽ chuẩn xác từ đỉnh cây nến `15:00` đến đáy cây nến `16:00` [HÌNH].
- **Các thông số định lượng còn thiếu (cần làm rõ nếu lập trình Bot)**:
  - Chưa có định nghĩa toán học cho "cây nến từ chối giá có râu dưới rất dài" (ví dụ: tỷ lệ chiều dài râu dưới so với tổng chiều dài nến `High - Low` hoặc so với thân nến phải đạt bao nhiêu %).
  - Chưa quy định rõ giới hạn thời gian tối đa: Nếu vùng FVG và cây nến đầu tiên hình thành trong khung `03:00 - 06:30` NY, nhưng giá hồi về FVG và đóng nến xác nhận sau `06:30` NY thì còn hợp lệ hay không (trong cả 2 ví dụ của video, nến xác nhận đều đóng lúc `17:00`, tức vẫn nằm trong khung `15:00 - 18:30` mà tác giả xét).
  - Không hiển thị rõ mức giá số học (Price level) trên trục tung của TradingView do trục giá bên phải bị cắt/mờ trong khung hình dọc.

## 10. Thông tin khác
- **Thông tin kênh & tác giả được nhắc tới**:
  - Tác giả phương pháp gốc: **Tyler** (biệt danh **TG Capital**) [NÓI].
  - Kênh thực hiện video phân tích & backtest: **Safe Trade (S TRADE - SAFE TRADING)** [NÓI, HÌNH].
- **Kết quả/thống kê được đề cập trong video (chưa được kiểm chứng độc lập)**:
  - Thông số của Tyler được giới thiệu ở đầu video: Tỷ lệ thắng (Winrate) công bố khoảng `90%`, tỷ lệ lời lỗ (R:R) thường từ `20R` trở lên, xây dựng từ hơn `6 năm` backtest, mỗi cặp tiền có khoảng `10 setup/năm` [NÓI, HÌNH].
  - Kết quả 2 ví dụ kiểm chứng của kênh Safe Trade trong video: Ví dụ 1 trên `EURUSD` đạt khoảng `8R` (`7.98R` trên hình); Ví dụ 2 trên `XAUUSD` đạt khoảng `5R` (`5.38R` trên hình) [NÓI, HÌNH].
- **Quảng cáo / Upsell trong video**:
  - Từ `00:42 - 00:58`: Mời tham gia nhóm cộng đồng giao dịch vàng miễn phí qua link ở phần bio (hình chụp màn hình nhóm Zalo "CỘNG ĐỒNG GIAO DỊCH" của Nguyễn Duy Lực) [NÓI, HÌNH].
  - Từ `11:38 - 11:52`: Giới thiệu khóa học Price Action toàn diện và thông tin liên hệ Zalo `0335303867`, Email `SAFETRADE1997@GMAIL.COM`, YouTube/TikTok `@SAFETRADE1997`, Telegram `T.ME/SAFETRADE1997` [NÓI, HÌNH].
- **Trích dẫn nguyên văn đáng giữ**:
  - "Nhiều lệnh không có nghĩa là nhiều tiền. Chất lượng mới là thứ quan trọng." (`01:28`) [NÓI].
  - "Thời gian quan trọng hơn hành động giá." (`01:38`) [NÓI].
  - "Cây nến tiếp theo không được đóng cửa vượt lên trên đỉnh của cây nến từ chối giá vừa xuất hiện." (`05:53`) [NÓI, HÌNH].
  - "Một vùng giá càng bị kiểm tra nhiều lần thì khả năng vùng đó bị phá vỡ càng cao." (`07:38`) [NÓI].
- **Ghi chú của người trích xuất**:
  - [SUY LUẬN] Khi chuyển hóa phương pháp này thành Expert Advisor (EA) trên MT4/MT5 cho `XAUUSD` hoặc `EURUSD`, cần đặc biệt lưu ý tham số múi giờ Server của sàn (thường là GMT+2 mùa đông và GMT+3 mùa hè, tương ứng `03:00 - 06:30` giờ New York sẽ cố định là `10:00 - 13:30` theo giờ Server MT4/MT5 quanh năm mà không bị lệch bởi DST giữa Mỹ và Việt Nam).
  - [SUY LUẬN] Để định lượng hóa điều kiện "nến từ chối râu dài" và "thân nến không quá lớn đóng sát dưới FVG" như tác giả lưu ý ở Ví dụ 2, khi lập trình bot có thể thêm bộ lọc tỷ lệ `Lower_Wick / Candle_Range >= 0.5` và kiểm tra vị trí giá đóng cửa của nến từ chối so với `FVG_Bottom`.