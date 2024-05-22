# Tạo môi trường ảo với conda

## 1. Để tạo môi trường ảo với conda, chúng ta sử dụng lệnh sau:

```bash
conda create --name <Tên môi trường>
```

## 2. Khi conda hỏi bạn có muốn tiếp tục không, nhập `y` và nhấn `Enter`.
```bash
proceed ([y]/n)?
```

## 3. Tạo môi trường ảo với phiên bản Python cụ thể:
```bash
conda create --name <Tên môi trường> python=3.8
```

## 4. Để xem danh sách các môi trường ảo đã tạo, sử dụng lệnh sau:
```bash
conda env list
```

## 5. Để kích hoạt môi trường ảo, sử dụng lệnh sau:
```bash
conda activate <Tên môi trường>
```

## 6. Để thoát khỏi môi trường ảo, sử dụng lệnh sau:
```bash
conda deactivate
```

## 7. Để xóa môi trường ảo, sử dụng lệnh sau:
```bash
conda remove --name <Tên môi trường> --all
```