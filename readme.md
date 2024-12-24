1 Kiểm tra khả năng tương thích của GPU 

2 `nvidia-smi`

3  Tải Cuda toolkit với Cuda version bạn check được từ `nvidia-smi`

https://developer.nvidia.com/cuda-toolkit-archive

4 Tải CuDnn tương ứng với Cuda version bạn check được từ `nvidia-smi`

https://developer.nvidia.com/rdp/cudnn-archive

Sao chép các tệp từ thư mục bin cuDNN vào thư mục bin CUDA, sao chép các tệp từ thư mục cuDNN include vào thư mục include CUDA và cuối cùng, sao chép các tệp từ thư mục lib cuDNN vào thư mục lib CUDA. 

`LƯU Ý: Trong Windows 11, CUDA Toolkit có thể được tìm thấy theo đường dẫn sau: 'C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.x'`

5 Cài đặt TensorRT

https://developer.nvidia.com/tensorrt-download

Sao chép tất cả  các tệp dll (chỉ DLL!) từ thư mục lib TensorRT vào  thư mục bin CUDA .

6 Tải anaconda về để setup môi trường ảo

- Di chuyển đến từng thư mục TensorRT và cài đặt tất cả bằng Python pip:

`python -m pip install tensorrt_dispatch-8.6.1-cp311-none-win_amd64.whl`

`python -m pip install tensorrt-8.6.1-cp311-none-win_amd64.whl`

`python -m pip install tensorrt-8.6.1-cp311-none-win_amd64.whl`

LƯU Ý là đây chỉ là ví dụ, bạn cần check version của từng thư mục để cài đặt đúng version.

7 Tải pytorch về để setup môi trường ảo

https://pytorch.org/

`Tải phiên bản cuda dưới hoặc bằng với Cuda version gần nhất bạn check được`

` Nếu không chạy được thì cài đặt với phiên bản khác và không thấy Tensorrt thì nhúng DLL vào trong thư mục library của môi trường anaconda luôn`

Nếu bạn không chạy được thì có thể xem video hướng dẫn tại đây:

https://www.youtube.com/watch?v=WgPbbWmnXJ8&list=PLRt4lJgHZIbcKKXyyRQeOBhsokFakKg1r&index=6&ab_channel=Murtaza%27sWorkshop-RoboticsandAI

## Copyright
© 2024 [BaoHan1712]. All rights reserved.
