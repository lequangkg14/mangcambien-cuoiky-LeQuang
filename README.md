# Đồ án: Nhận diện mệnh giá tiền Polymer Việt Nam bằng Công nghệ Edge AI

## 👤 Thông tin sinh viên thực hiện
| **Họ và tên Sinh viên** | Lê Quang |
| **Mã số Sinh viên (MSSV)**| N23DCCI062 |

---

## 📊 Thông số cấu hình & Hiệu suất mô hình
* **Độ phân giải ảnh đầu vào (Input Resolution):** 240 x 240 pixels (Tối ưu hóa chi tiết vùng biên)
* **Kiến trúc mạng:** FOMO (Backbone MobileNetV2 0.35)
* **Độ chính xác đạt được (F1 Score):** **85.2%**
* **Cấu hình xuất bản (Deployment):** Thư viện C++ (Quantized int8) tối ưu qua EON™ Compiler.
  * *Tài nguyên tiêu thụ:* RAM ~862.4 KB \| FLASH ~67.2 KB (Phù hợp cho các thiết bị nhúng phần cứng hạn chế).

---

## 🔗 Liên kết dự án (Project Links)
* **Link mã nguồn trên GitHub:** [https://github.com/lequangkg14/mangcambien-cuoiky-LeQuang]
* **Link dự án công khai trên Edge Impulse:** [https://studio.edgeimpulse.com/public/1019565/live]

---

## 📂 Cấu trúc thư mục dự án (Repository Structure)
Dự án được tổ chức khoa học theo cấu trúc chuẩn để giảng viên tiện theo dõi và đánh giá:

```text
├── 📑 Document/
│   └── báo cáo đồ án IOT.docx             # File báo cáo chi tiết 14 trang
└── 💻 Source_Code/                        # Toàn bộ mã nguồn C++ xuất từ Edge Impulse
    ├── edge-impulse-sdk/                  # Bộ thư viện lõi của Edge Impulse SDK
    ├── model-parameters/                  # Chứa tham số cấu hình trọng số mô hình
    ├── tflite-model/                      # File mô hình đã nén định dạng tflite (int8)
    ├── CMakeLists.txt                     # File cấu hình build mã nguồn
    └── README.txt                         # Hướng dẫn kỹ thuật từ Edge Impulse
