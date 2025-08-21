# **BÀI TẬP CHƯƠNG III**
## **Mức dễ**

1. Viết một đoạn mã kiểm tra xem số `x` có phải là số chẵn hay lẻ. In ra `"Chẵn"` hoặc `"Lẻ"`.

2. Tạo một vector `v <- c(-2, 5, 0, 3, -1)`. Sử dụng `ifelse()` để in `"Dương"` nếu phần tử > 0, `"Không dương"` nếu <= 0.

3. Viết chương trình nhập vào một số `x`. Sử dụng `if ... else if ... else` để phân loại:

   * `x < 0` → `"Âm"`
   * `x == 0` → `"Bằng 0"`
   * `x > 0` → `"Dương"`

## **Mức trung bình**

4. Tạo một vector `v <- c(3, 7, 12, 5, 9)`. Sử dụng vòng lặp `for` và `if` để in ra các số lớn hơn 6.

5. Viết chương trình tính tổng các số lẻ từ 1 đến 20 sử dụng vòng lặp `while`.

6. Sử dụng `switch()` để in tên môn học dựa vào biến `choice`:

   * `"1"` → `"Toán"`
   * `"2"` → `"Lý"`
   * `"3"` → `"Hóa"`
   * Khác → `"Môn không xác định"`

## **Mức khó**

7. Tạo một vector số ngẫu nhiên `x <- c(2, -5, 8, -1, 0)`. Viết vòng lặp `for` in `"Dương"` nếu phần tử > 0, `"Âm"` nếu < 0, `"Bằng 0"` nếu = 0.

8. Viết chương trình dùng vòng lặp `repeat` để in các số từ 1 đến 10. Dừng vòng lặp bằng `break`.

9. Tạo một vector `v <- c(1, 4, 7, 10, 13)`. Sử dụng vòng lặp `for` với `next` để in tất cả các số **trừ** số chia hết cho 2.

10. Viết một chương trình tổng hợp:

* Nhập vào một vector số.
* Kiểm tra từng phần tử:
   * Nếu > 0 in `"Dương"`
   * Nếu < 0 in `"Âm"`
   * Nếu = 0 in `"Bằng 0"`
* Tính tổng các số dương bằng vòng lặp `for`.