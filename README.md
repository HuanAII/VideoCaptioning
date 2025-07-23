# VideoCaptioning

# Tổng quan dự án : 
Mục tiêu : Cho một video đầu vào , mô hình sẽ sỉnha mô tả dạng văn bản bằng tiếng Anh ( hoặc tiếng Việt nếu bạn muốn fine-tune)

* Pipe line :
Video (dạng .mp4) → Trích khung hình → CNN (trích đặc trưng) → LSTM (sinh chú thích) → Câu mô tả (caption)


1. THU THẬP VÀ XỬ LÝ DỮ LIỆU
   1.1 Chọn hoặc tải bộ dữ liệu :
   MSVD (Microsoft Research Video Description Corpus): khoảng 2000 video, mỗi video có nhiều mô tả.

   1.2 Tiền xử lý video :
   Cắt video thành khung hình mỗi 1-2 giây -> résize ảnh về cùng kích thước ( 224x224 cho ResNet ) -> lưu dạng tensor
   
2. TRÍCH XUẤT ĐẶC TRỪNG BẰNG CNN
3. XỬ LÝ MÔ TẢ VĂN BẢN (CAPTION)
4. XÂY DỰNG MÔ HÌNH CAPTIONING
5. KIỂM TRA VÀ ĐÁNH GIÁ 

