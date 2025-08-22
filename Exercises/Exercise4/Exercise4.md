## **BÀI TẬP CHƯƠNG III**

### **Mức dễ**

1. Sinh ra một bộ dữ liệu điểm của sinh viên 2345 hàng và bao gồm: mã sinh viên được đánh số từ 0001 đến 2345. Sử dụng phân bố đều sinh ngẫu nhiên điểm thường xuyên, điểm giữa kỳ, điểm cuối kỳ.

   * Tính điểm trung bình theo công thức 20-20-60 và ghép vào dữ liệu ban đầu.
   * Phân loại thành điểm chữ và ghép vào dữ liệu ban đầu.

2. Sinh dữ liệu 1000 nhân viên với các thông tin: `ID`, `Tuổi` (18–60), `Giới tính` (Nam/Nữ), `Lương cơ bản` (tạo ngẫu nhiên từ 5 triệu đến 20 triệu).

   * Tính tổng thu nhập theo công thức: Lương cơ bản + 10% phụ cấp.
   * Phân nhóm nhân viên thành “Thu nhập thấp” (<8 triệu), “Trung bình” (8–15 triệu), “Cao” (>15 triệu).

3. Tạo một dữ liệu bán hàng 500 dòng gồm: `Mã đơn hàng`, `Ngày bán` (ngẫu nhiên trong năm 2023), `Sản phẩm` (5 loại khác nhau), `Số lượng` (1–20), `Đơn giá` (tạo ngẫu nhiên từ 10 đến 100).

   * Tính `Doanh thu = Số lượng × Đơn giá`.
   * Lọc ra các đơn hàng có doanh thu lớn hơn 1000.

---

### **Mức trung bình**

4. Dữ liệu **Product.csv** có 24 hàng và 8 biến, đọc tệp đã cho và đặt tên nó là `data`. Thực hiện:

   * Trích ra bộ dữ liệu con gồm các mặt hàng được bán tại thành phố `Boston` và đặt tên nó là `data1`.
   * Tính tổng giá của mặt hàng `Carrot`.
   * Tính trung bình số lượng sản phẩm `Carrot` bán tại thành phố `Boston`.

5. Từ dữ liệu **Product.csv**, thực hiện:

   * Đếm số loại mặt hàng khác nhau có trong dữ liệu.
   * Tìm thành phố có tổng doanh thu cao nhất.
   * Tìm sản phẩm nào có số lượng bán ra trung bình lớn nhất.

6. Với dữ liệu **Product.csv**:

   * Tính tổng số lượng sản phẩm theo từng thành phố.
   * Tìm sản phẩm nào chỉ xuất hiện ở đúng một thành phố.
   * Thêm một biến mới `Doanh thu = Giá × Số lượng`. Xuất ra 5 dòng có doanh thu cao nhất.

---

### **Mức khó**

7. Từ dữ liệu **WHO1.xlsx** (195 quốc gia), thực hiện:

   * Nhập dữ liệu vào R, thay thế giá trị trống bằng median của Châu lục/ Vùng kinh tế.
   * Tính tuổi thọ trung bình của toàn bộ dữ liệu.
   * So sánh tuổi thọ trung bình của nhóm “quốc gia phát triển” và “chưa phát triển”.

8. Với dữ liệu **WHO1.xlsx**:

   * Trích dữ liệu của các nước `Vietnam`, `Thailand`, `Singapore` và so sánh tỷ lệ sinh sản.
   * Viết một hàm tìm ra 5 quốc gia có tuổi thọ cao nhất.
   * Viết một hàm khác tìm 5 quốc gia có tuổi thọ thấp nhất.

9. Với dữ liệu **WHO1.xlsx**:

   * Tính phân phối số lượng quốc gia theo từng nhóm phân loại (Phát triển, Đang phát triển, Chưa phát triển, Khác).
   * Vẽ biểu đồ cột thể hiện phân phối này.
   * Vẽ thêm biểu đồ hộp (boxplot) so sánh tuổi thọ theo từng nhóm.

10. Với dữ liệu **WHO1.xlsx**:

    * Viết hàm nhận đầu vào là một quốc gia, trả về toàn bộ thông tin (GNI, tuổi thọ, tỷ lệ sinh sản, dân số, nhóm).
    * Viết hàm nhận đầu vào là một nhóm (ví dụ “Phát triển”) và trả về quốc gia có tuổi thọ cao nhất trong nhóm đó.
    * Sử dụng hai hàm trên với dữ liệu thực tế.
