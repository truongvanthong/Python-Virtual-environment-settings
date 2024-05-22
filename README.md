# HƯỚNG DẪN TẠO MÔI TRƯỜNG ẢO PYTHON VỚI CONDA & VIRTUALENV

<!-- Mục lục -->
- [Tạo môi trường ảo với conda](#tạo-môi-trường-ảo-với-conda)
  - [1. Tạo môi trường ảo với conda](#1-tạo-môi-trường-ảo-với-conda)
  - [2. Khi conda hỏi bạn có muốn tiếp tục không, nhập `y` và nhấn `Enter`.](#2-khi-conda-hỏi-bạn-có-muốn-tiếp-tục-không-nhập-y-và-nhấn-enter)
  - [3. Tạo môi trường ảo với phiên bản Python cụ thể](#3-tạo-môi-trường-ảo-với-phiên-bản-python-cụ-thể)
  - [4. Xem danh sách các môi trường ảo đã tạo](#4-xem-danh-sách-các-môi-trường-ảo-đã-tạo)
  - [5. Kích hoạt môi trường ảo](#5-kích-hoạt-môi-trường-ảo)
  - [6. Thoát khỏi môi trường ảo](#6-thoát-khỏi-môi-trường-ảo)
  - [7. Xóa môi trường ảo](#7-xóa-môi-trường-ảo)

- [Cách cài đặt môi trường ảo bằng Virtualenv](#cách-cài-đặt-môi-trường-ảo-bằng-virtualenv)
    - [1. Cài đặt Virtualenv](#1-cài-đặt-virtualenv)
    - [2. Tạo môi trường ảo](#2-tạo-môi-trường-ảo)
    - [3. Kích hoạt môi trường ảo](#3-kích-hoạt-môi-trường-ảo)
    - [4. Lưu ý rằng để kích hoạt môi trường ảo của bạn trên Windows, sẽ cần chạy đoạn mã sau bên dưới:](#4-lưu-ý-rằng-để-kích-hoạt-môi-trường-ảo-của-bạn-trên-windows-sẽ-cần-chạy-đoạn-mã-sau-bên-dưới)
    - [5. Thoát khỏi môi trường ảo](#5-thoát-khỏi-môi-trường-ảo)
    - [6. Kiểm tra danh sách các thư viện đã cài đặt trong môi trường ảo](#6-kiểm-tra-danh-sách-các-thư-viện-đã-cài-đặt-trong-môi-trường-ảo)
    - [7. Xuất danh sách các thư viện đã cài đặt trong môi trường ảo ra file requirements.txt](#7-xuất-danh-sách-các-thư-viện-đã-cài-đặt-trong-môi-trường-ảo-ra-file-requirements.txt)
    - [8. Cài đặt các thư viện từ file requirements.txt](#8-cài-đặt-các-thư-viện-từ-file-requirements.txt)
    - [9. Xóa môi trường ảo](#9-xóa-môi-trường-ảo)

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

# Cách cài đặt môi trường ảo bằng Virtualenv

## 1. Cài đặt Virtualenv
```bash
pip install virtualenv
```

## 2. Tạo môi trường ảo
```bash
python<version> -m venv <Tên môi trường>
```
Ví dụ:
```bash
mkdir project
cd project
python3.9 -m venv myenv
```

## 3. Kích hoạt môi trường ảo
```bash
source myenv/bin/activate
```

## 4. Lưu ý rằng để kích hoạt môi trường ảo của bạn trên Windows, sẽ cần chạy đoạn mã sau bên dưới:
```bash
env/Scripts/activate.bat //In CMD
env/Scripts/Activate.ps1 //In PowerShell
```

## 5. Thoát khỏi môi trường ảo
```bash
deactivate
```

## 6. Kiểm tra danh sách các thư viện đã cài đặt trong môi trường ảo
```bash
pip list
```

## 7. Xuất danh sách các thư viện đã cài đặt trong môi trường ảo ra file requirements.txt
```bash
pip freeze > requirements.txt
```

## 8. Cài đặt các thư viện từ file requirements.txt
```bash
pip install -r requirements.txt
```

## 9. Xóa môi trường ảo
```bash
rm -rf myenv
```
