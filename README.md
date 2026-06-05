# Customer Segmentation & Marketing Campaign Optimization

**👉 Xem Báo cáo Trực quan (HTML Report): [Bấm vào đây để xem toàn bộ phân tích và biểu đồ](link-xem-truc-tiep)**

---

## 📌 Project Overview

Project nhằm phân khúc khách hàng bán lẻ dựa trên nhân khẩu học và hành vi mua sắm, từ đó xác định tệp khách hàng VIP mang lại tỷ suất hoàn vốn (ROI) cao nhất. Bằng cách kết hợp tư duy phân tích định lượng và trực quan hóa dữ liệu, dự án vạch ra các đặc điểm cốt lõi của từng nhóm khách hàng, làm cơ sở đề xuất chiến lược "Tiếp thị mục tiêu" (Targeted Marketing) thay vì chạy quảng cáo đại trà gây lãng phí ngân sách.

*   **Trạng thái dự án:** Đã hoàn thành (Gồm 1 báo cáo phân tích chi tiết dạng HTML).
*   **Công cụ sử dụng:** R (Data Cleaning, Feature Engineering, EDA, Visualization), RMarkdown.

---

## 🛠️ Tech Stack & Skills Demonstrated

*   **Data Cleaning & Quality Assessment:** Ứng dụng R để xử lý Missing Values bằng phương pháp nội suy trung vị có điều kiện (Conditional Median Imputation), bóc tách và loại bỏ các dữ liệu nhiễu (Outliers) có khả năng làm sai lệch mô hình.
*   **Feature Engineering:** Xây dựng các biến số học mới (`Deal_Dependency`, `Average_Order_Value`, `Behavior_Type`) để lượng hóa chính xác mức độ "nghiện" khuyến mãi và thói quen chi tiêu của khách hàng.
*   **Statistical Analysis:** Ứng dụng tư duy toán học để phân tích phân phối dữ liệu (Distribution), đánh giá độ biến thiên (Standard Deviation) và xác định các mốc phân vị (Quantile) hợp lý để phân nhóm.
*   **Data Storytelling:** Đóng gói và trình bày báo cáo trực quan, tính tương tác cao thông qua RMarkdown.

---

## 🧱 Data Quality Assessment & Feature Engineering (R)

### 1. Chiến lược làm sạch dữ liệu (Data Cleaning)
Dự án tập trung giải quyết các điểm mù dữ liệu để bảo vệ tính toàn vẹn của kết quả phân tích:
* Lấp đầy các giá trị `NULL` ở cột Thu nhập (Income) bằng cách sử dụng các mốc tham chiếu với Tổng chi tiêu (Total Spending), đảm bảo không làm mất đi tệp khách hàng có giá trị cao.
* Loại bỏ các dữ liệu gây nhiễu để đảm bảo biểu đồ phân phối không bị lệch phải quá mức.

## Một số biểu đồ trực quan: 


## 🌟 Executive Summary & Recommendations

**🔍 Key Insights (Phát hiện Cốt lõi):**
* **Chân dung Khách hàng VIP:** Nhóm *High Income - Organic Buyer* (Thu nhập cao - Không săn khuyến mãi) là nhóm mang lại giá trị cao nhất. Dù số lượng ít (209 người), họ có mức chi tiêu khổng lồ (Trung bình: 1,512) và tỷ lệ phản hồi chiến dịch Marketing cao nhất toàn hệ thống (41.6%).
* **Trụ cột Dòng tiền:** Nhóm *Mid Income - Organic Buyer* là tệp khách hàng nòng cốt mang lại dòng tiền ổn định, chiếm số lượng áp đảo (802 người) với mức chi tiêu khá (Trung bình: 941).
* **Tác động Nhân khẩu học:** Khách hàng không có con (Childless) chi tiêu vượt trội, đặc biệt định hướng vào 2 mặt hàng mang lại biên lợi nhuận cao là Rượu (Wines) và Thịt (Meats).

**💡 Actionable Recommendations (Hành động Đề xuất):**
1. **Dịch chuyển Ngân sách:** Ngừng Marketing đại trà, tập trung "Targeted Marketing" trực tiếp vào nhóm *High Income - Organic Buyer* nhằm tối đa hóa tỷ lệ chuyển đổi.
2. **Cá nhân hóa Sản phẩm:** Xây dựng các chiến dịch up-sell chuyên biệt cho mặt hàng Rượu và Thịt, nhắm thẳng vào tệp khách hàng *Childless*.
3. **Khai thác Kênh Online:** Dù cửa hàng vật lý (Store) đang chiếm 46.2% đơn hàng, kênh Website lại cho thấy hiệu suất chuyển đổi cực tốt (Conversion Rate tiệm cận 1.0). Cần phân bổ chi phí để kéo thêm Traffic về Web.

---
## 🙌 Nguồn dữ liệu & Lời cảm ơn (Acknowledgment)
Dự án này sử dụng bộ dữ liệu [Customer Personality Analysis](link-dataset-kaggle) được công bố bởi **Dr. Omar Romero - Hernandez** trên nền tảng Kaggle. Xin gửi lời cảm ơn trân trọng đến tác giả vì đã cung cấp một bộ dữ liệu bán lẻ mang tính thực tiễn cao, hỗ trợ rất lớn cho việc nghiên cứu và phân tích.
