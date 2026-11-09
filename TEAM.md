# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: NonTech
- Candidate problem nhóm chọn (1 câu): Mỗi buổi sáng, nhân viên vận hành sàn thương mại điện tử phải chuyển dữ liệu tải từ sàn sang đúng mẫu báo cáo công ty cho 3 kỳ (hôm qua, 7 ngày, 30 ngày) trước khi có số liệu dùng trong ngày (candidate #7).
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Thị Hồng San | 2A202603513 | Viết Problem Statement, quy trình | nghongsan |
| 2 | Nguyễn Thị Thanh Thúy | 2A202603523 | Ghi chép, phụ trách kiểm chứng (phỏng vấn) | thuydesign |
| 3 | Nguyễn Thị Hồng Hạnh | 2A202603537 | Chủ domain của candidate #7, đo baseline, vẽ quy trình | hanhshi96 |
| 4 | Hoàng Lam Minh | 2A202603566 | Phụ trách research công cụ (Power Query), tài liệu tham khảo | laminh-h |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Thị Hồng San | Cả nhóm | Cluster, cây OST, bảng chấm điểm (mục 2 trong `group_report.md`) |
| CP4 — Kiểm chứng | Nguyễn Thị Thanh Thúy | Nguyễn Thị Hồng Hạnh | Assumption map, interview snapshot (mục 3.1–3.2; `report/assets/cp4-interview-snapshot-N.md`) |
| CP4 — Research | Hoàng Lam Minh | Nguyễn Thị Hồng Hạnh | Bảng research có link (mục 3.3) |
| CP5 — Quy trình trước/sau | Nguyễn Thị Hồng Hạnh | Nguyễn Thị Hồng San | Quy trình + bảng before/after (mục 4; `report/assets/cp5-baseline-log.md`) |
| CP5 — Problem Statement v0 | Nguyễn Thị Hồng San | Nguyễn Thị Hồng Hạnh | Problem Statement v0 (mục 5) |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Thị Hồng San | Hoàng Lam Minh | Ma trận, AI Canvas, tiêu chí đánh giá, Problem Statement v1 (mục 6–7) |
| CP6 — Quyết định | Cả nhóm | — | 4 rủi ro + Not Yet, ngưỡng dừng (mục 8) |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenThiHongSan-2A202603513

**Phần việc phụ trách:**

- Fork repo, mời thành viên.
- CP3 (hội tụ nhóm), CP5 Problem Statement v0, CP6 mức can thiệp và Problem Statement v1; hỗ trợ vẽ quy trình CP5.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch 3 card (#1 phòng trọ, #2 CV theo JD, #3 calo) với số liệu đã bấm giờ (135 phút/tháng; 75 phút/JD).
- Đề xuất gom cluster B và gạch các tên giải pháp ("app quản lý nhà trọ AI") khỏi tầng opportunity của cây OST.
- Chấm lại bảng shortlist, ghi lý do chọn #7 và loại các candidate còn lại, đặt ngưỡng đổi đề tài.
- Soạn mục 4–10 của `group_report.md` (quy trình trước/sau, Problem Statement v0/v1, mức can thiệp, quyết định, hạn chế, tài liệu tham khảo) với hỗ trợ của AI (Claude); phần phản biện của AI được ghi rõ nguồn ở mục 5.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: mục 2.1 (dòng #1–#3 và câu phản biện ở dòng #5, #7), mục 2.4, mục 4–10.
- `report/assets/cp5-baseline-log.md`.
- Commit từ tài khoản `nghongsan`.

**Điều mình học được từ phần nhóm:**

- Card có số liệu bấm giờ thật dễ thuyết phục nhóm hơn card chỉ ghi "chưa đo", nên đo trước khi pitch.
- Chọn đề tài không chỉ dựa vào tổng điểm: cần hỏi thêm "công cụ có sẵn đã giải được chưa" và tần suất lặp lại; khi chọn khác điểm cao nhất thì phải ghi lý do và ngưỡng đổi đề tài.
- Không phải bước nào cũng cần AI: với #7, phần số liệu chỉ cần Rule; AI chỉ đáng xét ở bước Rule không làm được.

### NguyenThiThanhThuy-2A202603523

**Phần việc phụ trách:**

- Ghi chép trong các buổi thảo luận nhóm.
- CP4 kiểm chứng: lập danh sách câu hỏi phỏng vấn theo kiểu hỏi về lần gần nhất, phỏng vấn ít nhất 2 người làm báo cáo sàn (ngoài Hạnh), viết interview snapshot và bảng tổng hợp ở mục 3.2.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch 3 card: #4 sàng lọc tài liệu cho bài tập nhóm, #5 gom và đối chiếu góp ý bản nháp, #6 chốt lịch họp nhóm. Cả 3 card đều ghi rõ bottleneck là giả thuyết, chưa đo, và đều có phương án không dùng AI.
- Card #5 và #4 góp vào cluster C ("Sàng lọc và đối chiếu thông tin theo tiêu chí"), card #6 góp vào cluster B; giúp nhóm thấy pattern chung là tiêu chí chưa được viết ra từ đầu.
- Phụ trách kiểm chứng giả định 1, 2, 4 trong Assumption Map (mục 3.1) qua phỏng vấn.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (dòng #4–#6), mục 2.2 (cluster B, C), mục 3.2.
- `report/assets/cp4-interview-snapshot-N.md`.
- Commit từ tài khoản `thuydesign`.

**Điều mình học được từ phần nhóm:**

- Ghi bottleneck là giả thuyết khi chưa đo là đúng, nhưng card chưa có số đo sẽ khó được chọn; lần sau nên bấm giờ ít nhất một lần làm thật trước khi pitch.
- Nhiều vấn đề có thể giải bằng sửa quy trình (poll lịch, một tài liệu góp ý chung) trước khi nghĩ đến AI.
- Khi phỏng vấn phải hỏi về lần gần nhất đã xảy ra, không hỏi "bạn có muốn…".

### NguyenThiHongHanh-2A202603537

**Phần việc phụ trách:**

- Chủ domain của candidate #7 (vận hành sàn thương mại điện tử).
- CP5 quy trình: bấm giờ baseline 5 buổi sáng, đếm lỗi sai kỳ/sai cột, cung cấp bộ dữ liệu ẩn danh; xác nhận quy trình hiện tại ở mục 4.1.
- Hỗ trợ CP4: kiểm tra báo cáo có sẵn của sàn, hỏi quy định công ty về dữ liệu, giới thiệu người làm báo cáo tương tự để phỏng vấn.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch 3 card: #7 chuyển báo cáo sàn sang mẫu công ty, #8 rà tiến độ campaign, #9 chốt đầu việc với Marketing và kho.
- Problem Card #7 là nền của candidate nhóm chọn: quy trình 5 bước, bottleneck giả thuyết ở bước ánh xạ và chuyển đổi, metric ghép thời gian với độ đúng của 3 kỳ, phương án Rule bằng bảng ánh xạ + Power Query, giả thuyết AI chỉ cho phần nhận định bằng lời.
- Sau phản biện của San, tách kế hoạch bấm giờ riêng cho bước tải, ánh xạ/chuyển đổi và kiểm tra.
- Phụ trách log bấm giờ `cp5-baseline-log.md`, nguồn số liệu cho các ô baseline ở mục 4, 5, 7.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (dòng #7–#9), mục 2.4 (candidate được chọn), mục 4.1, mục 6.4 (trích Problem Card của Hạnh).
- `report/assets/cp5-baseline-log.md`.
- Commit từ tài khoản `hanhshi96`.

**Điều mình học được từ phần nhóm:**

- Chỉ đo tốc độ có thể bỏ qua lỗi báo cáo, nên metric phải ghép thời gian với kiểm tra độ đúng của cả 3 kỳ.
- Một việc lặp lại mỗi ngày chưa chắc cần AI: phần ánh xạ và tổng hợp làm được bằng quy tắc, AI chỉ đáng xét ở phần Rule không làm được.
- Khi chỉ một người hiểu domain, phải đưa dữ liệu và cách làm ra thành tài liệu (log, bảng ánh xạ) để cả nhóm cùng làm được.

### HoangLamMinh-2A202603566

**Phần việc phụ trách:**

- CP4 research công cụ: Power Query, báo cáo có sẵn của sàn; bảng research có link ở mục 3.3.
- Tài liệu tham khảo (mục 10); hỗ trợ CP6 so sánh các mức No AI / Rule / Workflow / Agent.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch 3 card: #10 tổng hợp báo cáo định kỳ từ nhiều nguồn, #11 đối chiếu hóa đơn chứng từ, #12 nhiệm vụ sau cuộc họp; #12 được nhóm giữ làm phương án dự phòng thứ hai.
- Card #10 cùng card #7 tạo thành cluster A ("Chuẩn hóa và tổng hợp dữ liệu thành báo cáo").
- Đề xuất so sánh phương án không dùng AI (chuẩn hóa biểu mẫu Excel, Pivot Table, SUMIFS, Power Query) với phương án AI trước khi chọn mức can thiệp; hướng này được nhóm dùng ở mục 6.2.
- Tìm tài liệu Power Query trên Microsoft Learn làm nguồn cho mục 3.3 và 10.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (dòng #10–#12), mục 2.2 (cluster A), mục 3.3, mục 6.2, mục 10.
- Commit từ tài khoản `laminh-h`.

**Điều mình học được từ phần nhóm:**

- Problem phải là khó khăn của người dùng trong tình huống cụ thể, không phải tên một công cụ; các ý như "chatbot cho toàn doanh nghiệp" là giải pháp nên phải bỏ.
- Nên bắt đầu từ phương án đơn giản nhất (Excel, Power Query) và chỉ lên mức AI khi có lý do rõ ràng.
- Không dùng số liệu AI tự giả định làm dữ liệu thật; baseline phải đo hoặc ghi rõ là chưa đo.
