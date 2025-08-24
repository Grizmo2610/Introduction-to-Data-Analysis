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

> Hàm `unique(x)` dùng để trả về 1 vector chứa các giá trị riêng biệt và không lặp lại.


>> `colnames(data)` để lấy ra các cột của `data` tương ứng. Ta cũng có thể đổi tên các cột bằng cách gán `colnames(data) = <vector>`

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
   * Tính tổng thu nhập (`TotalPrice`) và trung bình số lượng của mặt hàng `Carrot` bán tại thành phố `Boston`.
   * Tính tổng số lượng sản phẩm theo từng thành phố.
   * Tìm thành phố có tổng doanh thu (`TotalPrice`) cao nhất.
   * Tìm sản phẩm nào chỉ xuất hiện ở đúng một thành phố.

5. Từ dữ liệu **melb_data.csv**, thực hiện:
   * Thay thế các dữ liệu NA ở cột `Car` bằng giá trị 0
   * Thay thế dữ liệu NA ở cột `BuildingArea` bằng giá trị trung bình và cột `YearBuilt` bằng giá trị ngẫu nhiên theo phân bố đều với `min` và `max` của cột `YearBuilt` (Làm tròn thành số nguyên)
   * Trích xuất các căn giá có giá rẻ nhất trong các khu vực (`Regionname`)

6. Từ dữ liệu **AHCAvote2017** trong Gói `Stat2Data`
   * Hãy tìm số thành viên của quốc hội theo từng bang
   * Hãy tìm tổng số thành viên theo đảng Dân chủ (`Democrat`) và đảng Cộng hòa (`Republican`)
   * Hãy tìm khu vực (`STATE`) có tỷ lệ người dân không có bảo hiểm y tế ít nhất và nhiều nhất năm 2013 và 2015 (Mỗi dòng tương ứng với 1 đơn vị. Tất cả các dòng có chung giá trị `STATE` được tính là 1 khu vực. Tỷ lệ khu vực ở đây sẽ là trung bình giữa các đơn vị)

---

### **Mức khó**

7. Từ dữ liệu **WHO1.xlsx**, thực hiện:
   * Nhập dữ liệu vào R, thay thế giá trị trống bằng **mean** của Châu lục/ Vùng kinh tế.
   * Tính tuổi thọ trung bình của toàn bộ dữ liệu và So sánh tuổi thọ trung bình của nhóm "quốc gia phát triển" và "chưa phát triển".
   * Trích dữ liệu của các nước `Vietnam`, `Thailand`, `Singapore` và so sánh tỷ lệ sinh sản. (Gợi ý: Sử dụng `data$Country` để xem tên tất cả các nước trong dữ liệu)
   * Viết một hàm tìm ra 5 quốc gia có tuổi thọ cao nhất.

|-------------------------|-----------------|--------------------------|
| Nhóm quốc gia           | GNI/người (USD) | Diễn giải chung          |
|-------------------------|-----------------|--------------------------|
| Thu nhập thấp           | ≤ 1.145         | Quốc gia kém phát triển  |
| Thu nhập trung bình thấp| 1.146 – 4.515   | Đang phát triển (thấp)   |
| Thu nhập trung bình cao | 4.516 – 14.005  | Đang phát triển (cao)    |
| Thu nhập cao            | ≥ 14.006        | Quốc gia phát triển      |
|-------------------------|-----------------|--------------------------|

8. Từ dữ liệu **BirdNest** trong `Stat2Data`:
   * Xây dựng bảng tần số về số loài chim theo từng loại tổ (`Nesttype`)
   * Loài chim nào có chiều dài trung bình lớn nhất, nhỏ nhất?
   * Xây dựng bảng tần số về vị trí làm tổ của các loài chim
   * Hãy tính thời gian trung bình các loài chim này chăm sóc chim non trong tổ
