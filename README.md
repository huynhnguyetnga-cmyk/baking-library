# Baking Library Official V1

Bản chính thức đầu tiên của ứng dụng Baking Library.

## Chức năng
- Chạy thử ngay khi chưa kết nối cloud
- Đăng ký, đăng nhập khi bật Supabase
- Đồng bộ điện thoại và máy tính
- Thêm, sửa, xóa công thức
- Upload nhiều ảnh
- Gallery, tìm kiếm, phân loại, yêu thích, đánh giá
- Bảo mật dữ liệu theo từng tài khoản
- Triển khai được trên Vercel

## Chạy thử trên máy tính
1. Cài Node.js.
2. Mở Terminal tại thư mục dự án.
3. Chạy:
   npm install
   npm run dev
4. Mở địa chỉ hiện trên Terminal.

Khi chưa có file `.env.local`, app tự chạy ở chế độ dùng thử và lưu trên trình duyệt.

## Bật đồng bộ cloud
1. Tạo project Supabase.
2. Mở SQL Editor và chạy file `supabase/schema.sql`.
3. Authentication → Providers → bật Email.
4. Project Settings → API: lấy Project URL và anon key.
5. Copy `.env.example` thành `.env.local` và điền:
   VITE_SUPABASE_URL=...
   VITE_SUPABASE_PUBLISHABLE_KEY=...
6. Chạy lại `npm run dev`.

## Đưa lên Vercel
- Đưa dự án lên GitHub.
- Import repository vào Vercel.
- Thêm hai Environment Variables giống `.env.local`.
- Deploy.
