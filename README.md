ai-object-detection/
├── README.md                 # Mô tả tổng quan về dự án
├── requirements.txt          # Các thư viện cần thiết
├── .gitignore                # Danh sách file/thư mục cần bỏ qua khi push lên GitHub
├── config/                   # Thư mục cấu hình
│   ├── yolov5_config.yaml    # File cấu hình cho YOLOv5
│   ├── yolov8_config.yaml    # File cấu hình cho YOLOv8 (nếu cần)
│   └── ...                   # Các file cấu hình khác
├── data/                     # Thư mục chứa dữ liệu
│   ├── raw/                  # Dữ liệu gốc (chưa xử lý)
│   ├── processed/            # Dữ liệu đã qua tiền xử lý
│   ├── labels/               # File nhãn (annotations) cho từng ảnh
│   └── examples/             # Một số ảnh minh họa
├── notebooks/                # Thư mục chứa các file notebook
│   ├── data_preparation.ipynb # Tiền xử lý dữ liệu
│   ├── training.ipynb         # Huấn luyện mô hình
│   ├── evaluation.ipynb       # Đánh giá mô hình
│   └── inference.ipynb        # Triển khai dự đoán trên ảnh hoặc video
├── src/                      # Code chính của dự án
│   ├── train.py              # Script huấn luyện
│   ├── detect.py             # Script dự đoán thời gian thực
│   ├── utils.py              # Các hàm tiện ích (visualization, v.v.)
│   └── model/                # Thư mục chứa mã nguồn mô hình YOLO
│       ├── yolov5/           # YOLOv5
│       ├── yolov8/           # YOLOv8 (nếu cần)
│       └── ...
├── tests/                    # Thư mục kiểm thỬ
│   ├── test_data.py          # Unit tests cho việc tiền xử lý dữ liệu
│   ├── test_model.py         # Unit tests cho mô hình
│   └── test_inference.py     # Unit tests cho triển khai
├── outputs/                  # Thư mục lưu trữ kết quả
│   ├── checkpoints/          # File checkpoint mô hình (weights)
│   ├── logs/                 # File log huấn luyện
│   ├── predictions/          # Kết quả dự đoán (bounding boxes)
│   └── demo_videos/          # Video demo nhận dạng
└── docs/                     # Tài liệu dự án
    ├── project_overview.md   # Giới thiệu chi tiết dự án
    ├── setup_guide.md        # Hướng dẫn cài đặt
    ├── data_guide.md         # Hướng dẫn thu thập và gắn nhãn dữ liệu
    └── model_usage.md        # Hướng dẫn sử dụng mô hình