# **BÀI TẬP CHƯƠNG II**
> Trong phần này, sẽ có một số bài sử dụng ngẫu nhiên để lấy kết quả. Và vì là ngẫu nhiên nên mỗi lần sẽ đều khác nhau.Để hạn chế tình huống này chúng có thể dùng `set.seed(42)` để các kết quả random có thể lặp lại được. Lưu ý `set.seed()` đặt các kết quả ngẫu nhiên theo thứ tự. Tức là lần gọi ngẫu nhiên đầu tiên sau khi `set.seed` sẽ luôn cho kết quả giống nhau, nhưng nếu ta thay đổi chạy câu lệnh thứ 2 trước câu lệnh thứ 1 thì sẽ có kết quả khác. Số 42 được gọi là *seed* ta có thể thay đổi bất cứ số nào tùy thích miễn là dễ nhớ.


## **Dễ**

1. Viết hàm `tong_hai_so(a, b = 10)` tính tổng hai số. Gọi hàm với cả hai tham số và chỉ với tham số bắt buộc.

2. Viết hàm `binh_phuong(x, y)` trả về bình phương của `x` cộng với bình phương của `y`. Gọi hàm với `x = 4` và `y = 5`.

3. Sử dụng hàm `abs()`, `sqrt()` và `round()` với các giá trị `-7`, `16` và `5.6`.

## **Trung bình**

4. Viết hàm `tong_nhieu_so(...)` tính tổng nhiều số bất kỳ. Thử với các số `1,2,3,4,5`.

5. Tạo ma trận `mat_a <- matrix(c(2, 1, 3, 4), 2, 2)`. Tính chuyển vị và định thức.

6. Sinh 10 số ngẫu nhiên từ phân phối chuẩn với `mean = 0.5`, `sd = 0.5` và tính trung bình của chúng bằng `mean()`.

## **Khó**

7. Sinh 10 số ngẫu nhiên từ phân phối nhị thức `size = 20`, `prob = 0.3`. Tính tổng và trung bình các giá trị.

8. Sinh 5 số từ phân phối Poisson với `lambda = 3` và 5 số từ phân phối đều trên \[0,10]. Kết hợp thành một vector và tính `min()`, `max()`, `length()`.

9. Tạo vector `x <- c(4, 1, 5, 7, 2, 3, 6, 9)`. Sắp xếp vector, tính tổng, tích và số phần tử.

## **Rất khó**

10. Viết hàm `phan_tich_vector(v)` nhận một vector số nguyên. Hàm trả về list gồm:

* vector các số chẵn
* vector các số lẻ
* bình phương các số chẵn
* tổng các số lẻ

Gọi hàm với `v <- 1:20` và in kết quả.