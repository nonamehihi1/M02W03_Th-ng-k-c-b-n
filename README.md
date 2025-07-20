# M02W03_Basic_Statistic
Thống kê cơ bản và Ứng dụng correlation coefficient


Median
- Trung vị, dùng làm ảnh bị nhiễu (denoise)

Mean, Expected Value
- Mean là tính giá trị trung bình sau khi đã thu thập dữ liệu, còn Expected Value là giá trị mong muốn trước khi thu thập dữ liệu
+ Tính theo Population: tính trung bình trên toàn bộ tập dữ liệu
+ Tính theo Sample: Tính trung bình trên 1 tập nhỏ dữ liệu, ví dụ muốn tính trung bình chiều cao của 1 đất nước, rất khó có thể thu thập hết toàn bộ dữ liệu và tính trung bình, thay vào đó ta có thể tính trung bình trong 1 tập dữ liệu nhỏ hơn(như là 100k người thay vì 100 tr người)

Find the mean Z that minimizes the variance: 
<img width="1205" height="677" alt="image" src="https://github.com/user-attachments/assets/ec2b1691-7979-40db-8ea8-6c85dbd8ce95" />
- Như ở hình trên ta có cách chứng minh công thức tìm mean z từ đạo hàm của variance = 0 để Variance nhỏ nhất

Thường thì giá trị của Variance của Sample Mean sẽ nhỏ hơn so với Variance của Population Mean, vậy ta cần làm gì để giá trị Var của Sample Mean gần lại hơn với Population Mean:
<img width="317" height="65" alt="image" src="https://github.com/user-attachments/assets/73086caa-73ff-49cb-ba68-434fed494b66" />
- Là ta sẽ chia cho mẫu để làm tăng giá trị lên, thay vì là 'n' ta sẽ sửa thành 'n-1'

Tại sao công thức tính Variance(phương sai) của Sample Mean lại là 'n-1' chứ không phải 'n-2' hay 'n-3':
- Chúng ta sẽ lấy ví dụ như sau: có 2 người, 1 người tung xúc sắc, 1 người đoán mặt xúc sắc, nếu người tung nói không phải mặt 1 2 3 4 5, thì người còn lại có thể dễ dàng đoán được mặt còn lại chắc chắn là số 6, ta có thể thấy giá trị cuối cùng không thể là số khác ngoài những số đã chọn, vậy nên giá trị cuối cùng là cố định và không còn độc lập nữa, thêm ví dụ nữa, mean = 5, ta có 4 5 x, thì chắc chắn x sẽ là 6 mà không phải số nào khác
<img width="292" height="161" alt="image" src="https://github.com/user-attachments/assets/f73da389-d138-4871-aaf9-a5142a7358f6" />

Variance, Standard devation


Ứng dụng Variance sử dụng để làm nổi bật shape của bức ảnh

PMF: Discrete
+ Ví dụ như tung xúc xắc
PDF: Continous
CDF: Discrete và Continous

Correlation: Tương quan
- Tương quan giữa 2 biến:
<img width="630" height="308" alt="image" src="https://github.com/user-attachments/assets/23c52b52-8ee7-42fc-a1f4-b87e9e799577" />

- Covariance giữa 2 biến X và Y được tính bằng công thức:
<img width="347" height="90" alt="image" src="https://github.com/user-attachments/assets/b6c5cf04-9973-4610-96cf-2df5be166e1b" />

+ Cov > 0: Khi X tăng và Y tăng ==> MQH thuận chiều
+ Cov < 0: Khi X tăng mà Y giảm ==> MQH nghịch chiều

Covariance: Hiệp phương sai 

Corelation Coeficient: 
- Giá trị Covariance không được chuẩn hóa, nên nó phụ thuộc vào đơn vi đo của 2 biến, ví dụ giữa chiều cao(Cm) và cân nặng(kg) = 120, nhưng khi đổi Cm -> M thì Covariance != 120, vì vậy ta sẽ sử dụng Correlation Coeficient
<img width="171" height="84" alt="image" src="https://github.com/user-attachments/assets/fb78ec02-ea0f-48ab-9d40-c054f04150d2" />

Nhưng công thức trên là công thức lý thuyết, đúng cho Population, nhưng thực tế khi tính từ dữ liệu mẫu(sample) sẽ như sau: 

<img width="484" height="121" alt="image" src="https://github.com/user-attachments/assets/62dc67ed-490d-4075-ac11-5bc28063e8e7" />




