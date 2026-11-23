# Lối Khám

Nguyên mẫu web giúp người bệnh ngoại trú đi khám không bị lạc trong bệnh viện:

- **Quét mã trên phiếu số thứ tự** để thấy cả hành trình khám và **bước tiếp theo** (đóng tiền, phòng khám, xét nghiệm, nhận thuốc), kèm hình minh họa và những thứ cần mang theo.
- **Quét mã QR “Bạn đang ở đây”** dán tại các ngã rẽ để được chỉ đường từng bước, không cần GPS, thiết bị phát sóng hay cài ứng dụng.
- Chế độ **chữ to** và **đọc to** cho người cao tuổi; nút **Nhờ hỗ trợ** hiện mã để bảo vệ hoặc nhân viên Công tác xã hội tra cứu.
- **Màn hình cho bảo vệ và Phòng Công tác xã hội**: tra cứu bước hiện tại của người bệnh, gửi chỉ dẫn tới điện thoại, xem thống kê câu hỏi đường đi để biết biển chỉ dẫn nào cần sửa.
- **Nhật ký quét mã** ghi thời gian tìm đường của từng chặng, phục vụ đánh giá khi thử nghiệm.

**Xem trực tiếp:** https://btphuong3011.github.io/loi-kham/

Bấm **“Chạy kịch bản mẫu”** để xem một người bệnh đi hết buổi khám, kể cả bước chọn chỉ định sau khám; hoặc bấm vào các ô QR màu vàng trên bản đồ để quét thử. Bấm **“Xem điểm lạc đường”** để xem bản đồ cho bệnh viện.

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
- **Bản đồ điểm lạc đường** cho bệnh viện: mỗi mã QR cộng dồn số lượt quét lặp (cùng mã trong 10 phút), đi lệch lộ trình và nhờ hỗ trợ; màn hình nhân viên nêu hai điểm nhiều nhất kèm gợi ý sửa biển chỉ dẫn, để đo lại sau khi sửa.

Dữ liệu vẫn là giả lập; số liệu điểm lạc đường là dữ liệu mẫu cộng các lượt thử trên trang. Đường dẫn `/v2/` dùng tạm trước đây tự chuyển về trang chính.
