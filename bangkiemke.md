# BẢNG KIỂM KÊ MÀN HÌNH - DỰ ÁN CRAFTLINK

> **Học phần:** PHÁT TRIỂN ỨNG DỤNG WEB CƠ BẢN – CSE122  
> **Tên dự án:** CraftLink – Sàn sản phẩm sáng tạo tùy biến  

---

## Danh sách màn hình chi tiết

| Vai trò | Mục tiêu người dùng | Nhiệm vụ người dùng | Màn hình | Tệp | CRUD / Trạng thái | AI | Người phụ trách |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Khách hàng** | Khám phá & tìm kiếm sản phẩm | Tìm kiếm, lọc sản phẩm thủ công, xem chi tiết listing | Trang chủ / Khám phá Marketplace | `buyer-marketplace.html` | **R** <br>*(Bình thường, Đang tải, Rỗng)* | Không | **SV1** |
| **Khách hàng** | Tạo yêu cầu đặt hàng tùy chỉnh | Gõ ý tưởng thô, chuyển thành brief chi tiết có cấu trúc | Trình tạo Brief tùy biến (Brief Builder) | `buyer-custom-brief.html` | **C / R / U** <br>*(Nhập liệu, Đang xử lý, Thành công, Lỗi)* | **AI-1: Brief Builder** | **SV1** |
| **Khách hàng** | Theo dõi tiến độ đơn tùy chỉnh | Xem trạng thái đơn hàng, theo dõi các vòng chỉnh sửa | Quản lý Đơn hàng & Tiến độ | `buyer-orders.html` | **C / R / U / D** <br>*(Đang chờ, Đang làm, Hoàn thành, Đã hủy)* | Không | **SV1** |
| **Người sáng tạo** | Quản lý danh mục sản phẩm mẫu | Đăng bán, chỉnh sửa thông tin, ẩn/lưu trữ sản phẩm | Quản lý Listing & Sản phẩm mẫu | `maker-listing-management.html` | **C / R / U / D** <br>*(Bình thường, Đang tải, Rỗng)* | Không | **SV2** |
| **Người sáng tạo** | Tiếp nhận & đánh giá yêu cầu | Xem danh sách brief, nhận gợi ý độ phù hợp từ AI | Hộp thư Brief & Đề xuất tùy biến | `maker-brief-inbox.html` | **R / U** <br>*(Mới đến, Đã phản hồi, Đã từ chối)* | **AI-2: Style Matcher** | **SV2** |
| **Người sáng tạo** | Lập báo giá & mốc thời gian | Soạn thảo proposal, báo giá, hẹn ngày hoàn thành gửi khách | Soạn thảo Proposal & Báo giá | `maker-proposal-editor.html` | **C / R / U / D** <br>*(Nháp, Đã gửi, Khách yêu cầu sửa)* | Không | **SV2** |
| **Người sáng tạo** | Quản lý yêu cầu sửa đổi | Xem tóm tắt nhanh các điểm cần chỉnh sửa | Theo dõi & Tóm tắt yêu cầu sửa đổi | `maker-revision-tracker.html` | **R / U** <br>*(Bình thường, Có thay đổi mới)* | **AI-3: Revision Summarizer** | **SV2** |
| **Kiểm duyệt viên** | Đảm bảo chất lượng bài đăng | Kiểm tra nội dung, duyệt hoặc từ chối sản phẩm mới | Hàng đợi Kiểm duyệt Listing | `moderator-moderation-queue.html` | **R / U** <br>*(Chờ duyệt, Đã duyệt, Từ chối)* | Không | **SV3** |
| **Kiểm duyệt viên** | Giải quyết tranh chấp & báo cáo | Xem báo cáo vi phạm, xử lý/khóa nội dung | Trung tâm Xử lý Báo cáo vi phạm | `moderator-report-center.html` | **C / R / U** <br>*(Chưa xử lý, Đang xem, Đã phạt)* | Không | **SV3** |
| **Kiểm duyệt viên** | Ban hành quy định nền tảng | Cập nhật tiêu chuẩn cộng đồng, chính sách đăng bài | Quản lý Nguyên tắc nội dung | `moderator-content-guidelines.html` | **C / R / U / D** <br>*(Áp dụng, Bản nháp)* | Không | **SV3** |
| **Quản trị viên** | Quản lý phân loại hệ thống | Thêm/sửa/xóa danh mục ngành hàng | Quản lý Danh mục (Taxonomy) | `admin-category-management.html` | **C / R / U / D** <br>*(Hoạt động, Tạm khóa)* | Không | **SV3** |
| **Quản trị viên** | Kiểm soát tài khoản người dùng | Phân quyền, khóa/mở khóa tài khoản vi phạm | Quản lý Tài khoản người dùng | `admin-user-management.html` | **C / R / U** <br>*(Hoạt động, Bị khóa, Chờ xác thực)* | Không | **SV3** |
| **Quản trị viên** | Theo dõi sức khỏe hệ thống | Xem thống kê số lượng đơn hàng, doanh thu, tài khoản | Bảng điều khiển Tổng quan hệ thống | `admin-platform-dashboard.html` | **C / R / U / D** <br>*(Đang tải, Có dữ liệu)* | Không | **SV3** |
| **Dùng chung** | Xác thực & Quản lý hồ sơ | Đăng nhập hệ thống, cập nhật thông tin cá nhân | Đăng nhập & Trang cá nhân | `auth-login.html` / `profile.html` | **C / R / U** <br>*(Chưa đăng nhập, Đã đăng nhập)* | Không | **Chung** |
