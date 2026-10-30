1. VẤN ĐỀ
2. YÊU CẦU
3. CÁCH LÀM

# Báo cáo phân tích
** Sơ đồ luồng**
```
[ Designer bấm Ctrl+S ]
        |
        v
[ L1 - Local SSD ] Ghi file .blend 2GB vào D:\PTIT_Museum\ (0.1s, siêu nhanh)
        |
        v
[ L2 - Watcher ] OneDrive / Drive Client phát hiện file đổi, đưa vào hàng đợi Upload
        |
        v
[ L3 - Cloud Sync ] Đẩy file lên Cloud qua HTTPS, hiện icon đang xoay
        |
        v
[ L4 - Cloud Storage ] Lưu xong -> Trả về tích xanh ✓ + Tạo Version History mới
```


** Cách hệ thống sử lý khi sảy ra xung đột phiên bản**
Hệ thống sẽ KHÔNG ghi đè bừa. Nó sẽ làm:

1.  Giữ lại bản nào upload lên trước làm bản chính.
2.  Tự tạo 1 bản sao: `Ten_file (Conflicted copy from May A - 30-10-2026).blend`
3.  Cả nhóm sẽ có 2 bản để tự so sánh, không mất dữ liệu của ai.


# Quy trình thực thi



**Bước 1: Cài đặt google drive for desktop**
**Bước 2: Tạo thư mục để thiết kế 3D**
**Bước 3: Đưa thư mục dồng bộ vào google drive**



