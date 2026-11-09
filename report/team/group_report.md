# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: **SUDO**
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): **Khi nhân viên gửi yêu cầu hỗ trợ nội bộ (IT, Hành chính, Nhân sự) qua nhiều kênh với mô tả tự do và thiếu thông tin bối cảnh, nhân sự điều phối (Helpdesk/Admin) phải đọc hiểu, hỏi lại thông tin và phân loại thủ công từng yêu cầu để chuyển đúng bộ phận, gây nghẽn thời gian phản hồi ban đầu và dễ chuyển nhầm đầu mối.**
- Quyết định cuối: **Go (phạm vi nhỏ — Pilot 2 tuần với Workflow: Form chuẩn hóa + Rule lọc danh mục cố định + AI kiểm tra thiếu thông tin & gợi ý phân loại + Điều phối viên duyệt chuyển)**

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

*(Xem thông tin chi tiết tại file `TEAM.md` và các bản báo cáo cá nhân)*

### 2.2. Cluster

*(Xem chi tiết ở bản tổng hợp của nhóm trưởng)*

### 2.3. Opportunity Solution Tree rút gọn

*(Xem chi tiết ở bản tổng hợp của nhóm trưởng)*

### 2.4. Chấm điểm shortlist (1–5)

*(Xem chi tiết ở bản tổng hợp của nhóm trưởng)*

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

*(Xem chi tiết ở Mục 3.1 do Phạm Công Dũng phụ trách)*

### 3.2. Kiểm chứng

*(Xem chi tiết ở Mục 3.2 do Phạm Công Dũng phụ trách)*

### 3.3. Research giải pháp đã có

> **Phụ trách chính:** Nguyễn Huy Hoàng (`2A202603366`)

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Atlassian Rovo / Jira Service Management** | `https://www.atlassian.com/software/jira/service-management` | Giải quyết bước phân loại ticket và đề xuất tài liệu hướng dẫn cho agent. | Tích hợp sâu hệ sinh thái enterprise, AI tự động gắn nhãn và phân nhóm ticket rất mạnh. | Quá cồng kềnh, phức tạp và đắt đỏ đối với các tổ chức quy mô nhỏ (50–200 người). | Không tự xây dựng hệ thống quản lý cồng kềnh từ đầu mà học hỏi mô hình phân loại tự động. |
| **Zendesk Intelligent Triage** | `https://www.zendesk.com/service/ticketing/intelligent-triage/` | Giải quyết bước phân tích ý định (intent) và định tuyến ưu tiên từ yêu cầu thô. | Phân tích cảm xúc và ý định người gửi chuẩn xác, tự động hóa routing luồng nhanh. | Khó tùy chỉnh sâu các quy tắc nghiệp vụ đặc thù nội bộ bên ngoài chăm sóc khách hàng. | Cần thiết kế mô hình AI tập trung vào việc đọc hiểu mô tả tự do và gợi ý nhãn phân loại. |
| **Freshservice (Freddy AI)** | `https://www.freshworks.com/freshservice/` | Giải quyết bước tự động đề xuất danh mục sự cố và gán cho nhóm chuyên môn. | Giao diện trực quan, Freddy AI đề xuất danh mục sự cố dựa trên lịch sử dữ liệu cũ tốt. | Chi phí bản quyền cao, phụ thuộc hoàn toàn vào cơ sở dữ liệu lịch sử sẵn có của nền tảng. | Tận dụng cơ chế rule kết hợp AI để gợi ý danh mục cố định giúp tăng tốc độ xử lý. |
| **n8n Workflow Automation (Low-code)** | `https://n8n.io/` | Giải quyết toàn bộ luồng tích hợp Webhook, gọi LLM API trích xuất JSON và điều phối. | Linh hoạt tuyệt đối, dễ kết nối API tự do (Slack/Form với LLM), chi phí tự host tối ưu. | Đòi hỏi kỹ thuật cấu hình và bảo trì hạ tầng workflow riêng của đội ngũ. | Chọn kiến trúc **Workflow** (Form + Rule + LLM + HITL) triển khai qua Low-code/API là khả thi nhất cho lab. |

---

## 4. Quy trình trước/sau (CP5)

*(Xem chi tiết ở Mục 4 do Phạm Việt Hưng phụ trách)*

---

## 5. Problem Statement v0 (CP5)

*(Xem chi tiết ở Mục 5 do Phạm Công Dũng phụ trách)*

---

## 6. Mức can thiệp AI (CP6)

*(Xem chi tiết ở Mục 6 do Phạm Việt Hưng phụ trách)*

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

> **Phụ trách chính:** Nguyễn Huy Hoàng (`2A202603366`)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhân sự điều phối hỗ trợ nội bộ (Helpdesk / Operations / Admin) tại tổ chức quy mô 50–200 người. |
| **Quy trình** | Tiếp nhận yêu cầu hỗ trợ (IT, Hành chính, Nhân sự) gửi qua kênh chat/form với mô tả tự do và thiếu thông tin bối cảnh. |
| **Bottleneck** | Điều phối viên phải đọc thủ công, nhắn tin hỏi lại thông tin cơ bản và phân loại nhầm bộ phận (mất 3.5 phút/yêu cầu, 25% thiếu thông tin, 12% nhầm đầu mối). |
| **Impact** | Gây nghẽn thời gian phản hồi ban đầu, gián đoạn công việc nội bộ và làm quá tải đội ngũ điều phối (\~105 phút/ngày). |
| **Success Metric** (baseline → target, cách đo) | - Thời gian điều phối: từ 3.5 phút xuống < 1 phút/yêu cầu.<br>- Tỉ lệ chuyển nhầm bộ phận: từ 12% xuống < 3%.<br>- Tỉ lệ phải nhắn hỏi lại thông tin cơ bản: từ 25% xuống < 8%.<br>- Tỉ lệ điều phối viên đồng ý với nhãn AI gợi ý: ≥ 80%. |
| **Boundary** | AI không được tự ý đóng yêu cầu, không tự động chuyển thẳng các yêu cầu khẩn cấp hoặc có độ tự tin thấp khi chưa có điều phối viên duyệt thủ công (HITL). |
| **AI intervention point** | LLM trong mô-đun Workflow (kiểm tra thông tin thiếu, tóm tắt 1 câu, gợi ý nhãn phân loại bộ phận và mức độ ưu tiên). |
| **Mức chọn** | **Workflow** (Augment — Hỗ trợ con người) |
| **Rủi ro & người kiểm tra** | Rủi ro AI phân loại nhầm hoặc bỏ sót thông tin; điều phối viên Helpdesk là người kiểm tra và bấm duyệt cuối cùng trước khi chuyển bộ phận. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 (CP5) | v1 (CP6) | Vì sao đổi |
|---|---|---|---|
| **Phạm vi giải pháp** | Chưa chốt rõ mức can thiệp, hướng tới tự động hóa toàn phần. | Xác định rõ mức **Workflow** có người duyệt thủ công (HITL). | Kết quả kiểm chứng và research cho thấy không thể giao phó toàn quyền cho AI (rủi ro phân loại nhầm bộ phận nhạy cảm). |
| **Success Metrics** | Gồm 3 chỉ số cơ bản (thời gian, tỷ lệ nhầm, tỷ lệ hỏi lại). | Bổ sung chỉ số thứ 4: **Tỷ lệ điều phối viên đồng ý với nhãn AI gợi ý (≥ 80%)**. | Cần đo lường trực tiếp độ chính xác và mức độ hữu ích của mô-đun AI trong thực tế vận hành. |
| **Boundary** | Chỉ nêu chung chung không tự động hóa hoàn toàn. | Quy định rõ: AI không đóng ticket, không tự chuyển ca nhạy cảm/độ tự tin < 85%. | Đảm bảo an toàn vận hành, tránh trôi việc hoặc sai sót do AI hiểu sai ngữ cảnh. |

**Tiêu chí đánh giá đầu ra của AI (Eval):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Độ chính xác nhãn gợi ý (Category Accuracy)** | AI gợi ý đúng bộ phận xử lý đạt ≥ 80% so với thực tế duyệt. | AI gợi ý sai bộ phận xử lý vượt quá 20% tổng số ca test. |
| 2 | **Khả năng phát hiện thông tin thiếu (Missing Info Detection)** | Nhận diện chính xác 100% các yêu cầu thiếu bối cảnh cốt lõi để kích hoạt câu hỏi bổ sung. | Bỏ sót các trường hợp thiếu thông tin bắt buộc, khiến điều phối viên vẫn phải hỏi lại thủ công. |
| 3 | **Độ trễ xử lý (Latency)** | Thời gian phản hồi phân tích của AI dưới 3 giây kể từ khi nhận request. | Thời gian phản hồi kéo dài trên 5 giây, gây gián đoạn luồng thao tác. |
| 4 | **Tuân thủ Boundary** | Các yêu cầu có độ tự tin thấp tuyệt đối không tự động chuyển mà phải qua điều phối viên duyệt thủ công (tuân thủ 100%). | AI tự động chuyển hoặc tự xử lý các ca có độ tự tin thấp mà không cần con người duyệt. |

---

## 8. Quyết định (CP6)

*(Xem chi tiết ở Mục 8 do Chu Mai Hồng phụ trách)*

---

## 9. Hạn chế và hướng tiếp theo

*(Xem chi tiết ở Mục 9 do Chu Mai Hồng phụ trách)*

---

## 10. Tài liệu tham khảo

> **Bổ sung bởi:** Nguyễn Huy Hoàng (`2A202603366`)

- Tài liệu hướng dẫn Day 02: Discovery & Problem Framing (K5 Level 3).
- Atlassian Jira Service Management & Zendesk Intelligent Triage Product Documentation.
- Freshservice Freddy AI Capabilities Overview.
- n8n Low-code Workflow Automation Documentation.
- Ghi chú khảo sát và kiểm chứng thực tế từ đội ngũ Vận hành nội bộ.