### Hướng dẫn cài đặt
#### Chuẩn bị
Phiên bản python sử dụng: 3.7.9, trình soạn thảo: VsCode
#### Cài đặt thư viện
+ Để tránh ảnh hưởng đến các thư viện python trên máy hiện tại, chúng ta nên tạo một môi trường riêng để chạy ứng dụng này
+ Tạo môi trường python riêng: py -m venv fsl
    + chúng có thể chỉ định 1 phiên bản python cụ thể nếu trên máy chúng ta có nhiều phiên bản: py -3.7 -m venv fsl
+ Kích hoạt môi trường vừa tạo: .\fsl\Scripts\activate
+ Sau khi cài đặt môi trường python thì tiến hành cài các thư viện cần file reqirements.txt
+ Nếu gặp lỗi liên quan đến torch lỗi vui lòng cài torch theo câu lệnh ở dưới sau (đây là phiên bản torch phù hợp với python 3.7.x):
pip install torch==1.10.1+cu113 torchvision==0.11.2+cu113 torchaudio===0.10.1+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html

#### Chạy app
py .\web_app.py
