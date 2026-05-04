# ☁️ Cloud Infrastructure & Data Pipeline

Thư mục này quản lý toàn bộ hạ tầng triển khai và quy trình xử lý dữ liệu lớn (Big Data Pipeline) phục vụ cho bài toán làm giàu dữ liệu và huấn luyện mô hình y tế.

---

## 🏗 1. Deployment Architecture

Hệ thống được thiết kế theo kiến trúc Microservices để đảm bảo tính linh hoạt và khả năng mở rộng:

- **Containerization**: Sử dụng **Docker** để đóng gói toàn bộ dịch vụ từ Backend (Spring Boot), Frontend (React) đến các module Machine Learning.
- **Orchestration**: Triển khai trên cụm **Kubernetes** nhằm quản lý việc tự động điều phối và phục hồi các dịch vụ.
- **CI/CD**: Tích hợp quy trình kiểm tra mã nguồn (Checkstyle) và tự động hóa triển khai qua **GitHub Actions**.

## 🌊 2. Big Data & Machine Learning Pipeline

Hệ thống triển khai một Pipeline dữ liệu toàn diện để phục vụ thực nghiệm các thuật toán Stacking và SVM-SMOTE:

- **Data Ingestion**: Sử dụng **Apache Kafka** (triển khai bằng Python) để thu thập và điều phối dòng dữ liệu từ hệ thống quản lý phòng mạch theo thời gian thực.
- **Storage (Data Lake)**: Dữ liệu thô và dữ liệu sau xử lý được lưu trữ tập trung trên **Amazon S3**.
- **Processing (ETL)**: **Apache Spark** thực hiện các tác vụ biến đổi dữ liệu lớn, làm sạch và áp dụng kỹ thuật cân bằng dữ liệu.
- **Orchestration**: Toàn bộ luồng dữ liệu được điều phối tự động bởi **Apache Airflow**, đảm bảo tính nhất quán giữa các bước xử lý.
- **MLOps**: Tích hợp hệ thống theo dõi và tái huấn luyện mô hình tự động, giúp duy trì hiệu năng của hệ thống trong môi trường thực tế.

## 🛠 3. Technology Stack

| Thành phần              | Công nghệ sử dụng                         |
| :---------------------- | :---------------------------------------- |
| **Infrastructure**      | Docker, Kubernetes, Terraform             |
| **Data Lake & Storage** | Amazon S3, PostgreSQL                     |
| **Data Processing**     | Apache Spark, Apache Kafka (Python)       |
| **Workflow Manager**    | Apache Airflow                            |
| **Machine Learning**    | Scikit-learn (SVM-SMOTE, Stacking), MLOps |
