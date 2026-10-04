# Claude Prompt – SRS-Based Test Case Generation

Đọc file SRS tôi cung cấp và **chỉ generate Test Case dựa trên nội dung được mô tả trong SRS**.

## Quy tắc bắt buộc

* SRS là **source of truth duy nhất**.
* Không tự ý sửa, bổ sung hoặc diễn giải lại requirement.
* Không suy đoán behavior mà SRS không đề cập.
* Không tạo Test Case dựa trên kinh nghiệm QA hoặc nghiệp vụ bên ngoài SRS.
* Không lấy behavior từ Prototype/UI nếu SRS không mô tả behavior đó.
* Chỉ tạo Positive/Negative/Boundary/Validation Test Case khi SRS có đủ thông tin để kiểm thử.
* Nếu SRS không đề cập behavior hoặc không đủ thông tin → **không tạo Test Case**.
* Không tạo duplicate Test Case.
* Mỗi Test Case phải trace được về requirement trong SRS.
* Giữ nguyên terminology và ý nghĩa của SRS.

## Output Format

**Chỉ trả về bảng Test Case**, không cần phân tích SRS dài dòng.

| TC ID | Requirement/Source | Test Case | Preconditions | Test Steps | Test Data | Expected Result |
| ----- | ------------------ | --------- | ------------- | ---------- | --------- | --------------- |

Sau bảng, chỉ thêm một mục ngắn:

## Insufficient / Ambiguous Requirements

Liệt kê những requirement không thể tạo Test Case vì SRS thiếu thông tin hoặc có mâu thuẫn. Không tự giải quyết hoặc suy đoán thay SRS.

## Không cần

* Requirement Summary
* Coverage Check
* Giải thích lại nội dung SRS
* Phân tích Prototype
* Đề xuất sửa SRS
* Đề xuất requirement mới

**Hãy bắt đầu trực tiếp từ bảng Test Case.**
