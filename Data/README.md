# **Bộ dữ liệu: `Product.csv`**

##  **Mô tả**

Dữ liệu `Product.csv` chứa thông tin đơn hàng với các cột:

* **OrderDate**: ngày đặt hàng
* **Region**: khu vực bán hàng
* **City**: thành phố
* **Category**: loại sản phẩm
* **Product**: tên sản phẩm
* **Quantity**: số lượng bán
* **UnitPrice**: giá 1 sản phẩm
* **TotalPrice**: tổng giá trị đơn hàng (`Quantity * UnitPrice`)

Mỗi dòng tương ứng một đơn hàng, có thể dùng để phân tích doanh số theo sản phẩm, loại, thành phố hoặc khu vực.

## **Được sử dụng trong bài**
* [Chapter 4 - Nhập xuất dữ liệu](../Chapters/Chapter4.ipynb#nhập-xuất-dữ-liệu)
* [Exercise 4 - Bài 4](../Exercises/Exercise4/Exercise4.md)

---

# **Bộ dữ liệu: `WHO1.xlsx`**

## **Mô tả**
Dữ liệu `WHO1.xlsx` chứa thông tin các quốc gia với các cột:

* **Country**: tên quốc gia
* **Region**: khu vực (châu lục hoặc vùng kinh tế)
* **Population**: tổng dân số (nghìn người)
* **Under15**: tỷ lệ dân số dưới 15 tuổi (%)
* **Over60**: tỷ lệ dân số trên 60 tuổi (%)
* **FertilityRate**: tỷ lệ sinh trung bình
* **LifeExpectancy**: tuổi thọ trung bình
* **ChildMortality**: tỷ lệ tử vong trẻ em (trên 1.000 trẻ em)
* **LiteracyRate**: tỷ lệ biết chữ (%)
* **GNI**: thu nhập quốc dân bình quân đầu người (USD)

---

## **Được sử dụng trong bài**
* [Chapter 4 - Nhập xuất dữ liệu](../Chapters/Chapter4.ipynb#nhập-xuất-dữ-liệu)
* [Exercise 4 - Bài 7](../Exercises/Exercise4/Exercise4.md)


---

# **Bộ dữ liệu: `mtcars.csv` và `mtcars.xlsx`**

---

## **Mô tả**
Dữ liệu `mtcars.csv` và `mtcars.xlsx` chứa thông tin đặc tính và hiệu suất của các mẫu xe với các cột:

* **mpg**: số dặm xe đi được trên 1 gallon nhiên liệu
* **cyl**: số xy-lanh của động cơ
* **disp**: dung tích xi-lanh (cubic inches)
* **hp**: công suất động cơ (horsepower)
* **drat**: tỉ số truyền cầu sau
* **wt**: trọng lượng xe (1.000 lbs)
* **qsec**: thời gian hoàn thành 1/4 dặm (giây)
* **vs**: loại động cơ (0 = V-shaped, 1 = thẳng)
* **am**: loại hộp số (0 = tự động, 1 = số sàn)
* **gear**: số bánh răng
* **carb**: số bộ chế hòa khí (carburetor)

---

## **Được sử dụng trong bài**
* [Chapter 4 - Nhập xuất dữ liệu](../Chapters/Chapter4.ipynb#nhập-xuất-dữ-liệu)

---
# **Bộ dữ liệu: `melb_data.csv`**

## **Mô tả**

Dữ liệu `melb_data.csv` chứa thông tin về giá nhà và đặc tính của bất động sản tại thành phố Melbourne với các cột:

* **Suburb**: Tên khu vực/ngoại ô
* **Address**: Địa chỉ cụ thể của bất động sản
* **Rooms**: Số lượng phòng
* **Type**: Loại bất động sản (h = house, u = unit, t = townhouse, …)
* **Price**: Giá bán bất động sản (AUD)
* **Method**: Phương thức bán (S = Sold, SP = Sold prior, PI = Passed in, VB = Vendor bid, …)
* **SellerG**: Tên công ty/cá nhân môi giới
* **Date**: Ngày bán
* **Distance**: Khoảng cách từ bất động sản đến trung tâm thành phố (km)
* **Postcode**: Mã bưu điện của khu vực
* **Bedroom2**: Số phòng ngủ (ghi nhận)
* **Bathroom**: Số phòng tắm
* **Car**: Sức chứa bãi đỗ xe (số xe hơi)
* **Landsize**: Diện tích đất (m²)
* **BuildingArea**: Diện tích xây dựng (m²)
* **YearBuilt**: Năm xây dựng
* **CouncilArea**: Khu vực quản lý hành chính
* **Lattitude**: Vĩ độ vị trí bất động sản
* **Longtitude**: Kinh độ vị trí bất động sản
* **Regionname**: Tên vùng/khu vực lớn (ví dụ: Northern Metropolitan)
* **Propertycount**: Tổng số bất động sản được ghi nhận trong khu vực

---

## **Được sử dụng trong bài**

* [Chapter 4 - Xử lý dữ liệu bị thiếu](../Chapters/Chapter4.ipynb)
* [Exercise 4 - Bài 5](../Exercises/Exercise4/Exercise4.md)

---

# **Bộ dữ liệu: `AHCAvote2017.csv`**

---

## **Mô tả**

Dữ liệu `AHCAvote2017.csv` chứa thông tin về các Hạ nghị sĩ Hoa Kỳ và kết quả bỏ phiếu cho Đạo luật Chăm sóc Sức khỏe Mỹ năm 2017, với các cột:

* **STATE**: Tên bang
* **Dist**: Mã số đơn vị bầu cử (district)
* **Party**: Đảng phái của nghị sĩ (`R` = Cộng hòa, `D` = Dân chủ)
* **Dem**: Chỉ báo nghị sĩ thuộc Đảng Dân chủ (0 = Không, 1 = Có)
* **Rep**: Chỉ báo nghị sĩ thuộc Đảng Cộng hòa (0 = Không, 1 = Có)
* **uni2013**: Tỉ lệ không có bảo hiểm y tế tại đơn vị năm 2013
* **uni2015**: Tỉ lệ không có bảo hiểm y tế tại đơn vị năm 2015
* **uniChange**: Mức thay đổi tỉ lệ không có bảo hiểm y tế giữa 2013 và 2015
* **Member**: Tên nghị sĩ
* **AHCAvote**: Lá phiếu đối với AHCA (1 = Ủng hộ, 0 = Chống)
* **Trump**: Tỉ lệ phiếu bầu cho Donald Trump tại đơn vị trong bầu cử Tổng thống 2016

---

## **Được sử dụng trong bài**

* [Exercise 4 - Bài 6](../Chapters/Chapter4.ipynb)



---

# **Bộ dữ liệu: ``**

---

## **Mô tả**
Dữ liệu `` chứa thông tin:

---

## **Được sử dụng trong bài**