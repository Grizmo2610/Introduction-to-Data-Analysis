## **BÀI TẬP CHƯƠNG III**

>Ngoài cách sử dụng phân bố để sinh ngẫu nhiên dữ liệu. Ta cũng có thể sử dụng hàm `sample()` để sinh dữ liệu ngẫu nhiên

`sample(x, size, replace = FALSE, prob = NULL)`

* **x**: tập hợp giá trị để lấy mẫu (số, ký tự, v.v.)
* **size**: số lượng phần tử muốn lấy ra
* **replace**: `TRUE` thì lấy lặp lại được, `FALSE` thì không
* **prob**: vector xác suất tương ứng cho từng phần tử trong `x`

Ví dụ:

```r
age <- sample(18:60, 1000, replace = TRUE)
gender <- sample(c("Nam", "Nữ"), 1000, replace = TRUE)
```

* `18:60`: tập giá trị từ 18 đến 60 (tuổi)
* `c("Nam", "Nữ")`: tập giá trị giới tính
* `1000`: số lượng mẫu sinh ra
* `replace = TRUE`: cho phép trùng lặp khi chọn.



### **Mức dễ**

1. Sinh ra một bộ dữ liệu điểm của sinh viên 2345 hàng và bao gồm: mã sinh viên được đánh số từ 0001 đến 2345. Sử dụng phân bố đều sinh ngẫu nhiên điểm thường xuyên, điểm giữa kỳ, điểm cuối kỳ.

   * Tính điểm trung bình theo công thức 20-20-60 và ghép vào dữ liệu ban đầu.
   * Phân loại thành điểm chữ và ghép vào dữ liệu ban đầu.

| Điểm hệ 10 | Điểm chữ | Điểm hệ 4 |
|------------|----------|-----------|
| 9.0 - 10   | A+       | 4.0       |
| 8.5 - 8.9  | A        | 3.7       |
| 8.0 - 8.4  | B+       | 3.5       |
| 7.0 - 7.9  | B        | 3.0       |
| 6.5 - 6.9  | C+       | 2.5       |
| 5.5 - 6.4  | C        | 2.0       |
| 5.0 - 5.4  | D+       | 1.5       |
| 4.0 - 4.9  | D        | 1.0       |
| < 4.0      | F        | 0.0       |


2. Sinh dữ liệu 1000 nhân viên với các thông tin: `ID`, `Tuổi` (18–60), `Giới tính` (Nam/Nữ), `Lương cơ bản` (tạo ngẫu nhiên từ 5 triệu đến 20 triệu).

   * Tính tổng thu nhập theo công thức: Lương cơ bản + 10% phụ cấp.
   * Phân nhóm nhân viên thành "Thu nhập thấp" (<8 triệu), "Trung bình" (8–15 triệu), "Cao" (>15 triệu).

3. Tạo một dữ liệu bán hàng 500 dòng gồm: `Mã đơn hàng`, `Ngày bán` (ngẫu nhiên trong năm 2023), `Sản phẩm` (5 loại khác nhau), `Số lượng` (1–20), `Đơn giá` (tạo ngẫu nhiên từ 10 đến 100).

   * Tính `Doanh thu = Số lượng × Đơn giá`.
   * Lọc ra các đơn hàng có doanh thu lớn hơn 1000.

---

### **Mức trung bình**

4. Dữ liệu **Product.csv** có 24 hàng và 8 biến, đọc tệp đã cho và đặt tên nó là `data`. Thực hiện:
   * Trích ra bộ dữ liệu con gồm các mặt hàng được bán tại thành phố `Boston` và đặt tên nó là `data1`.
   * Tính tổng giá và trung bình số lượng của mặt hàng `Carrot` bán tại thành phố `Boston`.
   * Tìm thành phố có tổng doanh thu (`TotalPrice`) cao nhất.
   * Tính tổng số lượng sản phẩm theo từng thành phố.
   * Tìm sản phẩm nào chỉ xuất hiện ở đúng một thành phố.

5. Từ dữ liệu **melb_data.csv**, thực hiện:
   * Thay thế các dữ liệu NA ở cột `Car` bằng giá trị 0
   * Thay thế dữ liệu NA ở cột `BuildingArea` bằng giá trị trung bình và cột `YearBuilt` bằng giá trị ngẫu nhiên theo phân bố đều với `min` và `max` của cột `YearBuilt` (Làm tròn thành số nguyên)
   * Trích xuất các căn giá có giá rẻ nhất trong các khu vực (`Regionname`)
   * 


---

### **Mức khó**

7. Từ dữ liệu **WHO1.xlsx**, thực hiện:
   * Nhập dữ liệu vào R, thay thế giá trị trống bằng median của Châu lục/ Vùng kinh tế.
   * Tính tuổi thọ trung bình của toàn bộ dữ liệu và So sánh tuổi thọ trung bình của nhóm "quốc gia phát triển" và "chưa phát triển".
   * Trích dữ liệu của các nước `Vietnam`, `Thailand`, `Singapore` và so sánh tỷ lệ sinh sản.
   * Viết một hàm tìm ra 5 quốc gia có tuổi thọ cao nhất.

8. Với dữ liệu **WHO1.xlsx**:
