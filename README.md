# ThanhDat-Prototype

Prototype quản lý kho, báo giá, phê duyệt, hợp đồng và BOQ cho buổi demo khách hàng. Giao diện dùng React 19, HeroUI v3, HTML/CSS/JavaScript và Vite.

## Chạy

```bash
npm install
npm run dev
```

Mở `http://localhost:5173/`. Build bản tĩnh bằng `npm run build` (thư mục `dist/`).

## Luồng demo

1. **Kho sản phẩm:** Import Excel theo file mẫu hoặc thêm tay. Sản phẩm mới ở trạng thái chờ duyệt.
2. **Báo giá:** Chọn sản phẩm đã duyệt từ kho, nhập số lượng, lợi nhuận và thuế. Tổng tiền cập nhật theo từng dòng; gửi để quản lý duyệt.
3. **Phê duyệt:** Chuyển vai trò trong góc phải sang Quản lý / Trưởng phòng để duyệt hoặc từ chối kèm lý do.
4. **Tài liệu xuất:** Báo giá đã duyệt có thể tải `.xlsx` và hợp đồng mẫu `.docx`.
5. **BOQ & vật tư:** Import BOQ hoặc nhập tay; công trường đề xuất vật tư theo đợt. Vượt định mức sẽ có cảnh báo trong BOQ và trung tâm phê duyệt.

Dữ liệu demo được lưu trong `localStorage` của trình duyệt. Vai trò chỉ mô phỏng trải nghiệm; bản prototype chưa có đăng nhập, máy chủ, phân quyền bảo mật, đồng bộ nhiều người dùng hay mẫu hợp đồng pháp lý chính thức.
