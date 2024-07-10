# Đồ án: 
Trong vài năm gần đây, hệ thống nhận dạng cử chỉ bàn tay đã được chú ý rất nhiều vì khả năng tương tác với máy tính hiệu quả. Sử dụng cử chỉ
giúp cho việc tương tác giữa con người và máy tính trở nên dễ dàng,
thuận tiện và thú vị. Bằng chứng là ngày nay cử chỉ tay được sử dụng để
điều khiển các ứng dụng khác nhau như điều khiển robot, điều khiển TV
thông minh, chơi game, ... Cùng với sự phát triển mạnh mẽ của các hệ
thống đó, ngày càng có nhiều thiết bị mới trong lĩnh vực nhận dạng cử
chỉ ngày càng phổ biến và thành công. Do đó, trong đề tài này đã đưa ra
ý tưởng điều khiển các slide trong khi trình chiếu bằng hệ thống nhận
dạng cử chỉ tay sử dụng công nghệ Hand Tracking.

# Cài đặt
- Thư viện sử dụng: Thư viện OpenCV
OpenCV được xây dựng để cung cấp một cơ sở hạ tầng chung cho các ứng dụng thị giác
máy tính và để đẩy nhanh việc sử dụng nhận thức máy trong các sản phẩm thương mại.
Là một sản phẩm được cấp phép BSD, OpenCV giúp các doanh nghiệp dễ dàng sử dụng
và sửa đổi mã.
Cấu hình hệ thống:
- Hệ điều hành:
   + Ubuntu 14 hoặc ubuntu 16
   +  Windown 8 hoặc windown 10.
   + Mac OSX Maverichs và các phiên bản khác (trên tất cả các version CPU)
   + Cấu hình hệ thống (Cấu hình tiêu chuẩn) :
   + Nvidia GPU version: NVIDIA graphics card with at least 1.6 GB and At least 2.5 GB of free RAM memory for BODY_25 model or 2 GB for COCO.
Highly recommended: cuDNN.
   + AMD GPU version: Vega series graphics card. At least 2 GB of free RAM
memory.
   + CPU version: Around 8GB of free RAM memory.
  
# Giới thiệu:
Một thuật toán dựa trên chuyển động được sử dụng để phát hiện và theo dõi
bàn tay con người. Sau đó, các đường viền bàn tay được trích xuất và mô tả bằng
các vectơ đặc trưng bất biến về chiếu sáng, xoay và tỷ lệ. Sau đó, Logistic
regression và Multilayer perceptron classification được sử dụng cho tư thế tay và
nhận dạng cử chỉ tay động. Trong ứng dụng điều khiển thuyết trình, năm cử chỉ
được nhận dạng được sử dụng để di chuyển tới slide tiếp theo hoặc lùi về slide
trước đó, show pointer, highlight bản trình chiếu và xóa highlight.

## DEMO:
![Webcam](https://github.com/HungPham2002/Hand-Gesture-Controlled-Presentation/blob/main/presentation/22.png)
