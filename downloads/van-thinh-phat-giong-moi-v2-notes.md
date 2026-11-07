# Vạn Thịnh Phát — thay lời đọc bằng MP3 1103 (V2)

Đây là bản cập nhật audio cho phim 11 phút, không tạo hoặc nhân bản giọng mới. Giọng đọc lấy trực tiếp từ file 1103.MP3 người dùng cung cấp (660.401625 giây). Giữ nguyên cao độ và tốc độ bản đọc; chỉ đổi định dạng, trộn SFX giấy nhẹ và chặn đỉnh nếu cần. Không trộn lại bất kỳ giọng Piper cũ nào.

Nhận dạng tiếng Việt cục bộ bằng sherpa-onnx Zipformer VI 30M INT8 để đối chiếu: 2723/2769 đơn vị từ của script khớp (98.3%). Các khác biệt gồm lỗi nhận dạng và có thể có khác biệt lời đọc; tỷ lệ này không phải xác minh nội dung pháp lý. Mốc đầu 40 cảnh lệch tối đa 0.16 giây so với hình, nên giữ nhịp chuyển động gốc. Phụ đề 333 mục được căn lại theo mốc từ nhận dạng, giữ văn bản gốc để tránh đưa lỗi ASR vào tên và thuật ngữ. Nên nghe soát thủ công nếu cần bản chép nguyên văn tuyệt đối.

Các phụ đề cũ đã burn-in được che ở dải riêng 875–990 px, dưới nội dung chính; lớp phụ đề mới nằm trong cùng vùng. Sử dụng nguồn hình 15 fps gốc, xuất 30 fps như bản trước. Giữ khung cuối thêm khoảng 0.43 giây để chứa đủ MP3. SFX tổng hợp cũ được giữ nhỏ hơn, không sử dụng audio có giọng cũ của MP4 trước.

Đầu ra: van-thinh-phat-11min-giong-moi-v2.mp4 và van-thinh-phat-phu-de-giong-moi-v2.srt. Không xác nhận file MP3 được tạo bằng ElevenLabs hay là giọng người thật; nguồn audio do người dùng cung cấp. Các giới hạn đối chiếu số liệu và bối cảnh pháp lý của bản dựng gốc vẫn áp dụng.
