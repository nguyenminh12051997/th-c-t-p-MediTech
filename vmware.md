# Hướng dẫn sử dung máy ảo VMware

Đầu tiên, VMware Workstation là gì ?  VMware Workstation là chương trình giả lập máy tính, nó cho phép người dùng tạo nhiều máy tính ảo trên một máy tính vật lý. Các máy tính ảo này có đầy đủ các thiết bị phần cứng ảo và có thể hoạt động giống như một máy tính thật sự.

## Bước 1: Tạo máy ảo mới 

Chọn **create a new virtual machine**

## Bước 2: Cấu hình cho máy ảo 

<img src="https://psglee.files.wordpress.com/2015/07/next.png">

ở đây bạn thấy 2 lựa chọn là typical vào custom.   Nếu không cần thiết bị khác những thiết bị mặc định, chọn cấu hình mặc định cho máy ảo.

## Bước 3: Chọn ổ đĩa để cài đặt hệ điều hành 

<img src ="http://i.imgur.com/SaJSTlY.png">

trong này có 3 lựa chọn:

- cài hệ điều hành từ ổ đĩa
- cài hệ điều hành từ file .iso
- cài hệ điều hành sau 
  
Mình chọn cài sau...

## Bước 4: Chọn hệ điều hành sẽ được cài lên máy ảo

<img src="http://i.imgur.com/ZE3Nik1.png">

## Bước 5: Đặt tên vào vị trí lưu trong máy tính 

<img src="http://i.imgur.com/xTcuGRk.png">

## Bước 6: Chọn phần cứng cho máy ảo như processor, ram, card mạng 
trong đó có 3 loại card mạng: 

- Bridge:
 - Card Bridge trên máy ảo chỉ có thể giao tiếp với card mạng thật trên máy thật.
 - Card mạng Bridge này có thể giao tiếp với mạng vật lý mà máy tính thật đang kết nối.

- Host-only:
 - Card Host-only chỉ có thể giao tiếp với card mạng ảo VMnet1 trên máy thật.
 - Card Host-only chỉ có thể giao tiếp với các card Host-only trên các máy ảo khác.
 - Card Host-only không thể giao tiếp với mạng vật lý mà máy tính thật đang kết nối.

- NAT:
 - Card NAT chỉ có thể giao tiếp với card mạng ảo VMnet8 trên máy thật.
 - Card NAT chỉ có thể giao tiếp với các card NAT trên các máy ảo khác.
 - Card NAT không thể giao tiếp với mạng vật lý mà máy tính thật đang kết nối. Tuy nhiên nhờ cơ chế NAT được tích hợp trong VMWare, máy tính ảo có thể gián tiếp liên lạc với mạng vật lý bên ngoài.

**note** card NAT sau này sẽ dùng để tải các dịch vụ hay phần mềm về máy ảo còn cấu hình ta dùng thêm 1 card khác 

## Bước 7 : Select I/O Controller Types (Để mặc định)

Select a Disk Type: Nếu không phải đang lab liên quan đến ổ cứng, bạn nên để chế độ mặc định là SCSI

 ## Bước 8: Lựa chọn dung lượng phần cứng cho máy ảo 

Bạn có thể lựa chọn ổ cứng ổ sẽ lưu thành 1 file (Store virtual disk as a single file) hay tách ra làm nhiều file (Split virtual disk into multiple files)

<img src="http://i.imgur.com/hktx3vC.png">

Customize Hardware để sửa lại hoặc nhấn vào Finish để tạo máy ảo.
 <img src="http://i.imgur.com/5IuCJVy.png">

Sau khi máy ảo được tạo, như đã nói ở trên, bạn có thể chỉnh lại cấu hình phần cứng bằng cách vào Edit virtual machine settings. Bạn có thể thay đổi, thêm, bớt phần cứng như thêm ổ cứng, thêm card mạng thay đổi dung lượng Ram…



























