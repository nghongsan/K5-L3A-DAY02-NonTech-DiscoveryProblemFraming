# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thị Hồng Hạnh
- MSSV: 2A202603537
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NonTech
- Link repo nhóm: https://github.com/nghongsan/K5-L3A-DAY02-NonTech-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.
**Bối cảnh**: Tôi là nhân viên vận hành sàn thương mại điện tử. Mỗi buổi sáng, tôi tải dữ liệu từ sàn, tổng hợp chỉ số của ngày hôm qua. Cuối tuần sẽ tổng hợp thêm số liệu 7 ngày qua. Cuối tháng tổng hợp số liệu 30 ngày qua, sau đó chuyển dữ liệu sang định dạng báo cáo của công ty. Tôi cũng rà tiến độ các campaign trong tháng và lên kế hoạch làm việc với Marketing và bộ phận kho.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại|Khi bắt đầu buổi sáng, tôi muốn chuyển dữ liệu tải từ sàn sang đúng mẫu báo cáo công ty, để có đủ số liệu cho ba kỳ báo cáo. |Tôi, Team vận hành sàn |Việc chuyển đổi diễn ra mỗi buổi sáng. Thời gian khoảng 30p cho báo cáo ngày, 45p-60p cho báo cáo tuần. 1h-1h30 cho báo cáo tháng |
| 2 |Lặp lại |Khi lập báo cáo ngày hôm qua, 7 ngày và 30 ngày, tôi muốn kiểm tra mỗi chỉ số đang lấy đúng kỳ, để người đọc so sánh đúng phạm vi. |Tôi, Team vận hành | Mỗi kỳ tổng hợp cần check mốc ngày bắt đầu và kết thúc, số liệu cuối ngày chốt sổ, thời gian khoảng 30-45p|
| 3 | Tốn thời gian| Khi số liệu trên báo cáo công ty khác số liệu nguồn, tôi muốn truy được ô đó lấy từ file nào, cột nào và kỳ nào, để xác định chỗ cần sửa.|Tôi | Kiểm tra mỗi khi có chênh lệch số liệu, có thể là budget, tồn kho.|
| 4 |Cần đọc, tổng hợp nhiều thông tin | Khi rà các campaign trong tháng, tôi muốn nhìn được tiến độ và mốc tiếp theo của từng campaign, để biết việc nào cần xử lý trước.|Tôi, Marketing, Kho | Tôi có bước rà campaign trong công việc. Kiểm tra thông tin hiện nằm ở đâu và mất bao lâu để cập nhật trạng thái.|
| 5 |Pain từ người khác | Khi chuẩn bị campaign có sản phẩm cần kho xác nhận, tôi muốn biết SKU nào đã sẵn sàng và SKU nào còn chờ, để chốt kế hoạch với Marketing.|Tôi, Marketing, Kho |Campaign gần nhất cần kho xác nhận và thời gian chờ phản hồi khoảng 1-3 ngày. |
| 6 |Pain từ người khác | Khi Marketing thay đổi lịch hoặc danh sách sản phẩm của campaign, tôi muốn biết phần nào cần xác nhận lại với kho, để các bên làm theo cùng một kế hoạch.|Tôi, Marketing, kho |Phải update liên tục vào các ngày campaign để không gián đoạn kinh doanh, thời gian check mỗi ngày cần 20-30p |
| 7 |Cần đọc, tổng hợp nhiều thông tin |Khi lập kế hoạch làm việc sau khi rà campaign, tôi muốn xác định việc cần làm, người phụ trách và hạn phản hồi, để theo dõi đến lúc có kết quả. |Tôi, Marketing, kho | Tôi lên plan, kiểm tra các đầu việc của một campaign xem có mục nào thiếu người phụ trách hoặc hạn xử lý.|
| 8 |Tốn thời gian| Khi số liệu biến động, tôi muốn xác định chỉ số và kỳ nào cần kiểm tra trước, để tập trung thời gian vào những thay đổi đáng chú ý.|Tôi, Team vận hành | Khi có biến động cần họp với team marketing để theo dõi tiến độ, giải quyết mất khoảng 30p-1h để tìm nguyên nhân và giải pháp.|

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
- Tôi là người chọn bối cảnh và gợi ý các tình huống. AI gợi ý mục #6, #8
- Tôi không bỏ ý nào vì tôi thấy các ý trên đều cần thiết, tuy nhiên có những ý trùng cần phân tích sâu hơn xem có cần thiết dùng AI hay không.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chuyển báo cáo sàn sang mẫu báo cáo công ty (#1)|Quy trình rõ, tốn thời gian, có baseline đo thật | Narrative "đủ tốt" đo thế nào?|
| 2 | Cần kho xác nhận hàng tồn và hàng cần chuẩn bị (#5)|Quy trình rõ, rút ngắn được sẽ giúp flow làm việc tốt hơn|Sự sẵn sàng phối hợp của team kho|
| 3 |Rà soát tiến độ campaign trong tháng (#4)| Tiến độ campaign ảnh hưởng trực tiếp tới doanh thu, có thể kiểm soát đo lường được| Campaign không cố định theo season, số liệu nhiều campaign cùng lúc chảy về không đo lường được |

### Problem Card #1 — Chuyển báo cáo sàn sang mẫu báo cáo công ty (ý #1)

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu ca sáng, tôi muốn chuyển dữ liệu từ báo cáo sàn sang mẫu báo cáo công ty và tóm tắt các biến động đáng chú ý, để cả nhóm có số liệu thống nhất trước khi quyết định việc cần xử lý trong ngày. |
| Actor | Nhân viên vận hành sàn TMĐT lập báo cáo. Quản lý và các nhóm liên quan đọc báo cáo. |
| Thời điểm / bối cảnh | Mỗi sáng, cần tổng hợp số liệu ngày hôm qua. Mỗi cuối tuần, cần tổng hợp số liệu 7 ngày qua và Mỗi tháng, cần tổng hợp số liệu của 30 ngày qua. |
| Quy trình hiện tại (3–7 bước) | 1. Tải báo cáo từ sàn.<br>2. Chọn dữ liệu theo từng kỳ báo cáo.<br>3. Đối chiếu cột dữ liệu với chỉ số trong mẫu công ty.<br>4. Tính và điền số liệu vào mẫu.<br>5. Kiểm tra lại số liệu, viết nhận xét và gửi báo cáo. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4 lặp lại mỗi sáng vì định dạng báo cáo sàn khác mẫu công ty. 15-30p từ lần đo thực tế. Bước 5 mất khoảng 20p để dựng báo cáo |
| Impact (nếu không giải thì sao) | Báo cáo gửi muộn làm chậm việc chốt ưu tiên trong ngày. Nếu điền sai cột hoặc sai kỳ, team vận hành có thể đánh giá sai biến động doanh thu hoặc đơn hàng. |
| Success metric (baseline → target) | Thời gian từ lúc có file nguồn đến lúc gửi báo cáo **giảm ít nhất 30%**, với phạm vi báo cáo tương đương. Với phần nhận xét, đo tỷ lệ bản nháp được người phụ trách duyệt mà không phải sửa nội dung **≥90%**.|
| Phương án không dùng AI | Dùng Power Query hoặc script để ánh xạ cột, tính chỉ số theo từng kỳ và điền vào mẫu. Dùng ngưỡng do team thống nhất để đánh dấu các biến động cần xem. |
| Giả thuyết về AI (nếu có) | Khi bảng chỉ số đã được đối soát, AI có thể viết nháp phần nhận xét, kèm số liệu và kỳ so sánh cho từng ý. Thời gian chỉnh sửa và duyệt chỉ khoảng 10-15p |
| Cảm nhận nhanh | **Rule** cho phần chuyển đổi báo cáo. Có thể thử AI riêng cho phần nhận xét. |

Quy trình nháp hiện tại

```text
Tải file báo cáo từ sàn
→ Chọn dữ liệu ngày hôm qua, 7 ngày qua và 30 ngày qua
→ Đối chiếu cột nguồn với mẫu công ty
→ Tính chỉ số và điền vào mẫu
→ Kiểm tra số liệu, viết nhận xét và gửi báo cáo
```

### Problem Card #2 — Cần kho xác nhận hàng tồn và hàng cần chuẩn bị (ý #5)

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị hàng cho campaign, tôi muốn biết kho có thể bố trí bao nhiêu hàng theo từng SKU và khi nào hàng sẵn sàng, để chốt số lượng bán và kế hoạch chạy với marketing. |
| Actor | Nhân viên vận hành sàn gửi yêu cầu. Nhân viên kho kiểm tra và xác nhận. Marketing dùng thông tin để chốt kế hoạch. |
| Thời điểm / bối cảnh | Trước khi chốt kế hoạch campaign hoặc khi số lượng hàng cần chuẩn bị thay đổi. |
| Quy trình hiện tại (3–7 bước) | 1. Lập danh sách SKU, số lượng cần và hạn chuẩn bị.<br>2. Gửi yêu cầu cho kho.<br>3. Kho đối chiếu tồn và kiểm tra số lượng có thể bố trí.<br>4. Vận hành theo dõi, nhắc hoặc hỏi lại những SKU còn thiếu thông tin.<br>5. Tổng hợp xác nhận và cập nhật kế hoạch với marketing. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4 phụ thuộc vào phản hồi của kho. Cần **[60-120 phút chờ/yêu cầu]** từ lúc gửi đến lúc nhận đủ số lượng và thời điểm sẵn sàng. **[15 phút thao tác/yêu cầu]** để biết vận hành mất bao lâu cho việc nhắc và tổng hợp. |
| Impact (nếu không giải thì sao) | Marketing có thể phải chờ chốt kế hoạch hoặc sửa chương trình sát giờ. Nếu dùng số tồn chưa được xác nhận, vận hành có thể mở bán vượt số lượng kho thực sự bố trí được. |
| Success metric (baseline → target) | Thời gian trung vị từ lúc gửi đến lúc nhận đủ xác nhận **giảm ít nhất 25%**. Tỷ lệ yêu cầu được xác nhận trước hạn **≥90%**. Theo dõi thêm tỷ lệ yêu cầu kho cập nhật đúng nơi quy định để kiểm chứng mức độ phối hợp. |
| Phương án không dùng AI | Dùng bảng chung với mỗi dòng là một SKU trong một yêu cầu. Có cột số lượng cần, số lượng kho xác nhận, thời điểm sẵn sàng, người phụ trách và hạn phản hồi. Thống nhất với kho nơi cập nhật và quy tắc nhắc khi gần đến hạn. |
| Giả thuyết về AI (nếu có) | Nếu kho thường xác nhận bằng tin nhắn tự do, AI có thể trích SKU, số lượng và thời điểm sẵn sàng để điền nháp vào bảng. Kho xác nhận lại thông tin trước khi vận hành dùng để chốt kế hoạch. |
| Cảm nhận nhanh | **Workflow**. Mức cải thiện phụ thuộc vào việc kho có thể phản hồi đúng hạn và cập nhật đủ thông tin. |

Quy trình nháp hiện tại

```text
Lập danh sách SKU, số lượng cần và hạn chuẩn bị
→ Gửi yêu cầu cho kho
→ Kho kiểm tra số lượng có thể bố trí
→ Nhắc hoặc hỏi lại các mục còn thiếu
→ Tổng hợp xác nhận và cập nhật kế hoạch với marketing
```

### Problem Card #3 — Rà soát tiến độ campaign trong tháng (ý #4)

| Trường | Nội dung |
|---|---|
| Job Story | Khi rà soát các campaign đang chạy trong tháng, tôi muốn biết campaign nào lệch kế hoạch hoặc thiếu dữ liệu để đánh giá, để ưu tiên làm việc với marketing và kho trước khi hết thời gian điều chỉnh. |
| Actor | Nhân viên vận hành sàn theo dõi tiến độ. Marketing và kho phối hợp xử lý các vấn đề thuộc phần việc của mình. |
| Thời điểm / bối cảnh | Trong tháng, nhiều campaign có thể chạy chồng nhau, khác ngày bắt đầu, thời lượng và mục tiêu. Số liệu có thể về ở cấp campaign hoặc chỉ ở cấp gian hàng. |
| Quy trình hiện tại (3–7 bước) | 1. Lấy danh sách campaign đang chạy và các mốc kế hoạch.<br>2. Tải hoặc tổng hợp số liệu từ sàn.<br>3. Kiểm tra số liệu nào gắn được với từng campaign.<br>4. So sánh kết quả với mốc kế hoạch tại thời điểm rà soát.<br>5. Ghi nhận vấn đề, trao đổi với marketing hoặc kho và theo dõi xử lý. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4 tốn thời gian vì phải xác định số liệu thuộc campaign nào và đối chiếu theo các mốc khác nhau mất **[30-45 phút/lần rà soát]**, kèm số campaign đang chạy và số campaign có dữ liệu tách riêng. |
| Impact (nếu không giải thì sao) | Team có thể phát hiện chậm campaign lệch tiến độ và còn ít thời gian để điều chỉnh. Nếu gán doanh thu chung của gian hàng cho một campaign, team có thể ưu tiên sai việc. |
| Success metric (baseline → target) | Thời gian rà soát một lượt với số campaign tương đương **giảm ít nhất 30%**. Tỷ lệ campaign đang chạy có trạng thái rõ theo mốc rà soát **100%**, gồm đúng tiến độ, lệch tiến độ hoặc thiếu dữ liệu để đánh giá. Theo dõi riêng tỷ lệ campaign có chỉ số gắn được với mã campaign để biết phạm vi có thể đánh giá hiệu quả. |
| Phương án không dùng AI | Dùng tracker theo mã campaign, ngày bắt đầu và kết thúc, mục tiêu, mốc kiểm tra, nguồn số liệu và người phụ trách. So sánh theo mốc kế hoạch riêng của từng campaign. Nếu chỉ có doanh thu cấp gian hàng, hiển thị ở cấp gian hàng và đánh dấu campaign là thiếu dữ liệu cho chỉ số đó. |
| Giả thuyết về AI (nếu có) | Từ tracker và các chỉ số đã gắn đúng campaign, AI có thể tóm tắt các trường hợp lệch tiến độ, việc đang chờ và dữ liệu còn thiếu để chuẩn bị buổi rà soát. Kiểm chứng bằng thời gian chuẩn bị và số mục tóm tắt phải sửa. |
| Cảm nhận nhanh | **Workflow**. Có thể thêm **Rule** để cảnh báo lệch mốc khi chỉ số và mốc kế hoạch đã rõ. |

Quy trình nháp hiện tại

```text
Lấy danh sách campaign đang chạy và các mốc kế hoạch
→ Tổng hợp số liệu từ sàn
→ Kiểm tra chỉ số nào gắn được với từng campaign
→ Đối chiếu với mốc của từng campaign hoặc ghi nhận thiếu dữ liệu
→ Chốt việc cần xử lý với marketing hoặc kho và theo dõi
```
### Card muốn pitch nhất

- Card số: 01
- Vì sao: Công việc diễn ra mỗi buổi sáng, đầu vào là dữ liệu tải từ sàn và đầu ra là báo cáo theo mẫu công ty. Tôi có thể bấm giờ từng bước, thử chuyển đổi theo quy tắc và đối chiếu trực tiếp báo cáo đầu ra.
- Câu hỏi muốn nhóm phản biện: Nếu bước chuyển đổi dữ liệu chỉ mất vài phút nhưng tôi vẫn phải kiểm tra lại số liệu trước khi gửi, nhóm sẽ dựa vào phép đo nào để quyết định nên ưu tiên tự động hóa bước chuyển đổi hay cải thiện bước đối soát?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card giả định chuyển đổi dữ liệu là bước tốn thời gian nhất, nhưng chưa có số phút riêng để so sánh với bước đối soát và viết nhận xét. | Đồng ý | Tách ba bước để bấm giờ riêng: chuyển đổi dữ liệu, đối soát số liệu và viết nhận xét. Dùng kết quả đo để chọn bước cần ưu tiên. |
| Chỉ đo thời gian làm báo cáo có thể bỏ sót lỗi sai số liệu hoặc sai kỳ báo cáo. | Đồng ý | Bổ sung bước đối chiếu các chỉ số trong mẫu công ty với dữ liệu nguồn cho cả ba kỳ: ngày hôm qua, 7 ngày qua và 30 ngày qua. Đánh giá mức tiết kiệm thời gian trên các báo cáo đã qua đối soát. |
| Card chưa làm rõ phần việc nào cần AI và thế nào là một nhận xét đủ tốt để gửi. | Đồng ý | Tách phần chuyển đổi theo quy tắc bằng Power Query khỏi phần viết nhận xét. Chỉ cân nhắc thử AI nếu bước viết nhận xét thực sự tốn thời gian. Khi thử, đo cả thời gian duyệt và chỉnh sửa. Nhận xét đạt khi đúng số liệu, nêu rõ kỳ so sánh và chỉ ra biến động đáng chú ý. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi trình bày vấn đề, người gặp vấn đề và tình huống phát sinh để nhóm cùng thảo luận. | Nhóm có thêm một vấn đề để đối chiếu với các card còn lại. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Có tình huống thực tế nào cho thấy vấn đề này xảy ra thường xuyên và ảnh hưởng đến người dùng? | Câu hỏi giúp nhóm làm rõ căn cứ để đánh giá mức độ ưu tiên của vấn đề. |
| Nhận phản biện | Câu hỏi tôi nhận được: Phạm vi vấn đề đã đủ cụ thể để nhóm kiểm chứng chưa? | Tôi rà lại cách mô tả, làm rõ người gặp vấn đề, thời điểm phát sinh và điều còn cần xác minh. |
| Gom cluster / cây OST | Tôi cùng nhóm đối chiếu các card, tìm những nhu cầu chung và góp ý cách sắp xếp các nhánh trên cây OST. | Nhóm nhìn rõ mối liên hệ giữa các vấn đề và những nhu cầu cần xem xét tiếp. |
| Chọn candidate problem | Tôi góp ý khi nhóm so sánh các ứng viên dựa trên mức độ ảnh hưởng, bằng chứng hiện có và khả năng kiểm chứng. | Nhóm có căn cứ chung để thu hẹp danh sách bài toán. |
| Kiểm chứng / research | Tôi cùng nhóm rà soát thông tin đã có và góp ý những giả định cần kiểm tra thêm. | Bài nhóm phân biệt rõ các quan sát ban đầu với những điểm còn cần bằng chứng. |
| Quy trình nhóm | Tôi góp ý mô tả các bước trong quy trình hiện tại và xác định bước có thể gây chậm hoặc phát sinh thao tác lặp lại. | Nhóm có cơ sở để xác định điểm nghẽn cần tập trung phân tích. |
| Problem Statement | Tôi góp ý cách diễn đạt để nêu rõ ai gặp vấn đề, vấn đề xảy ra khi nào và gây ảnh hưởng gì. | Mô tả vấn đề của nhóm cụ thể hơn và có thể dùng để định hướng việc kiểm chứng. |
| Mức can thiệp AI | Tôi cùng nhóm xem xét bước nào có thể xử lý bằng quy tắc hoặc điều chỉnh quy trình, và bước nào có thể cần AI hỗ trợ. | Nhóm có cơ sở để giới hạn phạm vi sử dụng AI theo từng bước công việc. |
| Quyết định | Tôi tham gia thảo luận về bài toán ưu tiên và những điểm cần kiểm chứng tiếp. | Bài nhóm ghi lại lý do lựa chọn và hướng kiểm chứng tiếp theo. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Tôi đưa bối chân dung và context, AI gợi ý break down các công việc có thể ứng dụng AI |AI viết lại ý tưởng mạch lạc hơn |AI chỉ nói chung chung chưa thể đưa ra số liệu vì ko thực tế làm |Tôi sửa lại trau chuốt các chi tiết và add thêm ý tưởng rõ hơn cho AI |
| CP2 Problem Card |Tôi dùng AI để diễn đạt ý tưởng|AI giúp tôi chỉnh sửa format, phân tích sâu hơn, đưa thêm góc nhìn những điểm cần bổ sung |AI ko hiểu rõ quy trình làm việc nên có những ý tưởng bị trùng lặp ko cần thiết |Tôi bỏ các ý tưởng trùng lặp |
| CP4 Research | Tôi dùng AI để gợi ý câu hỏi kiểm chứng cho bài toán nhóm đang xem xét. | AI giúp tôi tách thông tin nhóm đã có khỏi những giả định cần hỏi thêm, như vấn đề xảy ra thường xuyên đến đâu và ảnh hưởng thế nào đến người dùng. | Một số câu hỏi còn rộng, dễ nhận được câu trả lời chung chung mà khó đối chiếu với tình huống thực tế. | Tôi thu hẹp câu hỏi vào lần gần nhất vấn đề xảy ra và ưu tiên ghi nhận ví dụ cụ thể từ người trực tiếp gặp vấn đề. |
| CP5 Quy trình | Tôi dùng AI để sắp xếp các bước trong quy trình hiện tại và gợi ý điểm nghẽn cần xem xét. | AI giúp trình bày rõ thứ tự các bước và chỉ ra chỗ có thể phát sinh chờ đợi hoặc làm lại. | AI có xu hướng mô tả quy trình theo một luồng lý tưởng và dễ xem bước có nhiều thao tác là bước gây chậm nhất. | Tôi đối chiếu với mô tả của nhóm, chỉnh lại các bước cho sát thực tế và ghi rõ điểm nghẽn nào còn cần kiểm chứng. |
| CP5–6 Problem Statement | Tôi dùng AI để viết lại bản mô tả vấn đề từ nội dung nhóm đã thảo luận. | AI giúp câu mô tả gọn hơn và làm rõ ai gặp vấn đề, trong tình huống nào và chịu ảnh hưởng gì. | Một số cách viết đưa giải pháp vào quá sớm hoặc diễn đạt nguyên nhân còn đang được kiểm chứng như một kết luận. | Tôi bỏ phần đề xuất giải pháp khỏi câu mô tả và chỉ giữ những ảnh hưởng có căn cứ từ thông tin nhóm đã thu thập. |
| CP6 Mức can thiệp / quyết định | Tôi dùng AI để so sánh các mức can thiệp và rà lại lý do chọn hướng xử lý của nhóm. | AI giúp phân biệt việc có thể xử lý bằng quy tắc, việc cần điều chỉnh quy trình và việc có thể thử AI hỗ trợ. | Gợi ý ban đầu chưa tính đủ đến dữ liệu nhóm có thể tiếp cận và công sức kiểm tra đầu ra. | Tôi cân nhắc lại theo dữ liệu, thời gian và khả năng kiểm chứng của nhóm, rồi làm rõ AI có thể hỗ trợ ở bước nào và bước nào cần người kiểm tra. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?** Các problems khi nhìn chung bề ngoài sẽ thấy không phải problem, nhưng khi bóc tách ra thì có nhiều cách cải thiện để giúp việc học tập và làm việc hiệu suất hơn rất nhiều.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?** Nhóm ko bị solution-first, nhưng vấn đề đưa ra thường chung chung như tổng hợp tài liệu, những problems này ở hiện tại đều có các công cụ để giải quyết. Vấn đề chỉ nằm ở sự chủ động của cá nhân, hay sự sẵn sàng phối hợp của các phòng ban trong quá trình làm việc.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.** Không có, vì những vấn đề tôi gặp trong thực tế, các bạn giúp tôi có thêm góc nhìn nhưng quan điểm vẫn chưa thay đổi.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?** Research không làm tôi bất ngờ vì đây thật sự là vấn đề chung, muốn thay đổi phải có độ trễ nhất định để thay đổi thói quen và tư duy của con người.

**6.5. Điều khó nhất khi viết Problem Statement là gì?** Điều khó nhất là xác định boundary của problems, vì giới hạn không đặt ra cụ thể có thể dẫn tới thảm hoạ.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?** Tôi sẽ không thay đổi gì cả.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo
