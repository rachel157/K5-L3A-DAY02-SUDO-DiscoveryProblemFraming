# Báo cáo cá nhân — 2A202603366_NguyenHuyHoang

## 1. Thông tin học viên

- Họ tên: Nguyễn Huy Hoàng
- MSSV: 2A202603366
- Email trường: 
- Tên nhóm: SUDO
- Link repo nhóm: https://github.com/rachel157/K5-L3A-DAY02-SUDO-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | **Tốn thời gian** & **Lặp lại** | Khi nhân viên nội bộ gửi yêu cầu hỗ trợ (IT, Hành chính, Nhân sự) qua nhiều kênh với mô tả tự do và thiếu thông tin bối cảnh, tôi muốn hệ thống tự động gom nhóm, kiểm tra thông tin thiếu và gợi ý phân loại đúng bộ phận xử lý, để không phải đọc thủ công từng tin nhắn và hỏi lại mất thời gian. | Nhân sự điều phối (Helpdesk / Operations / Admin), Nhân viên IT Support | Xảy ra hằng ngày với quy mô 50–200 người, xử lý trung bình 30 yêu cầu/ngày; quy trình cũ mất trung bình 3.5 phút/yêu cầu (~105 phút/ngày). |
| 2 | **Cần đọc, tổng hợp nhiều thông tin** | Khi tìm kiếm tài liệu nghiên cứu công nghệ mới hoặc thư viện cho đồ án, tôi muốn tổng hợp các bài viết, tài liệu API và mã nguồn mẫu từ nhiều nguồn, để không phải mở hàng chục tab trình duyệt và đọc lặp lại thông tin cũ. | Sinh viên làm đồ án tốt nghiệp, lập trình viên | Diễn ra hằng ngày trong giai đoạn R&D; mất từ 1-2 tiếng mỗi ngày chỉ để lọc và đọc tài liệu phân tán. |
| 3 | **Pain từ người khác** | Khi quản lý các yêu cầu hỗ trợ kỹ thuật rải rác trên nhiều kênh (Slack, Zalo, email), tôi muốn có một hệ thống ghi nhận tập trung (Ticketing system), để tránh việc tin nhắn trôi đi khiến các yêu cầu khẩn cấp bị bỏ sót. | Trưởng bộ phận IT, Nhân viên cần hỗ trợ | Xảy ra liên tục trong tuần; có sự cố bị phản hồi chậm do trôi tin nhắn trên group chat chung. |
| 4 | **Lặp lại** & **Tốn thời gian** | Khi ứng tuyển thực tập và cập nhật CV trên các nền tảng tuyển dụng (TopCV), tôi muốn tự động điều chỉnh mô tả dự án và kỹ năng trong CV sao cho khớp với từ khóa của từng Job Description (JD), để không phải sửa thủ công từng dòng cho mỗi lần nộp hồ sơ. | Sinh viên năm cuối, ứng viên tìm việc Fresher | Diễn ra mỗi khi ứng tuyển một vị trí mới; mất khoảng 20-30 phút chỉnh sửa tỉ mỉ cho mỗi bộ hồ sơ. |
| 5 | **Cần đọc, tổng hợp nhiều thông tin** | Khi tham gia các khóa học lập trình dài hạn hoặc xem các chuỗi podcast kỹ thuật, tôi muốn trích xuất và tóm tắt các điểm cốt lõi thành tài liệu ngắn gọn, để dễ ôn tập lại mà không phải tua lại video hàng tiếng đồng hồ. | Sinh viên tự học, học viên các chương trình đào tạo công nghệ | Xảy ra hằng tuần; mỗi video dài 1-3 tiếng, tốn rất nhiều thời gian xem lại khi cần ôn kiến thức. |
| 6 | **Pain từ người khác** | Khi các thành viên trong nhóm làm đồ án phân công công việc và theo dõi tiến độ qua các công cụ quản lý, tôi muốn nhận được cảnh báo tự động khi có task bị chậm deadline, để nhóm không bị dồn việc vào phút chót trước ngày nộp. | Thành viên nhóm đồ án, nhóm trưởng (Project Manager) | Xảy ra xuyên suốt quá trình làm đồ án; tuần nào cũng có ít nhất 1-2 task bị trễ hạn do không theo dõi sát sao. |
| 7 | **Tốn thời gian** & **Lặp lại** | Khi làm đồ án nhóm, tôi muốn tự động đồng bộ hóa và kiểm tra trạng thái các biến môi trường (env/secrets) giữa các thành viên, để không bị lỗi xung đột hoặc lộ thông tin bảo mật khi push code lên GitHub. | Sinh viên làm đồ án nhóm, Fresher Engineer | Xảy ra mỗi khi bắt đầu sprint mới hoặc có thành viên join nhóm; mất 15-30 phút cấu hình lại file `.env` thủ công. |
| 8 | **Lặp lại** & **Pain từ người khác** | Khi quản lý các thông báo, lịch sinh hoạt và tài liệu học tập trong các kênh cộng đồng (như Slack hoặc Discord), tôi muốn hệ thống tự động gom nhóm các thông báo quan trọng theo chủ đề, để không bị trôi tin nhắn và bỏ lỡ deadline. | Thực tập sinh, sinh viên tham gia các chương trình đào tạo thực tế | Xảy ra hằng ngày; hàng trăm tin nhắn trôi qua khiến sinh viên dễ bỏ lỡ thông báo lịch họp hoặc deadline quan trọng. |

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tiếp nhận và phân loại yêu cầu hỗ trợ nội bộ (Internal Helpdesk Ticketing) | Pain rất rõ từ bộ phận Helpdesk/Operations (30 yêu cầu/ngày, mất 3.5 phút/yêu cầu), tần suất cao, dễ sót việc và chuyển nhầm. | Liệu nhân viên có chịu thay đổi thói quen điền Form chuẩn hóa thay vì nhắn tin tự do không? |
| 2 | Đồng bộ và quản lý biến môi trường (`.env`/secrets) khi làm đồ án nhóm | Xảy ra thường xuyên trong các dự án phần mềm, ảnh hưởng trực tiếp đến tốc độ phát triển và bảo mật. | Mức độ phức tạp của các cấu hình bảo mật có vượt quá phạm vi bài toán đơn giản không? |
| 3 | Tối ưu hóa mô tả CV theo từng Job Description (JD) khi ứng tuyển thực tập | Giúp tiết kiệm thời gian chỉnh sửa hồ sơ lặp đi lặp lại cho sinh viên năm cuối chuẩn bị đi làm. | Độ chính xác của việc parse JD và match kỹ thuật bằng AI có đủ tin cậy với người dùng không? |

### Problem Card #1 (Trọng tâm của nhóm)

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhân viên gửi yêu cầu hỗ trợ nội bộ (IT, Hành chính, Nhân sự) qua nhiều kênh với mô tả tự do và thiếu thông tin bối cảnh, tôi muốn nhân sự điều phối (Helpdesk/Admin) có công cụ tự động kiểm tra thông tin thiếu và gợi ý phân loại đúng bộ phận, để giảm thời gian xử lý thủ công và hạn chế tối đa việc chuyển nhầm đầu mối. |
| Actor | Nhân sự điều phối hỗ trợ nội bộ (Helpdesk / Operations / Admin) tại tổ chức quy mô 50–200 người. |
| Thời điểm / bối cảnh | Xảy ra liên tục trong giờ làm việc hằng ngày khi tiếp nhận khoảng 30 yêu cầu/ngày từ nhân viên. |
| Quy trình hiện tại (3–7 bước) | 1. Nhân viên gửi yêu cầu qua kênh chat/email với mô tả tự do.<br>2. Điều phối viên đọc hiểu thủ công nội dung.<br>3. Điều phối viên nhắn hỏi lại thông tin thiếu.<br>4. Điều phối viên tự định nghĩa danh mục và phân công cho bộ phận IT/HR/Admin.<br>5. Chuyển tiếp yêu cầu và theo dõi xử lý. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, 3 & 4 (Đọc hiểu mô tả tự do thiếu thông tin, nhắn hỏi lại và phân loại thủ công); chiếm ~2.5 phút/yêu cầu (khoảng 25% yêu cầu bị thiếu thông tin phải hỏi lại và 12% bị chuyển nhầm bộ phận). |
| Success metric (baseline → target) | - Thời gian điều phối: từ 3.5 phút xuống < 1 phút/yêu cầu.<br>- Tỉ lệ chuyển nhầm bộ phận: từ 12% xuống < 3%.<br>- Tỉ lệ phải nhắn hỏi lại thông tin cơ bản: từ 25% xuống < 8%.<br>- Tỉ lệ điều phối viên đồng ý với nhãn AI gợi ý: ≥ 80%. |
| Phương án không dùng AI | Dùng Form chuẩn hóa kết hợp Rule định danh danh mục cố định (ví dụ chọn dropdown danh mục), không xử lý được các mô tả tự do phức tạp. |
| Giả thuyết về AI (nếu có) | Dùng Workflow kết hợp LLM để kiểm tra thông tin thiếu, tóm tắt 1 câu và gợi ý nhãn bộ phận kèm mức độ ưu tiên. |
| Cảm nhận nhanh | Workflow |

---

## 4. Phần việc chi tiết của cá nhân trong nhóm (CP3 → CP7)

### 4.1. Research giải pháp thị trường (CP4 - Phụ trách chính Mục 3.3 trong báo cáo nhóm)
Tôi đã kiểm tra trực tiếp và tổng hợp 4 giải pháp thực tế trên thị trường:
1. **Atlassian Rovo / Jira Service Management:** Tích hợp AI phân loại request và gợi ý tài liệu khắc phục sự cố.
2. **Zendesk Intelligent Triage:** Sử dụng AI phân tích ý định để tự động gắn thẻ và định tuyến ưu tiên.
3. **Freshservice (Freddy AI):** Tự động đề xuất danh mục sự cố và gán ticket cho nhóm chuyên môn.
4. **n8n Workflow Automation (Low-code):** Xây dựng luồng kết nối Webhook, gọi LLM API để trích xuất cấu trúc dữ liệu.
*Kết luận từ Research:* Đã có sẵn các công cụ giải quyết bài toán trên thị trường, nhóm **không tự xây dựng hệ thống từ đầu** mà tích hợp theo mô hình Workflow sẵn có.

### 4.2. Viết Problem Statement v1 & Bộ tiêu chí Eval (CP6 - Phụ trách chính Mục 7 trong báo cáo nhóm)
* **Problem Statement v1 (Đã đồng bộ toàn nhóm):**
  > *Khi nhân viên gửi yêu cầu hỗ trợ nội bộ (IT, Hành chính, Nhân sự) qua nhiều kênh với mô tả tự do và thiếu thông tin bối cảnh, nhân sự điều phối (Helpdesk/Admin) phải đọc hiểu, hỏi lại thông tin và phân loại thủ công từng yêu cầu để chuyển đúng bộ phận, gây nghẽn thời gian phản hồi ban đầu và dễ chuyển nhầm đầu mối. Bằng cách áp dụng **Workflow** (Form chuẩn hóa cho yêu cầu cố định + Rule lọc danh mục + LLM kiểm tra thông tin thiếu, tóm tắt và gợi ý nhãn phân loại cho yêu cầu tự do + Duyệt thủ công bởi điều phối viên), chúng ta kỳ vọng giảm thời gian điều phối từ 3.5 phút xuống dưới 1 phút/yêu cầu, hạ tỷ lệ chuyển nhầm bộ phận từ 12% xuống dưới 3%, hạ tỷ lệ phải nhắn hỏi lại từ 25% xuống dưới 8%, và đạt tỷ lệ điều phối viên đồng ý với nhãn AI gợi ý ≥ 80%, với ràng buộc AI không được tự ý đóng hoặc chuyển thẳng yêu cầu nhạy cảm/độ tự tin thấp khi chưa có người duyệt.*

* **Bộ tiêu chí đánh giá (Eval) cho mô-đun AI Workflow:**
  1. **Độ chính xác nhãn gợi ý (Category Accuracy):** AI gợi ý đúng bộ phận xử lý đạt ≥ 80% so với thực tế duyệt.
  2. **Khả năng phát hiện thông tin thiếu (Missing Info Detection):** Nhận diện chính xác 100% các yêu cầu thiếu bối cảnh cốt lõi để kích hoạt câu hỏi bổ sung.
  3. **Độ trễ xử lý (Latency):** Thời gian phản hồi phân tích của AI dưới 3 giây.
  4. **Tuân thủ Boundary:** Các yêu cầu có độ tự tin thấp tuyệt đối không tự động chuyển mà phải qua điều phối viên duyệt thủ công (tuân thủ 100%).

---

## 5. Dùng AI

| Checkpoint | Nhân sự / AI làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 & CP2 | Hỗ trợ cấu trúc hóa Problem Card và số liệu baseline. | Chuẩn hóa văn phong Job Story và Success Metrics. | Đưa ra số liệu ước lượng cảm tính không sát thực tế doanh nghiệp. | Căn chỉnh lại số lượng 30 yêu cầu/ngày và baseline 3.5 phút theo số liệu thực tế của nhóm. |
| CP4 Research | Tìm kiếm các giải pháp thị trường (Jira, Zendesk, n8n). | Cung cấp góc nhìn về kiến trúc Workflow tích hợp LLM sẵn có. | Đề xuất các hệ thống Enterprise quá đắt đỏ so với quy mô 50–200 người. | Lọc chọn các mô hình Low-code / Workflow linh hoạt, phù hợp để Pilot. |
| CP6 Eval & v1 | Xây dựng tiêu chí Eval và hoàn thiện Problem Statement v1. | Đồng bộ hóa chỉ số đo lường với các thành viên khác trong nhóm. | Đặt chỉ số đánh giá quá lỏng lẻo (không có mốc định lượng rõ ràng). | Thiết lập các ngưỡng số cụ thể cho Eval (ví dụ: độ đồng ý ≥ 80%, độ trễ < 3s). |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì từ quá trình làm bài chung của nhóm?**
Việc kiểm chứng thực tế qua *The Mom Test* và dữ liệu research đã giúp nhóm loại bỏ hoàn toàn các ý tưởng lan man (như dùng AI giải quyết toàn bộ sự cố). Chúng tôi nhận ra rằng sự cố thực sự nằm ở **khâu đầu vào (mô tả tự do thiếu thông tin) và khâu định tuyến thủ công**, từ đó việc kết hợp Form + Rule + Workflow là phương án tối ưu và khả thi nhất.

**6.2. Hiểu bài:** 
Chuỗi bài toán của nhóm đi từ **problem** Helpdesk mất 3.5 phút/yêu cầu do mô tả tự do và thiếu thông tin. **Bottleneck** nằm ở việc đọc hiểu và phân loại thủ công. Nhóm chọn mức can thiệp **Workflow** (Form + Rule + AI gợi ý + Người duyệt) với mục tiêu giảm thời gian xuống < 1 phút, giảm nhầm lẫn xuống < 3%. **Boundary** giữ chân con người ở khâu duyệt cuối cùng đối với ca rủi ro/độ tự tin thấp. Cuối cùng, nhóm đưa ra quyết định **Go với Pilot 2 tuần** kèm 3 ngưỡng dừng định lượng rõ ràng.

---

## 7. Tài liệu tham khảo

- Tài liệu hướng dẫn Day 02: Discovery & Problem Framing (K5 Level 3).
- Atlassian Jira Service Management & Zendesk Intelligent Triage Documentation.
- Ghi chú khảo sát và kiểm chứng thực tế từ đội ngũ Vận hành nội bộ.