# Screen Inventory

> Bảng này là nguồn kiểm kê màn hình để nhóm cập nhật trong suốt dự án. Danh sách 12 màn hình dưới đây là bộ khung bắt buộc ban đầu; có thể bổ sung màn hình khi luồng nghiệp vụ cần.

| ID | Role | Screen | File | CRUD/State | AI | Owner |
|---|---|---|---|---|---|---|
| 01 | Buyer | Marketplace | pages/buyer-marketplace.html | R | - | SV1 |
| 02 | Buyer | Custom Brief | pages/buyer-custom-brief.html | C/R/U | Brief Builder | SV1 |
| 03 | Buyer | Buyer Orders | pages/buyer-orders.html | C/R/U/D | - | SV1 |
| 04 | Maker | Listing Management | pages/maker-listing-management.html | R | - | SV2 |
| 05 | Maker | Brief Inbox | pages/maker-brief-inbox.html | C/R/U | Style Matcher | SV2 |
| 06 | Maker | Proposal Editor | pages/maker-proposal-editor.html | C/R/U/D | - | SV2 |
| 07 | Moderator | Moderation Queue | pages/moderator-moderation-queue.html | R | - | SV3 |
| 08 | Moderator | Report Center | pages/moderator-report-center.html | C/R/U | - | SV3 |
| 09 | Moderator | Content Guidelines | pages/moderator-content-guidelines.html | C/R/U/D | - | SV3 |
| 10 | Admin | Category Management | pages/admin-category-management.html | R | - | SV3 |
| 11 | Admin | User Management | pages/admin-user-management.html | C/R/U | - | SV3 |
| 12 | Admin | Platform Dashboard | pages/admin-platform-dashboard.html | C/R/U/D | - | SV3 |
| 13 | Shared | Landing / Marketplace | pages/index.html | R | - | Shared |
| 14 | Shared | Login | pages/login.html | R | - | Shared |
| 15 | Shared | Register | pages/register.html | C/R | - | Shared |
| 16 | Shared | Profile | pages/profile.html | R/U | - | Shared |
| 17 | Shared | Notifications | pages/notifications.html | R/U | - | Shared |
| 18 | Buyer | Proposal / Revision Detail | pages/buyer-proposal-detail.html | R/U | Revision Summarizer | SV1 |

## State coverage to review
Normal, Loading, Empty, Success, Error, Disabled, Pending, Rejected, Completed, Cancelled/Archived where applicable.
