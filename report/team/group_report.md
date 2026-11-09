# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: NonTech
- Thành viên: xem `TEAM.md` (Nguyễn Thị Hồng San, Nguyễn Thị Thanh Thúy, Nguyễn Thị Hồng Hạnh, Hoàng Lam Minh)
- Candidate problem được chọn (1 câu): Mỗi buổi sáng, nhân viên vận hành sàn thương mại điện tử phải chuyển dữ liệu tải từ sàn sang đúng mẫu báo cáo công ty cho 3 kỳ (hôm qua, 7 ngày, 30 ngày) trước khi có số liệu dùng trong ngày, mất gần một tiếng mỗi sáng (theo phỏng vấn) và đã có lỗi lệch số khi sàn đổi thứ tự cột.
- Quyết định cuối: Go cho pilot Rule (10 buổi, 1 sàn); Not Yet cho bước AI

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Thị Hồng San | Chủ trọ: khi có nhiều phòng cho thuê, tôi muốn ghi số điện nước, tính tiền, gửi hóa đơn, nhắc tiền phòng và theo dõi báo hỏng ở một chỗ, để không phải nhắn từng người và không bỏ sót việc. Người thuê: tôi muốn hóa đơn ghi rõ số cũ, số mới và báo hỏng có người tiếp nhận, để không phải hỏi đi hỏi lại | Chủ trọ nhỏ (6–15 phòng) và người thuê; liên lạc qua Zalo | Thu tiền: tính tiền + soạn tin từng phòng ~50' (tổng ~135'/tháng, 2/3 tháng tính sai 1 phòng). Báo hỏng: không có danh sách việc, 2/6 lần bị quên, chờ sửa ~3 ngày | "Nếu dùng một app quản lý nhà trọ có sẵn thì còn vấn đề không?"; "Khách trả trễ vì không nhận được tin, hay vì chưa có tiền?" (người hỏi: …) |
| 2 | Nguyễn Thị Hồng San | Khi mỗi JD lại phải sửa CV và đoạn giới thiệu nhiều vòng, tôi muốn dán JD vào là có bản phù hợp, đúng độ dài và ngôn ngữ, để nộp nhanh mà vẫn đúng trọng tâm | Sinh viên năm 3 ứng tuyển 15–20 vị trí thực tập Data/BA mỗi mùa | Viết lại gạch đầu dòng theo từ khóa JD ~20' + đoạn giới thiệu ~15' (tổng ~75'/JD; 5/18 JD bỏ không nộp vì hết hạn) | |
| 3 | Nguyễn Thị Hồng San | Khi đang giảm cân, tôi muốn biết mỗi ngày ăn vào và tiêu hao bao nhiêu calo, và có thực đơn tuần theo mục tiêu, ngân sách, ăn ngoài hay tự nấu, để giảm đều mà không bỏ cuộc | Sinh viên giảm cân vừa phải, ăn ngoài 4–5 bữa/tuần, ngân sách ăn ~1,5 triệu/tháng | Tra calo món Việt ăn ngoài ~12'/ngày (tổng ~20'/ngày) + lên thực đơn ~40'/tuần; 2 lần bỏ ghi sau ~10 ngày | |
| 4 | Nguyễn Thị Thanh Thúy | Khi được giao tìm hiểu một chủ đề cho bài tập nhóm, tôi muốn sàng lọc được tài liệu liên quan và đáng tin cậy, để tập trung đọc các nguồn phù hợp | Thành viên được giao tìm tài liệu cho một phần bài tập nhóm | Bước 3–4: mở và sàng lọc từng nguồn theo mức liên quan, độ tin cậy (giả thuyết, chưa đo) | |
| 5 | Nguyễn Thị Thanh Thúy | Khi nhận góp ý cho bản nháp từ nhiều thành viên, tôi muốn gom và đối chiếu các góp ý, để biết điểm nào cần sửa, điểm nào trùng hoặc cần hỏi lại | Thành viên chịu trách nhiệm chỉnh sửa bản nháp | Bước 3–5: đọc, gom góp ý nằm ở nhiều nơi và làm rõ ý mâu thuẫn (giả thuyết, chưa đo) | "Lần gần nhất bạn nhận góp ý, có bao nhiêu góp ý và bao nhiêu cái thật sự mâu thuẫn nhau?" (San hỏi) |
| 6 | Nguyễn Thị Thanh Thúy | Khi nhóm cần tổ chức một buổi họp, tôi muốn biết khung giờ mọi người cùng tham gia được, để chốt lịch mà không phải nhắn qua lại nhiều lần | Thành viên điều phối lịch họp của nhóm | Bước 2–4: chờ phản hồi và đối chiếu lịch khi câu trả lời đến rải rác (giả thuyết, chưa đo) | |
| 7 | Nguyễn Thị Hồng Hạnh | Khi bắt đầu buổi sáng, tôi muốn chuyển dữ liệu tải từ sàn sang đúng mẫu báo cáo công ty cho 3 kỳ (hôm qua, 7 ngày, 30 ngày), để có số liệu dùng trong ngày | Nhân viên vận hành sàn thương mại điện tử phụ trách báo cáo định kỳ | Bước 3–4: ánh xạ và đưa dữ liệu nguồn vào đúng cột, đúng kỳ trong mẫu công ty (giả thuyết, cần bấm giờ) | "Sáng gần nhất bạn làm báo cáo, bước ánh xạ cột mất bao nhiêu phút so với bước tải và kiểm tra?" (San hỏi) — dẫn đến yêu cầu hỏi riêng thời gian từng bước khi phỏng vấn (mục 3.2) |
| 8 | Nguyễn Thị Hồng Hạnh | Khi rà các campaign trong tháng, tôi muốn biết campaign nào đúng tiến độ, đang chờ, mốc nào cần xử lý trước, để ưu tiên việc trong ngày | Nhân viên vận hành sàn theo dõi campaign tháng | Bước 3–4: đối chiếu cập nhật gần nhất và xác định việc đang chờ hoặc có nguy cơ trễ (giả thuyết) | |
| 9 | Nguyễn Thị Hồng Hạnh | Khi campaign có việc cần Marketing hoặc kho xác nhận, tôi muốn chốt rõ yêu cầu, người phụ trách và hạn phản hồi, để biết phần nào đã sẵn sàng triển khai | Nhân viên vận hành sàn điều phối với Marketing và kho | Bước 2–4: gửi yêu cầu, theo dõi phản hồi, ghi nhận xác nhận (phản hồi kho 1–3 ngày; cần tách thời gian xử lý và thời gian chờ) | |
| 10 | Hoàng Lam Minh | Khi đến cuối tuần/cuối tháng, tôi muốn tổng hợp nhanh và chính xác kết quả công việc từ nhiều nguồn, để hoàn thành báo cáo đúng hạn cho quản lý | Nhân viên văn phòng phụ trách tổng hợp báo cáo; quản lý là người dùng báo cáo | Bước 2–3: tìm kiếm, đối chiếu và kiểm tra dữ liệu từ Excel, email, tài liệu (chưa đo, cần bấm giờ) | |
| 11 | Hoàng Lam Minh | Khi tiếp nhận hóa đơn và chứng từ thanh toán, tôi muốn kiểm tra và đối chiếu chính xác thông tin, để hạn chế sai sót khi thanh toán và lưu trữ | Nhân viên kế toán, hành chính hoặc mua hàng | Bước 3–4: kiểm tra ngày, số tiền và đối chiếu với đơn hàng/hợp đồng (cần đo thời gian mỗi chứng từ) | |
| 12 | Hoàng Lam Minh | Khi kết thúc cuộc họp có nhiều nhiệm vụ được giao, tôi muốn xác định rõ công việc, người phụ trách và deadline, để mọi người phối hợp đúng tiến độ | Nhân viên ghi biên bản, thành viên dự họp, trưởng nhóm | Bước 2–4: chuyển nội dung trao đổi thành nhiệm vụ có người phụ trách và deadline (cần đo thời gian hoàn thiện biên bản, số lần hỏi lại) | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Chuẩn hóa và tổng hợp dữ liệu thành báo cáo | #3 (ghi calo và lên thực đơn từ nhiều nguồn), #7 (chuyển báo cáo sàn sang mẫu công ty), #10 (tổng hợp báo cáo định kỳ nhiều nguồn) | Dữ liệu đến từ nhiều nguồn hoặc nhiều định dạng, phải tra cứu, chuyển đổi, gộp thủ công trước khi ra được một bản tổng hợp; việc lặp lại theo ngày/tuần/kỳ và đo được bằng số phút |
| B — Giao việc, xác nhận và theo dõi phản hồi | #1 (thu tiền phòng và tiếp nhận báo hỏng giữa chủ trọ và người thuê), #6 (chốt lịch họp nhóm), #8 (rà tiến độ campaign), #9 (chốt đầu việc với Marketing và kho), #12 (nhiệm vụ sau cuộc họp) | Việc cần gửi yêu cầu cho nhiều người rồi chờ phản hồi hoặc xác nhận; thời gian mất chủ yếu ở soạn từng tin, chờ đợi và hỏi lại vì chưa rõ ai làm, hạn khi nào, trạng thái đến đâu; thông tin trạng thái nằm rải trong tin nhắn nên dễ bị quên |
| C — Sàng lọc và đối chiếu thông tin theo tiêu chí | #2 (đối chiếu CV với yêu cầu từng JD), #4 (sàng lọc tài liệu), #5 (gom và đối chiếu góp ý bản nháp), #11 (đối chiếu hóa đơn, chứng từ) | Phải mở, đọc từng mục (JD, nguồn, góp ý, chứng từ) để kiểm tra theo một bộ tiêu chí; tiêu chí thường chưa được viết ra từ đầu nên mỗi lần làm lại một kiểu |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian làm thủ công và số lần sai sót, bỏ sót ở các việc lặp lại
         mà thành viên nhóm đang làm (đo bằng phút/lần và số lỗi/kỳ)
├── Opportunity A: Dữ liệu nằm ở nhiều nguồn, khác định dạng, phải tra cứu và gộp tay
│                  mới ra được một bản tổng hợp dùng được
│   ├── Báo cáo sàn phải ánh xạ cột sang mẫu công ty cho 3 kỳ mỗi sáng (#7)
│   ├── Báo cáo tuần/tháng phải tìm và đối chiếu từ Excel, email, tài liệu (#10)
│   └── Món Việt ăn ngoài không có sẵn số calo, phải tra từng món mỗi ngày (#3)
├── Opportunity B: Gửi yêu cầu cho nhiều người rồi không biết ai đã phản hồi,
│                  trạng thái đến đâu, nên phải soạn từng tin và hỏi lại nhiều lần
│   ├── Chủ trọ soạn hóa đơn từng phòng, người thuê không hiểu cách tính nên hỏi lại;
│   │   báo hỏng nằm lẫn trong Zalo nên bị quên (#1)
│   ├── Chốt lịch họp phải nhắn qua lại, câu trả lời đến rải rác (#6)
│   ├── Việc cần Marketing/kho xác nhận không rõ đã sẵn sàng chưa (#8, #9)
│   └── Nhiệm vụ sau họp không rõ người phụ trách và deadline (#12)
└── Opportunity C: Phải đọc từng mục để kiểm tra theo tiêu chí chưa được viết ra,
                   nên mỗi lần làm lại một kiểu và dễ sót
    ├── Mỗi JD có yêu cầu khác, phải chọn và viết lại kinh nghiệm cho khớp (#2)
    ├── Tài liệu và góp ý bản nháp phải lọc theo mức liên quan, mâu thuẫn (#4, #5)
    └── Hóa đơn, chứng từ phải đối chiếu ngày, số tiền với đơn hàng (#11)
```

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #2 Sửa CV và đoạn giới thiệu theo từng JD (cụm C) | 5 | 5 | 4 | 4 | 5 | 4 | 5 | **32** |
| #1 Quản lý phòng trọ: hóa đơn điện nước minh bạch + tiếp nhận báo hỏng (cụm B) | 5 | 5 | 5 | 4 | 4 | 5 | 2 | **30** |
| #12 Nhiệm vụ sau cuộc họp (cụm B) | 4 | 4 | 2 | 3 | 5 | 5 | 5 | **28** |
| #7 Chuyển báo cáo sàn sang mẫu công ty (cụm A) | 5 | 5 | 3 | 4 | 3 | 4 | 2 | **26** |

*Cách chấm:* 5 = có số liệu đo thật hoặc rất rõ; 3 = có mô tả nhưng còn là giả thuyết, chưa bấm giờ; 1 = chưa có. Mỗi cụm đưa 1–2 card mạnh nhất vào shortlist. "Nhóm hiểu domain" chấm theo số thành viên trực tiếp làm việc đó (1 người = 2 điểm, cả nhóm = 5 điểm).

*Ghi chú về #7:* "Quy trình rõ" = 5 vì đầu vào (file tải từ sàn) và đầu ra (mẫu báo cáo công ty) cố định, kiểm tra được từng ô. "Impact đo được" = 4 vì việc lặp mỗi buổi sáng (khoảng 20–22 lần/tháng) và đo được bằng phút/buổi và số ô sai kỳ, sai cột, dù baseline chưa bấm giờ. "Vừa sức lab" = 3 vì là dữ liệu nội bộ, phải ẩn danh trước khi đưa vào lab.

**Candidate được chọn:** #7 — Mỗi buổi sáng, nhân viên vận hành sàn thương mại điện tử phải chuyển dữ liệu tải từ sàn sang đúng mẫu báo cáo công ty cho 3 kỳ (hôm qua, 7 ngày, 30 ngày) trước khi có số liệu dùng trong ngày.

**Vì sao chọn (dù tổng điểm không cao nhất):**

Bảng chấm điểm cho thấy #7 đứng sau #2, #1 và #12, chủ yếu vì chưa bấm giờ và chỉ một thành viên hiểu domain. Nhóm vẫn chọn #7 vì các lý do nằm ngoài 7 cột chấm:

- **Tần suất cao nhất trong shortlist:** lặp mỗi buổi sáng (khoảng 20–22 lần/tháng), so với 1 lần/tháng của #1 và theo mùa tuyển dụng của #2. Chỉ cần tiết kiệm vài phút mỗi buổi, tổng thời gian tiết kiệm trong tháng đã đáng kể. Baseline sẽ được đo ở CP4 để kiểm tra nhận định này.
- **Bối cảnh công việc thật, có người dùng kết quả:** báo cáo được dùng ngay trong ngày, nên kết quả lab có thể áp dụng tiếp sau buổi học, và sai sót (sai kỳ, sai cột) có hậu quả kiểm chứng được.
- **Giải pháp có sẵn chưa phủ được bài toán:** mẫu báo cáo là mẫu riêng của công ty, nên công cụ chung (báo cáo có sẵn của sàn, chatbot) không xuất đúng mẫu. Ngược lại, #2 có rủi ro cao là chatbot có sẵn đã giải phần lớn vấn đề.
- **Phép so sánh các mức can thiệp rõ ràng:** bước ánh xạ cột và chọn kỳ có thể chỉ cần **Rule** (bảng ánh xạ + Power Query). AI chỉ được cân nhắc nếu báo cáo có phần nhận định bằng lời. Nhóm chấp nhận khả năng kết luận cuối là Rule / No AI nếu bằng chứng cho thấy như vậy.

**Điều kiện để giữ #7 (kiểm chứng ở CP4):**

- Phỏng vấn Hạnh về buổi sáng gần nhất làm báo cáo: thời gian từng bước (tải, ánh xạ/chuyển đổi, kiểm tra) và lần gần nhất bị sai kỳ hoặc sai cột.
- Phỏng vấn thêm một đồng nghiệp cũ của Hạnh từng làm báo cáo sàn, cùng bộ câu hỏi, để có góc nhìn ngoài Hạnh.
- Dữ liệu đưa vào lab phải được ẩn danh (bỏ tên shop, thay doanh thu thật bằng số mẫu).
- **Ngưỡng đổi đề tài:** nếu theo phỏng vấn, bước ánh xạ và chuyển đổi chiếm dưới 10 phút/buổi và cả hai người đều không nhớ lần nào bị sai kỳ, sai cột, nhóm chuyển sang phương án dự phòng.

*Kết quả CP4 (mục 3.2): đạt điều kiện — bước ghép + điền khoảng 25–30 phút/sáng và đã có lỗi lệch số tuần trước, nên nhóm giữ #7.*

**Vì sao loại các candidate còn lại:**

- **#2 Sửa CV theo JD:** điểm cao nhất và có số đo thật (khoảng 75 phút/JD, 18 JD, 5 JD bỏ không nộp), nhưng chatbot có sẵn đã làm được phần lớn việc viết lại theo JD; phần còn lại (không bịa kinh nghiệm, giữ thư viện gạch đầu dòng) nhỏ. Chưa có bằng chứng nhà tuyển dụng đánh giá cao CV được sửa theo JD, và số liệu mới đến từ một người.
- **#1 Phòng trọ:** có baseline bấm giờ và phỏng vấn hai phía, nhưng việc chỉ diễn ra 1 lần/tháng (khoảng 135 phút), chỉ một thành viên hiểu domain, và phạm vi gồm hai luồng (thu tiền, báo hỏng) khá rộng cho một buổi lab. Giữ làm **phương án dự phòng thứ nhất** vì đã có sẵn bằng chứng.
- **#12 Nhiệm vụ sau cuộc họp:** cả nhóm hiểu domain nhưng pain chỉ là mô tả chung, chưa có lần nào được đo (thời gian hoàn thiện biên bản, số lần hỏi lại). Giữ làm **phương án dự phòng thứ hai**.
- **Các card còn lại của cụm C (#4, #5, #11):** tiêu chí sàng lọc chưa được viết ra và chưa có baseline; nên viết tiêu chí trước rồi mới đánh giá lại.

**Xử lý bất đồng (nếu có):**

- Bất đồng 1: có ý kiến cho rằng nên chọn card có điểm cao nhất (#2) hoặc card đã có số đo và phỏng vấn (#1), vì #7 chưa bấm giờ. Nhóm thống nhất vẫn chọn #7 vì tần suất hằng ngày và tính ứng dụng trong công việc thật, nhưng đặt điều kiện phỏng vấn kiểm chứng và ngưỡng đổi đề tài ở trên; nếu không đạt thì chuyển sang #1.
- Bất đồng 2: chỉ Hạnh hiểu domain sàn và có dữ liệu. Nhóm thống nhất Hạnh cung cấp baseline (qua phỏng vấn) và bộ dữ liệu ẩn danh, đồng thời giới thiệu một đồng nghiệp cũ để có góc nhìn thứ hai; các thành viên khác phụ trách phỏng vấn, research công cụ (Power Query, báo cáo có sẵn của sàn), vẽ quy trình và viết Problem Statement, để không phụ thuộc vào một người.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Bước 3–4 (ánh xạ cột, điền chỉ số) chiếm phần lớn thời gian làm báo cáo mỗi sáng, lớn hơn bước tải file | Value | 5 | 2 | **Có** — phỏng vấn Hạnh và đồng nghiệp cũ (thời gian từng bước sáng gần nhất) |
| 2 | Lỗi sai kỳ / sai cột thật sự xảy ra và phải sửa lại báo cáo | Value | 4 | 1 | **Có** — phỏng vấn: lần gần nhất bị sai, ai phát hiện, sửa mất bao lâu |
| 3 | File xuất từ sàn giữ nguyên tên và thứ tự cột qua các ngày | Feasibility | 5 | 1 | **Có** — phỏng vấn: lần gần nhất sàn đổi tên/thứ tự cột |
| 4 | Người làm báo cáo sàn khác (ngoài Hạnh) cũng gặp vấn đề tương tự | Value | 3 | 1 | **Có** — phỏng vấn đồng nghiệp cũ của Hạnh |
| 5 | Báo cáo có phần nhận định bằng lời và phần này tốn thời gian | Value (cho bước AI) | 3 | 2 | Sau — chỉ quyết định có bước AI hay không |
| 6 | Công ty cho phép đưa dữ liệu bán hàng đã ẩn danh vào công cụ AI bên ngoài | Viability | 3 | 1 | Sau — chỉ cần nếu giả định 5 đúng |

*"Đã có bằng chứng" = 2 khi mới có mô tả trong Problem Card của Hạnh; = 1 khi chưa có gì.*

Giả định nhóm kiểm chứng trong buổi này: **giả định 1 và 3** — quan trọng nhất và ít bằng chứng nhất. Nếu giả định 1 sai, bottleneck nằm chỗ khác và cả hướng giải pháp phải đổi; nếu giả định 3 sai, phần Rule sẽ lỗi thường xuyên.

**Kết quả sau phỏng vấn (mục 3.2):** giả định 1 **đúng một phần** — ghép + điền là khâu lâu nhất của Hạnh (25–30 phút) nhưng đồng nghiệp cũ cho rằng kiểm tra mới lâu nhất (15–20 phút). Giả định 2 **đúng**, nhưng lỗi không chỉ là sai cột mà còn là đơn hủy lẫn trong file. Giả định 3 **sai** — sàn đã đổi thứ tự cột tuần trước. Giả định 4 **đúng** — đồng nghiệp cũ cũng mất gần một tiếng mỗi sáng. Giả định 5, 6 chưa kiểm chứng.

### 3.2. Kiểm chứng

Cách đã dùng: **Phỏng vấn** — 2 người, ngày 09/11/2026, hỏi về buổi sáng gần nhất và lần gần nhất gặp lỗi (bộ câu hỏi và ghi chép đầy đủ: [cp4-interview-snapshot-1.md](../assets/cp4-interview-snapshot-1.md)).

Interview snapshot:

| Trường | #1 — Hạnh (trực tiếp) | #2 — Đồng nghiệp cũ của Hạnh (online) |
|---|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Nhân viên vận hành sàn TMĐT, làm báo cáo buổi sáng, tải dữ liệu từ 2 sàn | Nhân viên vận hành sàn TMĐT, trước đây phụ trách báo cáo |
| Câu nói đáng nhớ nhất (nguyên văn) | "Sáng nào cũng phải tải file về rồi ghép lại, nói chung cũng mất kha khá thời gian. Hôm nào file bị đổi cột là lại phải ngồi sửa từ đầu." | "Thực ra nhập số liệu không lâu lắm, mất thời gian nhất là kiểm tra xem số liệu đã đúng chưa. Nhiều lúc làm xong vẫn phải mở từng file ra đối chiếu lại." |
| Lần gần nhất gặp vấn đề này | Tuần trước, một sàn đổi thứ tự cột; copy vào mẫu như cũ nên lệch số liệu, đến bước kiểm tra mới phát hiện, phải sửa lại | Báo cáo doanh thu bị cao bất thường vì đơn hủy vẫn nằm trong file tải về; phải lọc lại, tính lại, sửa báo cáo |
| Workaround hiện tại | File Excel mẫu cố định, một số ô có công thức sẵn; lọc thông tin cần rồi copy sang; vẫn tự kiểm tra | File mẫu có công thức; lọc đơn cần thiết; mở báo cáo hôm trước ra so để tìm số bất thường |
| Mất bao lâu | Kỳ 5' · tải 10–15' · ghép cột 15–20' · điền mẫu 10' · kiểm tra 10–15' → gần 1 tiếng; hôm ít dữ liệu ~30' | Tải 10' · lọc + ghép 15–20' · nhập mẫu 10' · kiểm tra 15–20' → gần 1 tiếng, hôm dữ liệu có vấn đề thì lâu hơn |
| Insight | Ánh xạ phải theo **tên** cột, không theo vị trí, và phải phát hiện khi cột thay đổi | Kiểm tra gần ngang ghép dữ liệu; cần lọc đơn hủy/hoàn theo trạng thái và so với hôm trước để đánh dấu số bất thường |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn Hạnh | 1 | Làm mỗi sáng, gần 1 tiếng; ghép + điền 25–30' là khâu lâu nhất; lỗi lệch số khi sàn đổi thứ tự cột (tuần trước) | Có file mẫu và công thức nên ngày bình thường "không quá vất vả"; không phải ngày nào cũng lỗi; hôm ít dữ liệu ~30' |
| Phỏng vấn đồng nghiệp cũ | 1 | Cũng làm bằng Excel, gần 1 tiếng; sai số liệu phải làm lại báo cáo | Nhập số "không lâu lắm" — **bước kiểm tra (15–20') mới lâu nhất**, trái giả thuyết bottleneck chỉ ở bước 3–4; quen tay thì làm khá nhanh; lỗi đến từ dữ liệu (đơn hủy) chứ không phải cột |
| Câu hỏi 7 (phần nhận xét bằng lời) | 0 | — | Chưa hỏi được → chưa có căn cứ cho bước AI |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

1. **Bottleneck mở rộng:** từ "bước 3–4" thành "bước 3–4 (ghép + điền, 25–30') **và** bước 5 kiểm tra (10–20')". Kiểm tra lâu vì phải tự mở từng file đối chiếu — nên quy trình tương lai phải giảm cả việc kiểm tra tay, không chỉ ghép cột.
2. **Thêm nguồn lỗi:** ngoài sai kỳ/sai cột, có lỗi **dữ liệu** (đơn hủy/hoàn vẫn trong file). Rule thêm bước lọc theo trạng thái đơn và so với báo cáo hôm trước để đánh dấu số bất thường.
3. **Sửa thiết kế ánh xạ:** giả định "cột ổn định" sai → bảng ánh xạ phải khớp theo **tên** cột và dừng khi có cột lạ/thiếu, không copy theo vị trí.
4. **Phạm vi:** Hạnh tải từ **2 sàn**, không phải 1; pilot vẫn bắt đầu với 1 sàn, sàn thứ hai thêm sau.
5. **Có baseline (tự ước lượng):** khoảng 50–65 phút/sáng, lấy **B ≈ 60 phút** ("gần một tiếng"); số này cần được xác nhận bằng bấm giờ ở pilot.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Power Query — gộp file trong thư mục (Combine files) | [learn.microsoft.com/…/combine-files-overview](https://learn.microsoft.com/en-us/power-query/combine-files-overview) | Bước 3–4: gộp các file cùng cấu trúc trong một thư mục thành một bảng | Không cần viết code; các bước được lưu lại, lần sau chỉ cần làm mới | Tài liệu ghi rõ chỉ gộp tốt khi các file **cùng loại và cùng cột**; khi tên cột hoặc kiểu dữ liệu đổi, bước đổi kiểu có thể báo lỗi | Giả định 3 (cột ổn định) đã sai — sàn từng đổi thứ tự cột → khớp cột theo tên và thiết kế "dừng và báo lỗi" thay vì để truy vấn chạy sai |
| Power Query — tổng quan | [learn.microsoft.com/…/power-query-what-is-power-query](https://learn.microsoft.com/en-us/power-query/power-query-what-is-power-query) | Bước 1, 3, 4: lấy dữ liệu, đổi hình dạng, lưu thành truy vấn lặp lại được | Có sẵn trong Excel cho Windows và Mac; biến việc làm tay một lần thành quy trình làm mới được | Cần người biết dùng để dựng và sửa truy vấn; nhóm chưa xác nhận ai đã dùng Power Query | Phần số liệu giải được bằng **Rule** có sẵn, không cần AI; cần phân công người học Power Query |
| Pattern: chọn mức đơn giản nhất (Anthropic — Building effective agents) | [anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents) | Không giải bước cụ thể; là nguyên tắc chọn mức can thiệp | Phân biệt rõ Workflow (bước định sẵn) và Agent (AI tự quyết bước); khuyên bắt đầu từ giải pháp đơn giản nhất | Là hướng dẫn chung, không phải công cụ | Bài có các bước định sẵn → loại Agent; chỉ thêm AI ở bước Rule không làm được (mục 6) |

*Chưa research: báo cáo có sẵn trong trang quản lý của sàn (có xuất đúng 3 kỳ không, có tùy chỉnh cột không) — cần Hạnh kiểm tra trên tài khoản thật vì đây là công cụ cạnh tranh trực tiếp với phương án Rule.*

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Phạm vi: báo cáo vận hành buổi sáng theo mẫu công ty, 3 kỳ (hôm qua, 7 ngày, 30 ngày); Hạnh hiện tải từ 2 sàn. Tần suất: mỗi sáng ngày làm việc. Thời gian từng bước lấy từ phỏng vấn Hạnh ngày 09/11/2026 ([cp4-interview-snapshot-1.md](../assets/cp4-interview-snapshot-1.md)), là số tự ước lượng, chưa bấm giờ.

Sơ đồ:

```text
QUY TRÌNH HIỆN TẠI — mỗi sáng, 1 nhân viên vận hành, tổng khoảng 50–65 phút, "gần một tiếng" (theo phỏng vấn)

[1 Xác định kỳ: ngày bắt đầu/kết thúc của 3 kỳ: ~5']
        │
        ▼
[2 Tải dữ liệu từ sàn cho 3 kỳ (3 file): 10–15']
        │
        ▼
[3 Đối chiếu trường nguồn với cột mẫu công ty: 15–20']   ← BOTTLENECK
        │
        ▼
[4 Copy, chuyển đổi, điền chỉ số vào mẫu cho 3 kỳ: ~10']        ← BOTTLENECK
        │
        ▼
[5 Kiểm tra kỳ và số liệu so với nguồn: 10–15']   ← bottleneck phụ (đồng nghiệp cũ: 15–20')
        │
   Có sai? ──Có──► quay lại bước 3–4 sửa (lần gần nhất: tuần trước, sàn đổi thứ tự cột)
        │
       Không
        ▼
[Báo cáo hoàn tất, dùng trong ngày]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Nhân viên vận hành | Ngày hiện tại, quy tắc tính kỳ (hiện chưa viết ra) | Khoảng ngày của 3 kỳ: hôm qua, 7 ngày, 30 ngày | ~5 phút / mỗi sáng | Rủi ro chọn lệch ngày, hoặc lấy số khi sàn chưa chốt |
| 2 | Nhân viên vận hành | Tài khoản trang quản lý của sàn, 3 khoảng ngày | 3 file xuất (Excel/CSV) | 10–15 phút / mỗi sáng | Phụ thuộc tốc độ xuất file của sàn; Hạnh tải từ 2 sàn |
| 3 | Nhân viên vận hành | 3 file nguồn, mẫu báo cáo công ty | Biết cột nguồn nào ứng với cột nào trong mẫu (ánh xạ nằm trong đầu người làm) | 15–20 phút / mỗi sáng | Copy theo vị trí cột; khi sàn đổi thứ tự cột thì lệch số (tuần trước) |
| 4 | Nhân viên vận hành | 3 file nguồn, ánh xạ ở bước 3 | Mẫu báo cáo đã điền chỉ số cho 3 kỳ | ~10 phút / mỗi sáng | Một số ô có công thức sẵn; phần còn lại copy tay; phải tự lọc đơn cần thiết |
| 5 | Nhân viên vận hành | Báo cáo đã điền, file nguồn | Báo cáo đã kiểm tra, hoặc danh sách ô cần sửa | 10–15 phút / mỗi sáng (đồng nghiệp cũ: 15–20); lần gần nhất bị sai: tuần trước | Mở từng file và báo cáo hôm trước để đối chiếu; nếu sai thì quay lại bước 3–4 |

**Bottleneck chính:** bước 3–4 (ghép cột + điền mẫu, khoảng 25–30 phút, gần một nửa thời gian) — làm tay, copy theo vị trí cột nên lệch số khi sàn đổi thứ tự cột. **Bottleneck phụ:** bước 5 kiểm tra (10–20 phút), vì phải tự mở từng file và báo cáo hôm trước để đối chiếu; đồng nghiệp cũ cho rằng đây mới là bước lâu nhất. Bước 2 (tải file, 10–15 phút) không phải bottleneck chính, nên ngưỡng đổi đề tài ở mục 2.4 chưa bị chạm.

### 4.2. Quy trình tương lai

```text
QUY TRÌNH TƯƠNG LAI — mỗi sáng

[1 RULE   Công thức tính sẵn 3 kỳ theo quy tắc đã chốt (hôm qua = TODAY()-1, ...)]
        │
        ▼
[2 NGƯỜI  Tải 3 file từ sàn, lưu vào thư mục cố định, đặt tên theo kỳ]
        │
        ▼
[3 RULE   Power Query đọc thư mục + BẢNG ÁNH XẠ cột nguồn → cột mẫu công ty]
        │
   Thiếu cột / sàn đổi tên cột / file sai kỳ?
        ├──Có──► DỪNG, báo lỗi rõ cột nào → PHƯƠNG ÁN QUAY VỀ A
        │
       Không
        ▼
[4 RULE   Lọc đơn hủy/hoàn + tự điền chỉ số 3 kỳ vào mẫu
          + đối chiếu tổng với file nguồn và với báo cáo hôm trước, đánh dấu số bất thường]
        │
        ▼
[5 NGƯỜI  Kiểm tra các ô bị đánh dấu chênh lệch, DUYỆT báo cáo]   ← HITL bắt buộc
        │
        ▼
[6 AI (tùy chọn) Soạn nháp 3–5 câu nhận định từ số ĐÃ DUYỆT]       ← chỉ làm nếu xác nhận được
        │                                                            báo cáo có phần nhận định bằng lời
        ▼
[7 NGƯỜI  Sửa/duyệt nhận định → báo cáo hoàn tất]
        │
   Nhận định sai số hoặc suy diễn sai? → PHƯƠNG ÁN QUAY VỀ B
```

| Bước | Loại | Ai làm | Ghi chú |
|---:|---|---|---|
| 1 | **Rule** | Công thức trong file mẫu | Quy tắc tính kỳ và giờ chốt số được viết ra một lần, người làm và người nhận báo cáo cùng thống nhất |
| 2 | **Con người** | Nhân viên vận hành | Giữ thủ công vì chưa xác định sàn có cho xuất tự động hay không; chỉ chuẩn hóa nơi lưu và tên file |
| 3 | **Rule** | Power Query + bảng ánh xạ | Bảng ánh xạ là một sheet riêng, khớp theo **tên** cột (không theo vị trí, vì sàn từng đổi thứ tự cột); không đoán cột khi không khớp |
| 4 | **Rule** | Power Query / công thức | Lọc đơn hủy/hoàn theo trạng thái; tự đối chiếu tổng với file nguồn và với báo cáo hôm trước, đánh dấu chênh lệch bất thường — thay phần kiểm tra tay ở bước 5 |
| 5 | **Con người (HITL)** | Nhân viên vận hành | Không có báo cáo nào được dùng khi chưa có người duyệt |
| 6 | **AI (tùy chọn)** | Mô hình ngôn ngữ, chỉ đọc bảng số đã duyệt | Chỉ có nếu báo cáo thật sự cần phần nhận định bằng lời |
| 7 | **Con người** | Nhân viên vận hành | Duyệt từng câu nhận định trước khi dùng |

**Boundary:**

- Ánh xạ cột, tính kỳ, tính chỉ số **chỉ dùng Rule**; AI không được ánh xạ cột, không được tính hay sửa bất kỳ con số nào.
- AI (nếu dùng) chỉ đọc bảng số **đã được người duyệt**, chỉ được nhắc các con số có trong bảng, không suy đoán nguyên nhân khi không có dữ liệu, và không tự gửi báo cáo cho ai.
- Dữ liệu đưa vào AI phải ẩn danh (không tên shop, không thông tin khách hàng); không đưa file nguồn gốc của sàn vào AI.
- Khi Power Query gặp cột lạ hoặc thiếu cột thì phải **dừng và báo lỗi**, không tự đoán ánh xạ.

**Phương án quay về:**

- **A — Rule lỗi** (sàn đổi định dạng file, thiếu cột, đối chiếu tổng không khớp): làm tay bước 3–4 như hiện tại nhưng theo bảng ánh xạ đã viết ra (in sẵn làm checklist); sau đó cập nhật bảng ánh xạ để hôm sau chạy lại được.
- **B — AI nhận định sai** (nhắc số không có trong bảng, sai xu hướng, suy diễn nguyên nhân): bỏ phần nhận định của AI hôm đó, người tự viết hoặc gửi báo cáo chỉ có số. Nếu trong 2 tuần có từ 2 lần AI nhắc sai số, bỏ hẳn bước 6.

### 4.3. Before / after

Gọi **B** = tổng thời gian làm báo cáo mỗi sáng theo phỏng vấn Hạnh: khoảng 50–65 phút, lấy **B ≈ 60 phút** ([cp4-interview-snapshot-1.md](../assets/cp4-interview-snapshot-1.md)).

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 (+ vòng sửa lại khi sai) | 5 (không có bước 6–7) / 7 (có bước AI) | Số bước gần như giữ nguyên; thay đổi nằm ở việc ai/cái gì làm từng bước |
| Tổng thời gian | B ≈ 60 phút/buổi (tự ước lượng) | ≤ 42 phút (0,7 × B) | Mục tiêu theo Problem Card của Hạnh; bấm giờ 5 buổi sau khi áp dụng |
| Số bước thủ công | 5 / 5 | 2 (tải file, duyệt) — thêm 1 nếu có bước duyệt nhận định AI | Bước 3–4 chuyển sang Rule |
| Lỗi số liệu (sai cột, đơn hủy lẫn vào) | Lần gần nhất: tuần trước (sàn đổi thứ tự cột) | 0 lỗi lọt qua bước duyệt | Rule khớp cột theo tên, lọc đơn hủy, đối chiếu tổng |
| Bottleneck chính | Bước 3–4: ghép + điền bằng tay (25–30'); phụ: kiểm tra tay (10–20') | Bước 2: tải file từ sàn (10–15', thời gian chờ) | Bottleneck dịch sang phần nhóm chưa can thiệp |
| Rủi ro mới phát sinh | — | Sàn đổi tên/thứ tự cột làm Power Query lỗi; người tin số tự động nên kiểm tra qua loa; lưu nhầm file kỳ vào thư mục; AI (nếu dùng) nhắc sai số hoặc suy diễn | Xử lý bằng: dừng khi lỗi cột, đối chiếu tổng tự động, duyệt bắt buộc, phương án quay về A/B |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhân viên vận hành sàn thương mại điện tử phụ trách báo cáo định kỳ buổi sáng; người dùng báo cáo là quản lý / team vận hành trong ngày |
| **Quy trình** | Mỗi sáng ngày làm việc: (1) xác định 3 kỳ (hôm qua, 7 ngày, 30 ngày) → (2) tải 3 file từ sàn → (3) đối chiếu cột nguồn với cột mẫu công ty → (4) copy, chuyển đổi, điền chỉ số vào mẫu → (5) kiểm tra kỳ và số liệu, sai thì quay lại bước 3–4 (chi tiết ở mục 4.1) |
| **Bottleneck** | Bước 3–4, ghép cột và điền chỉ số cho 3 kỳ bằng tay (khoảng 25–30 phút/sáng), copy theo vị trí cột nên lệch số khi sàn đổi thứ tự cột; bước 5 kiểm tra tay (10–20 phút) là bottleneck phụ (phỏng vấn, mục 3.2) |
| **Impact** | Việc lặp lại khoảng 20–22 buổi sáng/tháng, tức khoảng 20–22 giờ/tháng (B ≈ 60 phút), trong đó ghép + điền khoảng 9–10 giờ; khi số liệu sai phải sửa lại báo cáo (lần gần nhất: tuần trước, do sàn đổi thứ tự cột) |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian mỗi sáng: B ≈ 60 phút (tự ước lượng qua phỏng vấn) → ≤ 42 phút; đo bằng bấm giờ 5 buổi sau khi áp dụng. (2) Số lần lỗi sai kỳ / sai cột lọt qua bước kiểm tra: baseline ít nhất 1 lần trong tuần gần nhất (theo phỏng vấn) → 0; đo bằng đối chiếu tổng đơn và doanh thu của từng kỳ với file nguồn. (3) Tỷ lệ chỉ số bắt buộc của cả 3 kỳ khớp nguồn theo định nghĩa đã thống nhất: → 100% |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Không dùng AI để ánh xạ cột, tính kỳ hay tính chỉ số; không đưa dữ liệu chưa ẩn danh (tên shop, thông tin khách hàng) ra ngoài công ty; khi gặp cột lạ hoặc thiếu cột thì dừng và báo lỗi, không đoán. HITL: nhân viên vận hành duyệt mọi báo cáo trước khi dùng, nhất là các ô bị đánh dấu chênh lệch so với nguồn |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

*(Phản biện dưới đây do AI (Claude) đưa ra khi rà v0; cột phản hồi là đề xuất, nhóm xác nhận hoặc sửa theo thảo luận thật.)*

- **"Bottleneck và Impact đều chưa có số, Problem Statement đang dựa trên giả thuyết."** → Đồng ý. Không điền số ước đoán; dùng số từ phỏng vấn Hạnh (ghi rõ là tự ước lượng) làm baseline và giữ ngưỡng đổi đề tài ở mục 2.4. Sau phỏng vấn, baseline là khoảng 60 phút/sáng.
- **"Metric chỉ đo tốc độ có thể làm nhóm bỏ qua chất lượng: báo cáo nhanh hơn nhưng sai kỳ thì vô ích."** → Đồng ý. Đã thêm metric (2) và (3) về số ô sai và tỷ lệ chỉ số khớp nguồn.
- **"Bài này nghe như chỉ cần Power Query, AI ở đâu?"** → Đồng ý một phần. Phần chính (ánh xạ, tính kỳ) là Rule; AI chỉ được xét cho phần nhận định bằng lời nếu báo cáo thật sự có phần này (xem mục 6).
- **"Định nghĩa '7 ngày' là 7 ngày tính cả hôm nay hay không, và lấy số khi sàn đã chốt hay chưa?"** → Đồng ý. Chưa có quy tắc viết ra; cần chốt với người nhận báo cáo trước khi viết công thức ở bước 1.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ thấp × Độ phức tạp cao** (phần chính: ánh xạ và tính chỉ số). Riêng phần nhận định bằng lời (nếu có) nằm ở ô **Độ mơ hồ cao × Độ phức tạp thấp**.

Vì sao:

- **Độ mơ hồ thấp:** mỗi ô trong mẫu báo cáo có một đáp án đúng duy nhất, kiểm tra được bằng cách so với file nguồn. Cùng một file đầu vào thì phải ra cùng một báo cáo.
- **Độ phức tạp cao (theo định nghĩa của worksheet):** 3 nguồn dữ liệu (3 file theo kỳ, nhân với 2 sàn), 5 bước nối tiếp, bước sau phụ thuộc bước trước (sai kỳ ở bước 1 thì mọi số sau đều sai). Nhưng mọi bước đều xác định được trước, nên chỉ cần một chuỗi Rule cố định, không cần AI quyết định bước nào.
- **Phần nhận định bằng lời:** nhiều cách viết đều chấp nhận được (mơ hồ cao) nhưng chỉ là một bước, đầu vào là bảng số đã duyệt (phức tạp thấp) → nếu cần thì Workflow có AI ở một bước là đủ.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Viết quy tắc tính kỳ và bảng ánh xạ cột ra giấy/sheet; dùng làm checklist khi làm tay; lưu file vào thư mục cố định | Khi bước 3–4 chỉ chậm vì phải nhớ ánh xạ, còn thao tác copy-paste nhanh | Vẫn copy-paste tay mỗi sáng nên vẫn có thể dán nhầm kỳ, nhầm cột; tiết kiệm thời gian ít | Không — nhưng **là nền** của mức Rule (bảng ánh xạ và quy tắc kỳ phải viết ra trước) |
| **Rule** | Công thức tính 3 kỳ + Power Query đọc thư mục, áp bảng ánh xạ theo tên cột, lọc đơn hủy/hoàn, điền mẫu, đối chiếu tổng với nguồn và với hôm trước; dừng khi gặp cột lạ | Khi tên cột của sàn ổn định (thứ tự cột có thể đổi vì ánh xạ theo tên — sàn đã đổi thứ tự tuần trước) và định nghĩa chỉ số đã thống nhất — đúng với phần chính của bài | Sàn đổi tên/thứ tự cột làm truy vấn lỗi (đã có phương án quay về A); người tin số tự động nên kiểm tra qua loa (đã có bước duyệt bắt buộc) | **Có — mức chính** |
| **Workflow** | Rule như trên + **một bước AI** soạn nháp 3–5 câu nhận định từ bảng số đã duyệt; người sửa và duyệt | Chỉ khi xác nhận được báo cáo thật sự có phần nhận định bằng lời **và** phần này tốn thời gian đáng kể (câu hỏi 7 chưa hỏi được ở CP4) | AI nhắc số không có trong bảng hoặc suy diễn nguyên nhân sai; thêm chi phí và bước duyệt (đã có phương án quay về B) | **Có điều kiện** — chỉ thêm khi đạt điều kiện ở cột "Đủ khi nào" |
| **Agent** | AI tự đăng nhập sàn, tự tải file, tự đoán ánh xạ cột, tự sửa khi lỗi và tự gửi báo cáo | Khi các bước thay đổi liên tục và không viết trước được — không đúng với bài này | AI đoán sai ánh xạ mà không ai thấy; giữ quyền truy cập tài khoản sàn; đưa dữ liệu nội bộ ra ngoài; khó kiểm tra | **Không** — mọi bước đều xác định trước được, không cần AI tự quyết bước tiếp theo |

**Mức chọn:** **Rule** cho toàn bộ phần ánh xạ, tính kỳ và tính chỉ số. **Workflow có AI ở một bước** (soạn nháp nhận định) chỉ được thêm khi hỏi được câu hỏi 7 và đạt điều kiện ở bảng trên; nếu không đạt, bài dừng ở Rule và trường "AI intervention point" ở mục 7 ghi "Không có" kèm lý do.

**Vì sao không chọn mức đơn giản hơn:**

- **No AI không đủ** vì dù có checklist, nhân viên vẫn copy-paste tay 3 kỳ mỗi sáng và tự mở từng file để kiểm tra; lỗi lệch số (copy theo vị trí cột, quên lọc đơn hủy) đến từ chính thao tác tay này, nên chỉ viết quy tắc ra giấy không loại bỏ được nguồn lỗi.
- **Không lên mức cao hơn Rule cho phần chính** vì đầu ra có đúng/sai rõ ràng: Rule cho kết quả giống nhau mỗi lần, kiểm tra được, không tốn chi phí AI. Dùng AI để ánh xạ cột chỉ thêm khả năng sai mà không thêm giá trị.
- **Workflow chỉ được xét cho phần nhận định bằng lời** vì đây là phần duy nhất Rule không làm được (viết câu tự nhiên mô tả biến động).

### 6.3. AI Canvas rút gọn

*Áp dụng cho bước AI có điều kiện (bước 6 ở mục 4.2). Câu hỏi về phần nhận định bằng lời chưa được hỏi ở CP4; nếu câu trả lời là không có, bỏ phần này.*

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Bản nháp 3–5 câu nhận định: chỉ số nào tăng/giảm đáng kể giữa các kỳ (hôm qua so với trung bình 7 ngày, 7 ngày so với 30 ngày), chỉ nhắc số có trong bảng |
| **Judgment** — con người cân nhắc, quyết định gì? | Nhân viên vận hành xét: câu nào đúng với số, biến động nào thật sự đáng chú ý, nguyên nhân là gì (campaign, hết hàng…) — AI không được tự nêu nguyên nhân |
| **Action** — hành động cuối cùng là gì, ai làm? | Nhân viên vận hành sửa, xóa hoặc giữ từng câu rồi đưa vào báo cáo; AI không gửi báo cáo cho ai |
| **Outcome** — đo kết quả bằng gì? | Số phút viết nhận định trước/sau; số câu nhắc sai số (mục tiêu 0); tỷ lệ câu được giữ nguyên hoặc chỉ sửa nhẹ |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Bảng chỉ số 3 kỳ **đã được người duyệt**, ẩn danh (không tên shop, không dữ liệu khách hàng) + danh sách chỉ số cần nhận định. Có sẵn sau bước 5 của quy trình tương lai; chưa có nếu Rule chưa chạy |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Bản nháp AI so với bản cuối người duyệt (câu nào bị sửa/xóa, vì sao); ghi vào log hằng ngày để chỉnh hướng dẫn cho AI và để quyết định bỏ bước AI theo phương án quay về B |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: **Phần số liệu: automate** bằng Rule (không phải AI), vì đây là việc lặp lại, có đúng/sai rõ và nhân viên chỉ cần duyệt kết quả. **Phần nhận định: augment** — AI chỉ soạn nháp, người quyết định, vì nhân viên vận hành biết bối cảnh (campaign, tình trạng kho) mà bảng số không có. Bằng chứng hiện có là Problem Card của Hạnh ("Vận hành kiểm lại nhận định trước khi dùng"); chưa hỏi được ở CP4 (câu hỏi 7), cần hỏi thêm Hạnh và người nhận báo cáo.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **Báo nhầm tệ hơn** — một câu nhận định nêu sai số hoặc sai xu hướng có thể khiến quản lý ra quyết định sai trong ngày, trong khi bỏ sót một biến động vẫn còn bảng số đầy đủ để người đọc tự thấy. Thiết kế xử lý: AI chỉ đọc bảng đã duyệt, chỉ được nhắc số có trong bảng, không nêu nguyên nhân; người duyệt từng câu; nếu trong 2 tuần có từ 2 lần nhắc sai số thì bỏ bước AI (phương án quay về B). Ở phần Rule, bỏ sót (lỗi cột không bị phát hiện) mới là kiểu tệ hơn, nên Rule được thiết kế dừng và báo lỗi thay vì đoán.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhân viên vận hành sàn thương mại điện tử phụ trách báo cáo định kỳ buổi sáng (hiện làm 2 sàn; pilot bắt đầu với 1 sàn, một mẫu báo cáo công ty); người dùng báo cáo là quản lý / team vận hành trong ngày |
| **Quy trình** | Mỗi sáng ngày làm việc: xác định 3 kỳ → tải 3 file từ sàn → ánh xạ cột nguồn sang mẫu công ty → điền chỉ số 3 kỳ → kiểm tra với nguồn, sai thì làm lại (mục 4.1) |
| **Bottleneck** | Bước 3–4 (ghép + điền bằng tay, 25–30') và bước 5 (kiểm tra tay, 10–20'). **Nguyên nhân gốc:** bảng ánh xạ cột, quy tắc tính kỳ và quy tắc lọc đơn chưa được viết ra, nên mỗi sáng copy theo vị trí cột và phải tự mở từng file để kiểm tra |
| **Impact** | Khoảng 20–22 buổi/tháng × B ≈ 60 phút ≈ 20–22 giờ/tháng; lỗi lệch số (sàn đổi thứ tự cột, đơn hủy lẫn vào) khiến phải sửa lại báo cáo, người nhận phải chờ bản sửa |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian mỗi sáng: B ≈ 60 phút (tự ước lượng) → ≤ 42 phút (bấm giờ 10 buổi pilot; 5 buổi đầu cũng dùng để xác nhận lại B). (2) Số lần lỗi số liệu (sai kỳ, sai cột, đơn hủy lẫn vào) lọt qua bước duyệt: baseline ít nhất 1 lần/tuần gần nhất → 0 (đối chiếu tổng từng kỳ với nguồn). (3) Tỷ lệ chỉ số bắt buộc của 3 kỳ khớp nguồn: → 100%. (4) *Chỉ khi có bước AI:* số câu nhận định nhắc sai số → 0; thời gian viết nhận định giảm ít nhất 50% |
| **Boundary** | Rule làm toàn bộ phần số; AI không ánh xạ cột, không tính hay sửa số, không nêu nguyên nhân biến động, không gửi báo cáo. AI chỉ đọc bảng số **đã duyệt và đã ẩn danh**. Gặp cột lạ/thiếu cột thì Rule dừng và báo lỗi, không đoán. HITL: nhân viên vận hành duyệt bảng số (bước 5) và duyệt từng câu nhận định (bước 7) trước khi dùng |
| **AI intervention point** | **Có điều kiện — bước 6:** soạn nháp 3–5 câu nhận định từ bảng số đã duyệt. Chỉ áp dụng nếu xác nhận được báo cáo có phần nhận định bằng lời và phần này tốn thời gian (câu hỏi 7 chưa hỏi được ở CP4). Nếu không: **"Không có"** — vì mọi đầu ra còn lại có đúng/sai rõ ràng, Rule xử lý được và kiểm tra được |
| **Mức chọn** | **Rule** (phần chính); Workflow có AI ở một bước chỉ khi đạt điều kiện ở trên |
| **Rủi ro & người kiểm tra** | Sàn đổi định dạng file → Rule dừng, Hạnh cập nhật bảng ánh xạ (phương án quay về A). Người tin số tự động, kiểm tra qua loa → bước đối chiếu tổng tự động + Hạnh duyệt các ô bị đánh dấu. AI nhắc sai số → Hạnh duyệt từng câu; 2 lần sai trong 2 tuần thì bỏ bước AI (phương án quay về B). Dữ liệu nội bộ lộ ra ngoài → chỉ đưa bảng đã ẩn danh, hỏi quy định công ty trước khi dùng AI |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Bottleneck | Bước 3–4 (ghép + điền); kiểm tra là bottleneck phụ | Thêm **nguyên nhân gốc**: bảng ánh xạ, quy tắc kỳ và quy tắc lọc đơn chưa được viết ra; nhấn mạnh việc copy theo vị trí cột | Phỏng vấn cho thấy lỗi đến từ copy theo vị trí cột và đơn hủy; khi so 4 mức ở mục 6 thấy viết các quy tắc này ra là điều kiện của mọi phương án |
| Success Metric | 3 chỉ số (thời gian, số ô sai, tỷ lệ khớp nguồn) | Thêm chỉ số (4) cho bước AI; đổi thời gian đo sau khi áp dụng từ 5 buổi thành 10 buổi pilot | Bước AI cần metric riêng về độ đúng; 10 buổi đủ để thấy các lần sàn đổi định dạng hoặc ngày có biến động lớn |
| Boundary | AI không ánh xạ, không tính số; HITL duyệt báo cáo | Thêm: AI không nêu nguyên nhân, không gửi báo cáo, chỉ đọc bảng đã duyệt; thêm bước duyệt nhận định (bước 7) | Câu hỏi PAIR (mục 6.4) cho thấy báo nhầm là lỗi tệ hơn, nên phải chặn AI tự suy diễn |
| AI intervention point | *(chưa có ở v0)* | Bước 6, có điều kiện; nếu không đạt điều kiện thì "Không có" | Ma trận và bảng 4 mức (mục 6.1–6.2) cho thấy phần số chỉ cần Rule |
| Mức chọn | *(chưa có ở v0)* | Rule; Workflow có điều kiện | Như trên; Agent bị loại vì mọi bước xác định trước được |
| Actor / phạm vi | Một sàn | Hạnh làm 2 sàn; pilot bắt đầu với 1 sàn | Phỏng vấn cho thấy Hạnh tải file từ 2 sàn; giữ pilot nhỏ để dễ kiểm soát |

**Tiêu chí đánh giá đầu ra (5 tiêu chí):**

*Tiêu chí 1–3 đánh giá đầu ra của Rule (phần chính, luôn áp dụng); tiêu chí 4–5 đánh giá đầu ra của AI (chỉ khi có bước 6).*

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Đúng kỳ** (Rule) | Ngày bắt đầu/kết thúc của cả 3 kỳ khớp quy tắc đã chốt; số liệu mỗi kỳ lấy từ đúng file của kỳ đó | Có ít nhất 1 kỳ lệch ngày, hoặc dữ liệu kỳ này nằm ở cột của kỳ khác |
| 2 | **Khớp nguồn** (Rule) | Tổng đơn và doanh thu của từng kỳ trong báo cáo bằng tổng trong file nguồn **sau khi đã loại đơn hủy/hoàn**; 100% chỉ số bắt buộc có giá trị | Có chênh lệch không được đánh dấu, đơn hủy/hoàn vẫn bị tính, hoặc thiếu chỉ số bắt buộc |
| 3 | **Dừng đúng lúc khi đầu vào lạ** (Rule) | Khi file nguồn thiếu cột, đổi tên cột hoặc sai kỳ, truy vấn dừng và báo rõ cột/file nào lỗi | Truy vấn vẫn chạy và điền số vào sai cột, hoặc để trống mà không báo |
| 4 | **Chỉ dùng số có trong bảng** (AI) | Mọi con số và xu hướng (tăng/giảm) trong nhận định đều đúng với bảng số đã duyệt | Có ít nhất 1 số không có trong bảng, sai giá trị hoặc sai chiều tăng/giảm |
| 5 | **Không suy diễn ngoài dữ liệu** (AI) | Nhận định chỉ mô tả biến động, không nêu nguyên nhân, không khuyến nghị hành động; dài 3–5 câu | Nêu nguyên nhân ("do campaign…", "do hết hàng…") hoặc khuyến nghị mà bảng không có căn cứ |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** (cho phần Rule) | Cả 2 người phỏng vấn đều mất gần một tiếng mỗi sáng; ghép + điền 25–30' và kiểm tra 10–20'; lỗi lệch số đã xảy ra (tuần trước). Phản bác: ngày bình thường "không quá vất vả", hôm ít dữ liệu ~30'. Số liệu là tự ước lượng của 2 người nên cần bấm giờ ở pilot |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp** | Đầu ra vẫn là mẫu báo cáo công ty mà Hạnh đang dùng; ô lệch nguồn được đánh dấu nên dễ thấy chỗ cần kiểm tra. Nhận định AI (nếu có) chỉ 3–5 câu, sửa trực tiếp được. Rủi ro còn lại: người tin số tự động và kiểm tra qua loa — đã có bước đối chiếu tổng tự động |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **TB** | Công cụ (Excel, Power Query) có sẵn. Đã biết sàn **có** đổi thứ tự cột (tuần trước) → Rule phải khớp theo tên cột và dừng khi lạ; chưa biết sàn có đổi cả tên cột không; trạng thái đơn hủy/hoàn phải có trong file để lọc được; nhóm có ai đã dùng Power Query chưa; dữ liệu cho lab phải ẩn danh. Chỉ Hạnh có dữ liệu và hiểu domain |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **TB** | Phần Rule không tốn thêm chi phí và chạy trên máy công ty. Bước AI cần đưa dữ liệu ra công cụ bên ngoài: **chưa biết quy định của công ty** về dữ liệu bán hàng. Người vận hành và cập nhật bảng ánh xạ là Hạnh — rủi ro phụ thuộc một người khi Hạnh nghỉ |

### 8.2. Kết luận

**Quyết định:** **Go cho pilot Rule** · **Not Yet cho bước AI**

**Lý do:** Phỏng vấn 2 người xác nhận vấn đề có thật và lặp lại (gần một tiếng mỗi sáng, ghép + điền 25–30', đã có lỗi lệch số tuần trước), nên Value của phần Rule thấp rủi ro; ngưỡng đổi đề tài ở mục 2.4 không bị chạm. Pilot Rule rẻ, chạy trên Excel có sẵn và có phương án quay về làm tay. Feasibility vẫn TB vì sàn từng đổi thứ tự cột — pilot chính là cách kiểm chứng điều này. Bước AI vẫn **Not Yet**: chưa hỏi được báo cáo có phần nhận xét bằng lời không (câu hỏi 7) và chưa biết quy định công ty về dữ liệu.

**Nếu Go — pilot nhỏ nhất:** Hạnh chạy **chỉ phần Rule** (bảng ánh xạ theo tên cột, lọc đơn hủy, đối chiếu tổng và so với hôm trước) trong 10 buổi sáng liên tiếp, **một sàn**, một mẫu báo cáo; 5 buổi đầu bấm giờ cả cách làm cũ để xác nhận lại B ≈ 60 phút; vẫn giữ bảng ánh xạ in sẵn để quay về làm tay khi lỗi. Ghi thời gian từng buổi, số ô bị đánh dấu chênh lệch, số lần truy vấn dừng vì lỗi cột. Bước AI chỉ thử sau khi phần Rule đạt mục tiêu và đủ điều kiện ở mục 7.

**Cần kiểm chứng tiếp (phần Not Yet và trong pilot):**

1. **Baseline:** đã có qua phỏng vấn ([cp4-interview-snapshot-1.md](../assets/cp4-interview-snapshot-1.md)); bấm giờ thật ở 5 buổi đầu pilot để thay số tự ước lượng.
2. **Có phần nhận định bằng lời không:** hỏi Hạnh và người nhận báo cáo; nếu không có, bỏ bước AI, mức cuối là Rule.
3. **Định dạng file của sàn:** phỏng vấn cho thấy sàn có đổi thứ tự cột; cần kiểm tra thêm sàn có đổi cả **tên** cột không bằng cách so vài file tải ở các ngày khác nhau.
4. **Quy định công ty:** có được đưa dữ liệu bán hàng (đã ẩn danh) vào công cụ AI bên ngoài không.
5. **Ngoài Hạnh:** mới có 1 đồng nghiệp cũ; hỏi thêm 1–2 người làm báo cáo sàn để xem bước ghép cột hay bước kiểm tra mới là bước lâu nhất.

**Nếu No-Go — nên làm gì thay AI:** *(không áp dụng ở thời điểm này)* Nếu kiểm chứng cho thấy không đáng làm Rule, vẫn nên làm mức No AI: viết quy tắc tính kỳ và bảng ánh xạ cột thành một sheet tham chiếu, dùng làm checklist khi làm tay.

**Ngưỡng dừng:**

- **Trước pilot:** nếu theo phỏng vấn, bước 3–4 chiếm dưới 10 phút/buổi **và** không ai nhớ lần nào bị sai kỳ/sai cột, thì dừng #7 và quay về phương án dự phòng #1 (như mục 2.4). *Kết quả: không chạm ngưỡng — bước 3–4 khoảng 25–30 phút và đã có lỗi tuần trước.*
- **Trong pilot Rule:** nếu sau 10 buổi thời gian trung vị không xuống ≤ 42 phút (0,7 × B), **hoặc** có từ 2 buổi trở lên lọt ô sai qua bước duyệt, thì dừng Rule và quay về làm tay theo bảng ánh xạ (mức No AI).
- **Bước AI (nếu có):** nếu trong 2 tuần có từ 2 lần nhận định nhắc sai số, **hoặc** thời gian viết nhận định không giảm ít nhất 50%, thì bỏ bước AI và giữ Rule.

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế:**

- **Baseline là số tự ước lượng.** Thời gian từng bước ở mục 4, 5, 7 lấy từ trí nhớ của 2 người được phỏng vấn, chưa bấm giờ; hai người còn khác nhau về bước nào lâu nhất (ghép cột hay kiểm tra), nên cần bấm giờ thật ở pilot. 
- **Kiểm chứng ít mẫu:** chỉ 2 buổi phỏng vấn (Hạnh và một đồng nghiệp cũ), trong đó một người là người đề xuất card; chưa đủ để khái quát cho người làm báo cáo sàn nói chung.
- **Phụ thuộc một người:** chỉ Hạnh có dữ liệu, tài khoản sàn và hiểu domain; các thành viên khác chỉ làm được phần research và viết dựa trên số liệu Hạnh cung cấp.
- **Chọn candidate không theo điểm cao nhất:** #7 đứng cuối bảng chấm điểm (mục 2.4). Nhóm đã ghi lý do và đặt ngưỡng đổi đề tài; phỏng vấn cho thấy vấn đề đủ lớn (gần một tiếng mỗi sáng), nhưng đó vẫn là số tự ước lượng.
- **Bước AI chưa chắc tồn tại:** câu hỏi về phần nhận xét bằng lời (giả định 5) chưa được hỏi trong cả hai buổi phỏng vấn.
- **Phạm vi pilot hẹp hơn thực tế:** Hạnh làm báo cáo từ 2 sàn, pilot chỉ thử 1 sàn, một mẫu báo cáo, một người làm; kết luận chưa áp dụng được cho nhiều sàn hoặc nhiều mẫu.

**Hướng tiếp theo:**

| # | Việc | Người phụ trách | Đầu ra |
|---:|---|---|---|
| 1 | Hỏi tiếp Hạnh câu hỏi 7 (phần nhận xét bằng lời) và hỏi quy định công ty về dữ liệu | Thúy + Hạnh | Quyết định có giữ bước AI hay không (mục 6–7) |
| 2 | Viết bảng ánh xạ theo tên cột, quy tắc tính kỳ, quy tắc lọc đơn hủy/hoàn | Hạnh + Minh | Sheet tham chiếu cho Power Query |
| 3 | Kiểm tra báo cáo có sẵn trong trang quản lý của sàn (có xuất đúng 3 kỳ, tùy chỉnh cột được không) | Hạnh + Minh | Bổ sung một dòng vào bảng 3.3 |
| 4 | Chạy pilot Rule 10 buổi trên 1 sàn; 5 buổi đầu bấm giờ cả cách cũ để xác nhận B | Hạnh | Số đo thật thay cho số tự ước lượng; áp ngưỡng dừng ở mục 8.2 |
| 5 | Dựng bảng ánh xạ + Power Query trên dữ liệu ẩn danh; tạo 10 cặp đầu vào/đầu ra mong đợi (10 bộ file của 10 buổi) chấm theo tiêu chí 1–3 ở mục 7 | Hạnh + thành viên học Power Query | Bộ eval trong `report/assets/` |

## 10. Tài liệu tham khảo

**Tài liệu của khóa học**

- [docs/01-worksheet.md](../../docs/01-worksheet.md) — hướng dẫn CP1–CP7, ma trận độ mơ hồ × độ phức tạp, 4 mức can thiệp
- [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md) — tổng hợp các framework dùng trong bài
- Báo cáo cá nhân của các thành viên trong `report/individual/` — nguồn của 12 candidate ở mục 2.1 (Problem Card #7 của Nguyễn Thị Hồng Hạnh)

**Framework**

- Design Council — Framework for Innovation (Double Diamond): https://www.designcouncil.org.uk/resources/framework-for-innovation/
- Intercom — Job Stories: https://www.intercom.com/blog/accidentally-invented-job-stories/
- Teresa Torres — Opportunity Solution Trees: https://www.producttalk.org/opportunity-solution-trees/
- Teresa Torres — Interview Snapshot: https://www.producttalk.org/interview-snapshot/
- Strategyzer — Assumptions Mapping: https://www.strategyzer.com/library/how-assumptions-mapping-can-focus-your-teams-on-running-experiments-that-matter
- Rob Fitzpatrick — The Mom Test: https://www.momtestbook.com/
- Anthropic — Building Effective Agents: https://www.anthropic.com/research/building-effective-agents
- Agrawal, Gans, Goldfarb — AI Canvas (HBR): https://hbr.org/2018/04/a-simple-tool-to-start-making-decisions-with-the-help-of-ai
- Google PAIR Guidebook — User Needs: https://pair.withgoogle.com/chapter/user-needs/
- Marty Cagan (SVPG) — The Four Big Risks: https://www.svpg.com/four-big-risks/

**Công cụ**

- Microsoft Learn — What is Power Query?: https://learn.microsoft.com/en-us/power-query/power-query-what-is-power-query
- Microsoft Learn — Combine files overview (Power Query): https://learn.microsoft.com/en-us/power-query/combine-files-overview
