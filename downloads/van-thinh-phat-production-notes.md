# Vạn Thịnh Phát – SCB: Hồ sơ và dòng tiền

Bản dựng biên tập hoàn chỉnh 11 phút, 40 cảnh, 16:9, lời bình tiếng Việt, phụ đề và hiệu ứng âm thanh. Nguồn sáng tạo là brief người dùng. Remotion là bộ dựng, xuất hình 1920×1080 với nhịp stop-motion 15 fps; bản phân phối MP4 H.264/AAC là 30 fps bằng lặp đôi khung, không phải chuyển động gốc 30 fps. HyperFrames được dùng làm hướng dẫn thiết kế vật liệu, chuyển động và quy trình lời bình; dự án thực thi là React/Remotion, không phải HTML HyperFrames.

## Nội dung và giới hạn xác minh

Không đồng nhất tổng giải ngân với tiền chiếm đoạt hoặc thiệt hại. Đã bỏ so sánh một phần tư GDP thiếu năm. Tiền mặt hơn 108.000 tỷ được mô tả là tổng qua nhiều lần vận chuyển; 5,2 triệu USD là tổng tiền liên quan nhóm hành vi nhận hối lộ, không phải tất cả trong một thùng. Sơ đồ dùng người đứng tên và pháp nhân giả định để minh họa quan hệ, không giả mạo chứng cứ.

Truy cập báo chí trong môi trường này trả về lỗi chính sách mạng 403. Vì vậy không tuyên bố đã kiểm chứng độc lập các số liệu pháp lý hoặc cập nhật tình trạng tố tụng đến ngày xuất bản. Các mốc 91,5%, hơn 108.000 tỷ và 5,2 triệu USD phát triển từ brief và thông tin nền, phải đối chiếu nguồn tố tụng và báo chí đáng tin cậy trước khi phát hành như một phim điều tra đã kiểm chứng. Không dùng bộ phim như một bản cập nhật kết quả xét xử hiện tại.

## Audio và giấy phép

Không có công cụ/credential ElevenLabs trong phiên. Giọng đọc là Piper `vi_VN-vais1000-medium`, chạy cục bộ bằng sherpa-onnx 1.12.26; giọng gốc thiên nữ, chưa đáp ứng yêu cầu giọng nam ElevenLabs trầm trong brief. Không gắn nhãn Marcus hoặc giọng VTV. Mỗi câu được tạo riêng, bỏ đệm, chuẩn hóa và điều chỉnh tempo giữ cao độ để khớp cửa sổ cảnh. Các WAV hiện có đủ để xuất lại, không cần tải mô hình.

Attribution: VAIS-1000 Vietnamese speech synthesis corpus / VAIS contributors; Piper vi_VN-vais1000-medium model; distribution by k2-fsa/sherpa-onnx. Model card: public/licenses/Vietnamese-voice-MODEL_CARD.txt. Dataset link https://ieee-dataport.org/documents/vais-1000-vietnamese-speech-synthesis-corpus . License https://creativecommons.org/licenses/by/4.0/ . Mô hình tải từ https://github.com/k2-fsa/sherpa-onnx/releases/download/tts-models/vits-piper-vi_VN-vais1000-medium.tar.bz2 . Thay đổi: tách câu, cắt đệm, chuẩn hóa loudness, thay đổi tempo. Không dùng các mô hình VIVOS phi thương mại hoặc 25hours có giấy phép chưa rõ trong thành phẩm.

DejaVu Sans/DejaVu Sans Bold có giấy phép đi kèm trong public/licenses. Các hình ngân hàng, xe và sổ giấy được tạo bằng AI cho dự án. Đồ họa và hiệu ứng âm thanh được lập trình riêng; không có nhạc thương mại hay chân dung người thật.

## Dựng và xuất

`npm ci`; `npm run check`; `npm run dev` (Studio 3006).

Composition `VanThinhPhat`: 1920×1080, 15 fps, 9900 frames / 660 giây. `ScenePreview` có prop index để xem riêng từng cảnh. Mỗi cảnh có một JSX Sequence riêng trong Video.tsx. Nội dung, thời gian câu và tempo nằm trong src/story.json; phụ đề Caption JSON trong src/captions.json; toàn bộ kịch bản có SFX và image prompts trong KICH-BAN.md.

Render native: `npx remotion render src/index.ts VanThinhPhat out/van-thinh-phat-native-15fps.mp4 --muted --codec=h264 --crf=25`.

Tạo audio master: chạy scripts/sound.py bằng Python có numpy/soundfile. Đóng gói 30 fps và validate bằng các script cùng thư mục. Mô hình giọng đọc, node_modules và cache không được đóng gói.
