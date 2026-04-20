# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX  |Đúng, giữ khoảng trắng  |
| hello world | 5 |mjqqt btwqi | Đúng, xử lý chữ thường |
| LORYH BRX | 3 | I LOVE YOU   | Đúng, giải mã chính xác |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 |ILV O OEYU | Đúng, zigzag 2 dòng |
| I LOVE YOU | 4 |IY LOEOVU  | Đúng, phân bổ theo 4 rails  |
| IOEOLVYU | 2 |I LOVE YOU |  Đúng, giải mã chính xác |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ:
 - Ký tự đặc biệt → bị từ chối
  - Số → bị từ chối
- Kết quả đọc từ `data/input.txt`:
Message from file: I LOVE YOU
Enter rails: 2
Ciphertext: ILV O OEYU

## 4. Kết luận

Qua bài lab, em hiểu rõ hơn về cách hoạt động của các phương pháp mã hóa cổ điển, đặc biệt là sự khác biệt giữa phép thế (Caesar Cipher) và phép hoán vị (Rail Fence Cipher). Khó khăn lớn nhất là xử lý phần giải mã của Rail Fence Cipher do cần xác định đúng vị trí ký tự trong mô hình zigzag. Tuy nhiên, nhờ việc chạy thử nhiều test case và kiểm tra từng bước, em đã nắm vững cách triển khai và cải thiện kỹ năng lập trình cũng như tư duy thuật toán.
