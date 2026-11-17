# KẾT QUẢ CHẠY THỬ THỰC TẾ VỚI GIẢI PHÁP 2 (STRUCTURED COT + PROMPT CHAINING)

## 1. Prompt đã sử dụng để chạy thử
> **Vai trò:** Bạn là một Technical Project Manager (Quản lý dự án công nghệ) có 10 năm kinh nghiệm phát triển sản phẩm AI.  
> **Nhiệm vụ:** Lập kế hoạch triển khai dự án Web tư vấn tâm lý tích hợp AI trong 3 tháng (12 tuần).  
> **Quy trình thực hiện (Bắt buộc tuân thủ):**  
> 1. **Chain-of-Thought (Suy luận từng bước):** Trước khi lập lịch, hãy phân tích ngắn gọn 3 yếu tố: Yêu cầu tính năng cốt lõi (Chatbot, giao diện), Rủi ro kỹ thuật, và Nguồn lực cần thiết.  
> 2. **Prompt Chaining (Chia chuỗi thực hiện):** Chia dự án thành 3 giai đoạn (Tháng 1: Thiết kế & Backend; Tháng 2: Tích hợp AI & Frontend; Tháng 3: Kiểm thử & Triển khai). Hiện tại **CHỈ xuất kết quả của Giai đoạn 1 (Tháng 1)** dưới dạng bảng gồm: *Tuần | Đầu việc | Công nghệ sử dụng | Kết quả đầu ra (Deliverable)*.  
> 3. **Xử lý đứt gãy & Duy trì nhất quán:** Cuối phản hồi, hãy tóm tắt 3 gạch đầu dòng về trạng thái hiện tại của dự án và dừng lại để chờ lệnh *"Tiếp tục Giai đoạn 2"*. Không được tự ý viết gộp cả 3 tháng cùng lúc để tránh tràn bộ nhớ ngữ cảnh (Context Window).  
> **Ràng buộc:** Ngôn ngữ chuyên ngành chính xác, thực tế cho người mới bắt đầu (Junior Developer), không giải thích lan man.

---

## 2. Kết quả AI trả về

### PHẦN 1: PHÂN TÍCH CỐT LÕI (CHAIN-OF-THOUGHT)
* **Tính năng cốt lõi:** Giao diện trò chuyện mượt mà, hệ thống quản lý phiên hội thoại (Session) và API kết nối mô hình ngôn ngữ lớn (LLM) với System Prompt định hình phong cách tư vấn tâm lý nhẹ nhàng, đồng cảm.
* **Rủi ro kỹ thuật:** Độ trễ phản hồi của AI (Latency) gây khó chịu cho người dùng; bảo mật dữ liệu nhạy cảm của cuộc trò chuyện; AI đưa ra lời khuyên y khoa vượt quá giới hạn cho phép.
* **Nguồn lực & Công nghệ:** 1 lập trình viên Fullstack (sử dụng React/Next.js cho Frontend, Node.js/Python cho Backend, và Gemini/OpenAI API).

### PHẦN 2: KẾ HOẠCH GIAI ĐOẠN 1 (THÁNG 1 - THIẾT KẾ & XÂY DỰNG NỀN TẢNG)

| Tuần | Đầu việc | Công nghệ sử dụng | Kết quả đầu ra (Deliverable) |
| :--- | :--- | :--- | :--- |
| **Tuần 1** | Phân tích yêu cầu, thiết kế luồng người dùng (User Flow) và giao diện khung (Wireframe). | Figma, Notion | Tài liệu đặc tả tính năng (SRS) & Bản thiết kế UI/UX hoàn chỉnh. |
| **Tuần 2** | Khởi tạo dự án, thiết kế cơ sở dữ liệu lưu trữ người dùng và lịch sử chat. | Node.js (Express), PostgreSQL / MongoDB | Source code khung Backend & Sơ đồ ERD cơ sở dữ liệu. |
| **Tuần 3** | Xây dựng API xác thực người dùng (Đăng ký/Đăng nhập) và API quản lý phòng chat. | JWT, RESTful API, Postman | Bộ API hoạt động ổn định, đã test qua Postman. |
| **Tuần 4** | Thiết kế System Instruction (nhân cách AI tư vấn) và kết nối thử nghiệm API AI. | Google Gemini API / OpenAI API | Module xử lý hội thoại AI chạy thành công trên môi trường local. |

### TRẠNG THÁI DỰ ÁN (TÓM TẮT NGỮ CẢNH)
* Đã hoàn thành kiến trúc hệ thống, database và các API nền tảng trong Tháng 1.
* Đã tích hợp xong nhân cách AI tư vấn tâm lý ở mức độ thử nghiệm (Local).
* Sẵn sàng chuyển sang Giai đoạn 2 (Xây dựng giao diện người dùng & Tối ưu luồng chat thời gian thực).

*Tôi đã hoàn thành Giai đoạn 1. Vui lòng nhập **"Tiếp tục Giai đoạn 2"** để nhận kế hoạch chi tiết cho Tháng 2.*
