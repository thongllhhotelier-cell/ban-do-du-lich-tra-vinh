# WEBSITE BAN DO SO DU LICH TRA VINH - NCKH 2026

## 1. Gioi thieu
Mau website ban do so du lich Trà Vinh, giới thiệu 12 địa điểm nghiên cứu do nhóm học sinh Trường THPT chuyên Nguyễn Thiện Thành cung cấp.
Website dùng Leaflet (mã nguồn mở), ô bản đồ OpenStreetMap và có thể đăng miễn phí lên GitHub Pages.

## 2. Danh sach tep
- `index.html`: Giao diện, bộ lọc, bản đồ và chức năng.
- `du_lieu.js`: 12 địa điểm gồm tên, tọa độ, nội dung giới thiệu và đường dẫn ảnh (nếu có).
- `anh/`: Để ảnh do học sinh chụp sau khảo sát; chưa có ảnh nào được cung cấp.

## 3. Chay thu tren may tinh
Giải nén file ZIP, mở `index.html` bằng Chrome/Edge. Cần Internet để tải Leaflet và ô bản đồ.

## 4. Dang website MIEN PHI bang GitHub Pages
1. Vào https://github.com và tạo tài khoản GitHub.
2. Chọn New repository, đặt tên `ban-do-du-lich-tra-vinh`, chọn Public, Create repository.
3. Trong kho mã, chọn Add file > Upload files. Kéo **các tệp đã giải nén** `index.html`, `du_lieu.js`, `README.md` (và thư mục `anh/` khi có ảnh) vào thư mục gốc, nhấn Commit changes.
4. Mở Settings > Pages. Ở phần Build and deployment: chọn Deploy from a branch, chọn `main` và `/(root)`, nhấn Save.
5. Khi GitHub Pages xuất bản xong, web sẽ có địa chỉ mẫu: `https://TEN-GITHUB.github.io/ban-do-du-lich-tra-vinh/`. Đây là VÍ DỤ, không phải liên kết đã xuất bản.
6. Muốn cập nhật, sửa file trong kho mã và commit; website sẽ cập nhật sau một khoảng thời gian.

## 5. Them anh va chinh sua du lieu
- Ảnh thực địa: tạo `anh/TV01.jpg` (tương tự cho 12 mã). Trong `du_lieu.js`, đổi thuộc tính `image` của TV01 từ `""` thành `"anh/TV01.jpg"`.
- Sửa thông tin một điểm trong `du_lieu.js`. Không sửa `lat`/`lng` nếu chưa xác minh vị trí.
- Muốn thay đổi màu cụm hoặc tên cụm, tìm biến `GROUPS` trong `index.html`.
- Nút chỉ đường mở Google Maps chỉ khi người dùng nhấn.

## 6. Luu y quan trong cho bai thi
- Dữ liệu giới thiệu giữ theo tệp ngày 09/10/2026, chưa tự biên tập. TV08 dài 225 từ, cần rút xuống 100-150 từ nếu đó là quy định.
- Tên TV05 trong danh mục là `Hợp tác xã Dừa sáp Hòa Tân`, nhưng phần nguyên tắc đầu file còn tên cũ. Cần thống nhất.
- Mã DP01 có mâu thuẫn giữa phần mở đầu và danh mục điểm dự phòng, không đưa vào 12 ghim.
- Tọa độ là theo hồ sơ, cần đối chiếu lại trên Google Maps và khảo sát của học sinh.
- Nguồn OpenStreetMap được ghi công khai trên bản đồ. Không tải trước hàng loạt các ô bản đồ hoặc làm chức năng offline trên máy chủ OSM công cộng.
- GitHub Free cần kho mã công khai để dùng Pages. Không đưa đời tư, thông tin liên lạc cá nhân hay minh chứng chưa xin phép lên mạng.

## 7. Nguon cong nghe va huong dan
- GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages
- Cau hinh xuat ban: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Leaflet: https://leafletjs.com/
- OSM tile usage: https://operations.osmfoundation.org/policies/tiles/
