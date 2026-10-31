# Gốc Chữ Hán: cách cài lên điện thoại

Có hai cách. Cách A tạo file APK. Cách B không cần APK.

## Cách A: tạo APK bằng GitHub (miễn phí, không cần cài Android Studio)

1. Tạo tài khoản GitHub (nếu chưa có) và tạo một repository mới, ví dụ `goc-chu-han`.
2. Tải toàn bộ thư mục này lên repository (nút "Add file" > "Upload files", kéo cả thư mục `www`, `.github`, các file `package.json`, `capacitor.config.json`, `icon-source.png`). Nhớ tải cả thư mục ẩn `.github`.
3. Vào tab "Actions" của repository. Workflow "Build APK" sẽ tự chạy sau khi tải lên (mất khoảng 5 đến 10 phút). Nếu không tự chạy, chọn "Build APK" rồi bấm "Run workflow".
4. Khi chạy xong (dấu tích xanh), mở lần chạy đó, kéo xuống mục "Artifacts" và tải `goc-chu-han-apk`. Giải nén sẽ có file `app-debug.apk`.
5. Gửi file APK sang điện thoại Android, mở lên và cho phép "Cài đặt từ nguồn không xác định" khi máy hỏi.

Ghi chú: đây là bản debug, dùng cá nhân thì đủ. Không đăng lên Google Play được. iPhone không cài được file APK, hãy dùng cách B.

## Cách B: cài thẳng từ trình duyệt (Android và iPhone)

1. Đưa thư mục `www` lên một nơi có địa chỉ https (ví dụ GitHub Pages, Netlify hoặc Cloudflare Pages, đều miễn phí).
2. Mở địa chỉ đó trên điện thoại. Android Chrome: menu ⋮ > "Cài đặt ứng dụng" hoặc "Thêm vào màn hình chính". iPhone Safari: nút Chia sẻ > "Thêm vào Màn hình chính".
3. Ứng dụng mở toàn màn hình như app thường. Sau lần mở đầu tiên có thể dùng khi không có mạng.

## Lưu ý

- Tiến độ học lưu ngay trên điện thoại. Gỡ app hoặc xóa dữ liệu ứng dụng sẽ mất tiến độ.
- Font chữ Hán được tải từ Google Fonts khi có mạng. Khi mất mạng, app dùng font chữ Hán có sẵn của máy.
