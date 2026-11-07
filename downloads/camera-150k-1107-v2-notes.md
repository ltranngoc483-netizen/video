# Camera 150K — bản có lời đọc 1107.MP3

Bản hoàn chỉnh khoảng 60.07 giây, 15 cảnh, 1080×1920, H.264/AAC. Giọng lấy trực tiếp từ file 1107.MP3 (60.029375 giây) do người dùng cung cấp; không tạo, thay đổi cao độ hoặc thay đổi tốc độ giọng. SFX giấy được giữ nhỏ dưới lời đọc. Không xác nhận audio được tạo bởi ElevenLabs hoặc là giọng người thật.

ASR tiếng Việt cục bộ Zipformer VI 30M dùng để đối chiếu mốc đọc, khớp 175/180 đơn vị từ với script. Sai khác chủ yếu ở từ vay mượn như Wi-Fi, router, firmware, botnet; phụ đề giữ cách viết đúng từ brief. 38 cụm phụ đề được chia theo ý và lấy mốc từ từ ASR, kèm tô nền cyan từ đang đọc. Giữ 15 nhịp cảnh khoảng bốn giây vì audio phù hợp; camera xoay và khiên bảo vệ bám mốc từ liên quan. Hình stop-motion gốc 15 fps, xuất bản phân phối 30 fps lặp đôi khung.

Đây là mô hình giấy minh họa, không phải thử nghiệm một sản phẩm có giá 150K cụ thể. Camera tự xoay có thể là theo dõi chuyển động bình thường. UART thường cần tiếp cận vật lý; các rủi ro phụ thuộc thiết bị/cấu hình. CTA chỉ phù hợp khi người đăng đã gắn video dài thực sự về camera/bảo mật vào Related Video của YouTube.

`npm ci`; `npm run dev` (Studio 3008); `npm run check`. Source `Camera150K` có 901 khung/15 fps để chứa đủ cuối MP3. `scripts/finalize.py` trộn MP3 gốc với SFX nhẹ và xuất MP4. `scripts/validate.py` kiểm tra toàn bộ file và 15 cửa sổ audio. Các WAV/MP3 phải có trong public để dựng lại; font DejaVu có giấy phép đi kèm. Không dùng giọng TTS cục bộ cũ hoặc audio 1103.MP3 của phim Vạn Thịnh Phát.
