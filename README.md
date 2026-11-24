# Lối Khám

Nguyên mẫu web giúp người bệnh ngoại trú biết bước khám tiếp theo và tìm đường đến đúng phòng.

- **Quét mã trên phiếu số thứ tự** để thấy cả hành trình khám và **bước tiếp theo** (đóng tiền, phòng khám, xét nghiệm, nhận thuốc), kèm hình minh họa và những thứ cần mang theo.
- **Quét mã QR “Bạn đang ở đây”** dán tại các ngã rẽ để được chỉ đường từng bước, không cần GPS, thiết bị phát sóng hay cài ứng dụng.
- Chế độ **chữ to** và **đọc to** cho người cao tuổi; nút **Nhờ hỗ trợ** hiện mã để bảo vệ hoặc nhân viên Công tác xã hội tra cứu.
- **Màn hình cho bảo vệ và Phòng Công tác xã hội** minh họa cách tra cứu bước hiện tại, xem mốc quét gần nhất và gửi chỉ dẫn trong cùng phiên mô phỏng.
- **Nhật ký quét mã** hiển thị thời gian tìm đường giả lập theo từng chặng.

[Mở nguyên mẫu](https://btphuong3011.github.io/loi-kham/) · [Xem tuyến thí điểm đề xuất](https://btphuong3011.github.io/loi-kham/#tuyen-thi-diem)

Bấm **“Chạy kịch bản mẫu”** để xem hành trình, kể cả bước chọn theo phiếu chỉ định sau khám. Có thể bấm các ô QR màu vàng để quét thử hoặc mở **“Điểm cần hỗ trợ”** để xem các tín hiệu trên bản đồ.

## Tuyến thí điểm đề xuất

Nhóm đề xuất đánh giá một tuyến từ quầy tiếp nhận đến phòng khám đầu tiên, sau khi người bệnh hoàn tất thủ tục tiếp nhận. Ca mô phỏng trên trang minh họa tuyến đến phòng 205. Khi có bệnh viện phối hợp, nhóm sẽ thống nhất tuyến, diễn tập và so sánh chỉ dẫn hiện hành với chỉ dẫn có thêm Lối Khám trên cùng tuyến, trong các khung giờ tương đương.

Chỉ số chính là thời gian tìm đường từ lúc rời quầy đến đúng cửa phòng. Nhóm ghi riêng khoảng chờ. Chỉ số bổ sung gồm số lượt hỏi đường trên mỗi người và tỷ lệ đến đúng phòng ngay lần đầu.

## Lưu ý

- Bệnh viện, bản đồ, phiếu khám và mọi số liệu trong nguyên mẫu đều là giả lập.
- Nguyên mẫu không kết nối hệ thống thông tin của bệnh viện và không thu thập dữ liệu sức khỏe.
- Không dùng trong cấp cứu. Khi cấp cứu, hãy đến Khoa Cấp cứu hoặc gọi **115**.

## Chạy trên máy

Mở `index.html` bằng trình duyệt; không cần cài đặt hay máy chủ.

## Cập nhật sau vòng sơ khảo (từ 22/11/2026)

Bản nộp kèm hồ sơ được lưu ở mốc [`ban-nop-ho-so`](https://github.com/btphuong3011/loi-kham/tree/ban-nop-ho-so) (commit 29f22cb). Trang chính hiện có thêm:

- **Bác sĩ cho làm gì tiếp?** Giai đoạn 1 chưa kết nối hệ thống bệnh viện, nên hành trình chỉ biết trước các bước tới phòng khám. Khám xong, người bệnh hoặc nhân viên chọn đúng mục trên phiếu chỉ định giấy (đo điện tim, lấy máu, siêu âm – X-quang) hoặc đơn thuốc; ứng dụng tự thêm các bước và chỉ đường. Ứng dụng chỉ cần biết phòng nào, không cần biết bệnh gì.
- **Phiếu hành trình in giấy** cho người không dùng điện thoại: bảo vệ hoặc quầy hỗ trợ bấm *In phiếu hành trình giấy*; phiếu A4 có sơ đồ lộ trình, các bước, khu, tầng, màu vạch sơn, ô đánh dấu đã xong và các lựa chọn sau khám.
- **Bản đồ điểm cần hỗ trợ** tổng hợp lượt quét lặp, đi lệch tuyến hoặc yêu cầu hỗ trợ. Nhân viên có thể dùng các tín hiệu này để chọn vị trí cần kiểm tra biển chỉ dẫn.

Dữ liệu trên bản đồ gồm số liệu mẫu và các lượt thử trên trang. Đường dẫn `/v2/` tự chuyển về trang chính.
