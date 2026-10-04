# AI-Assisted Test Case Generation

## Tổng quan

Dự án khám phá việc sử dụng AI để phân tích Software Requirements Specification (SRS) và tạo Test Case bằng Claude.

## Mục tiêu

* Tạo Test Case dựa trên các requirement được mô tả trong SRS.
* Ngăn AI tự suy diễn hoặc thêm các behavior không được đề cập.
* Đảm bảo khả năng truy xuất giữa Test Case và requirement.
* Xác định các requirement chưa rõ ràng hoặc chưa đầy đủ.

## Quy trình hiện tại

1. Cung cấp tài liệu SRS cho Claude.
2. Phân tích requirement và xác định các điểm chưa rõ ràng.
3. Tạo Test Case dựa trên nội dung được mô tả trong SRS.
4. Xuất Test Case ra file Excel để review.

## Ví dụ dự án

**Shopee Order Tracking**

Đã tạo 15 Test Case dựa trên SRS được cung cấp. File Excel được lưu trong repository.

## Công nghệ

* Claude AI
* Microsoft Excel
* Git và GitHub
