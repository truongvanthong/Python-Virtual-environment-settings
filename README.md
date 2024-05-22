# Tạo môi trường ảo với conda

## 1. Tạo môi trường ảo với conda

```bash
conda create --name <Tên môi trường>
```

## 2. Khi conda hỏi bạn có muốn tiếp tục không, nhập `y` và nhấn `Enter`.
```bash
proceed ([y]/n)?
```

## 3. Tạo môi trường ảo với phiên bản Python cụ thể
```bash
conda create --name <Tên môi trường> python=3.8
```

## 4. Xem danh sách các môi trường ảo đã tạo
```bash
conda env list
```

## 5. Kích hoạt môi trường ảo
```bash
conda activate <Tên môi trường>
```

## 6. Thoát khỏi môi trường ảo
```bash
conda deactivate
```

## 7. Xóa môi trường ảo
```bash
conda remove --name <Tên môi trường> --all
```