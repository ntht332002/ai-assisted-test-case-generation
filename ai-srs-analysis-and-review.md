# SRS Analysis and Review

## Claude Analysis

* **Ambiguous/Conflict – 6.1.3 Triggers và 6.1.5 field 2:** bấm vào thông tin cơ bản của đơn hàng. Triggers nói xem được thông tin chi tiết đơn hàng, field 2 nói chuyển sang trang chi tiết thông tin vận chuyển. Không tạo Test Case.
* **UC002 (xem chi tiết đơn hàng):** SRS chỉ mô tả đường vào qua field 7 (đơn đã giao). Đường vào cho các đơn ở trạng thái còn lại không được mô tả.
* **UC003 (theo dõi trạng thái):** danh sách trạng thái dùng chữ "như:", chưa rõ có đầy đủ hay không. Chuyển đổi giữa các trạng thái không được mô tả.
* **Điều hướng tới các màn hình:** SRS không mô tả cách vào màn hình thông tin vận chuyển, màn hình đơn hàng đã hủy, màn hình liên hệ người bán. Cũng không rõ khung chat (field 3) có phải là màn hình liên hệ người bán hay không.
* **Điều kiện hiển thị nút "Mua lại", "Xem đánh giá":** SRS không nêu áp dụng cho trạng thái đơn hàng nào.
* **Nội dung trang chi tiết hủy đơn, trang cửa hàng, hành vi gửi tin nhắn, kiểu khớp khi tìm kiếm Shop, tên hiển thị các lựa chọn của combobox:** SRS không mô tả.
* **Pre-condition (6.1.3):** SRS không mô tả hành vi khi chưa đăng nhập hoặc tài khoản không có đơn hàng nào, nên không có Negative Test Case.
* **6.1.7 User-validation rules:** bảng trống, không có Validation/Boundary Test Case.
* **Mục 7 Others requirements (bảo mật, hiệu suất, kết nối API, thời gian thực, thông báo, quản lý lỗi và ngoại lệ, tương thích nền tảng, quyền riêng tư, hỗ trợ khách hàng):** chỉ nêu nguyên tắc chung, không có tiêu chí cụ thể để kiểm thử.

## Review

### Điểm đúng

* ✅ Xác định đúng các requirement mâu thuẫn/chưa rõ.
* ✅ Nhận diện được các requirement còn thiếu thông tin.
* ✅ Không tự suy diễn để bổ sung requirement.
* ✅ Nhận ra phần validation và NFR chưa đủ chi tiết để tạo test case.

### Điểm cần cải thiện

* ⚠️ Cần phân biệt rõ **behavior được mô tả trong SRS** và behavior chỉ được AI suy diễn.
* ⚠️ Nên nhấn mạnh hơn mâu thuẫn giữa **UC002 – field 2 – field 7**.
* ⚠️ Không nên xem các behavior được mô tả trong phần **Screen Description/Prototype** là ngoài SRS.

### Kết luận

Phần phân tích của Claude **đủ tốt để làm cơ sở generate test case**, nhưng vẫn cần review thủ công để đảm bảo **100% test case chỉ dựa trên requirement được SRS mô tả**.
