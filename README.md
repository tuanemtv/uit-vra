


## Yêu cầu ứng dụng
 Python 3.5, Tensorflow 1.2, Opencv 3.1

## Xây dựng bộ dữ liệu
- Dữ liệu train được xây dựng theo chuẩn của pascal với 2 classes: sếu đầu đỏ và sao la 
- Sử dụng công cụ [labelImg](https://github.com/tzutalin/labelImg) để tạo bộ dữ liệu train

 ![img](train_seu_dau_do.png)
- Toàn bộ dữ liệu train được lưu trong thư mục train/

## Train, test và sử dụng
Sử dụng mã nguồn [darkflow](https://github.com/thtrieu/darkflow) để kết hợp [Tensorflow](https://www.tensorflow.org/), [YOLO](https://pjreddie.com/darknet/yolo/) cho việc sử dụng Deep Learning trên bài toán nhận dạng thực thể trong hình ảnh và video

### Train

```bash
flow --model cfg/tiny-yolo-voc-2c.cfg --load bin/tiny-yolo-voc.weights --train --annotation train/Annotations --dataset train/Image
```
Kết quả log của quá trình train xem ở [train/train-log.txt](https://github.com/tuanemtv/uit-vra/blob/master/train/train-log.txt)

### Video

### Độ chính xác

 