# CAPSTONE-PRINTING-MANAGEMENT---2025F_C1SE.87
A web-based Printing Management System for organizations to manage print jobs, track costs, optimize resources, and provide secure user access.

## PROJECT STRUCTURE ##
project-root/
│
├── backend/                         # Java (API + DB)
│   ├── controllers/                 # REST API
│   │   ├── auth/                    # Login, Register
│   │   ├── customer/                # API cho khách hàng
│   │   ├── staff/                   # API cho nhân viên
│   │   └── owner/                   # API cho chủ cửa hàng
│   ├── services/                    # Xử lý logic (thanh toán, thông báo…)
│   ├── models/                      # Entity (ánh xạ bảng MySQL)
│   └── repositories/                # Truy vấn DB (JPA/Hibernate)
│
├── frontend/                        # ReactJS
│   ├── pages/
│   │   ├── auth/                    # Login, Register (dùng chung)
│   │   ├── customer/                # UI khách hàng (đặt đơn, thanh toán, theo dõi)
│   │   ├── staff/                   # UI nhân viên (nhận đơn, cập nhật tiến độ)
│   │   └── owner/                   # UI chủ cửa hàng (dashboard, doanh thu)
│   ├── components/                  # Component chung (navbar, footer, form…)
│   └── api/                         # Gọi API backend
│
├── docs/                            # Tài liệu (ERD, use case, phân công task)
├── .env                             # Config (DB_URL, VNPay_KEY…)
└── README.md                        # Hướng dẫn dự án

## PROJECT STRUCTURE ##