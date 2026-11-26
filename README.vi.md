# Pet Project Mini

[English](README.md) | **Tiếng Việt**

Tổng hợp các dự án nhỏ trong quá trình tự học: ba trang web tĩnh (HTML/CSS/JS) và một game Cờ Caro chạy trên console viết bằng C++.

## Danh sách dự án

| Thư mục | Dự án | Công nghệ |
|---|---|---|
| [`FE_Project_1`](FE_Project_1) | Trang web xem anime | HTML, CSS, Font Awesome, Google Fonts |
| [`FE_Project_2`](FE_Project_2) | Landing page doanh nghiệp "Softy Pinko" | HTML, CSS, Bootstrap 4, Font Awesome |
| [`FE_Project_3`](FE_Project_3) | Trang tra cứu đáp án "Vô Song Giáo" | HTML, CSS, JavaScript thuần |
| [`Console_GameCaro`](Console_GameCaro) | Game Cờ Caro trên console | C++, Win32 Console API, Visual Studio |

### 1. FE_Project_1 — Trang web xem anime

Giao diện một trang cho website xem anime, dựng lại từ thiết kế để luyện front-end:

- Banner chính giới thiệu *Demon Slayer (Thanh Gươm Diệt Quỷ)*
- Thẻ thể loại (Shonen, Action, Fantasy, Romance, Comedy, Drama, Sci-Fi, Adventure)
- Các mục **Trending Shows**, **Continue Watching**, **Recently Released**
- Footer với các nhóm liên kết

Dùng CSS reset và tách riêng `base.css` / `styles.css`.

### 2. FE_Project_2 — Landing page Softy Pinko

Dựng lại template *Softy Pinko* (gốc của TemplateMo) bằng hệ thống lưới của Bootstrap 4:

- Banner, danh sách tính năng, mục "Work Process"
- Đánh giá khách hàng, bảng giá, bài viết blog
- Form liên hệ và footer

### 3. FE_Project_3 — Tra cứu đáp án Vô Song Giáo

Trang hỗ trợ trả lời phần "Vấn Đáp Tông Môn" trên một trang web hoạt hình Trung Quốc:

- Khoảng **149 câu hỏi và đáp án** lưu trong `js.js`
- **Tìm kiếm tức thì**: bảng tự lọc khi gõ vào ô tìm kiếm
- Hiệu ứng trang trí Tết (pháo hoa, hoa mai rơi)

### 4. Console_GameCaro — Game Cờ Caro bằng C++

Game Cờ Caro chạy trên cửa sổ console Windows, viết theo hướng đối tượng (`_Board`, `_Game`, `_Point`, `_Common`, `_Play`).

**Tính năng**

- Bàn cờ 16 × 16 vẽ trên console
- Chế độ chơi: **Người vs Người** và **Người vs Máy**
- Máy tính điểm tấn công và phòng thủ cho từng ô trống theo hàng ngang, hàng dọc và hai đường chéo để chọn nước đi; trong code có sẵn bảng điểm cho mức dễ và khó
- Luật thắng: đủ đúng 5 quân liên tiếp và không bị chặn hai đầu (luật Caro Việt Nam)
- Đếm tỉ số qua các ván, hiệu ứng thắng/hòa và âm thanh khi thắng
- **Lưu / tải** ván cờ theo tên file (danh sách tên được ghi trong `Name.txt`)

**Phím điều khiển**

| Phím | Chức năng |
|---|---|
| `W` `A` `S` `D` | Di chuyển con trỏ |
| `Enter` | Đánh cờ / chọn mục trong menu |
| `L` | Lưu ván cờ |
| `T` | Tải ván cờ đã lưu |
| `Esc` | Quay lại / thoát |

**Cách build và chạy**

1. Mở `Console_GameCaro/GameCaroConsole/GameCaroConsole.sln` bằng **Visual Studio 2022** (toolset v143).
2. Build và chạy (`Ctrl + F5`). Chỉ chạy trên Windows vì game dùng `<Windows.h>`, `conio.h` và `winmm.lib` để phát âm thanh.
3. Tùy chọn: đặt file `win.wav` cạnh file thực thi để nghe âm thanh khi thắng.

Báo cáo đồ án nằm ở `Console_GameCaro/BaoCao.docx`.

## Chạy các dự án front-end

Không cần build. Clone repo rồi mở file `index.html` của từng dự án bằng trình duyệt:

```bash
git clone https://github.com/thiennguyenk01/Pet_Project_Mini.git
cd Pet_Project_Mini
# sau đó mở FE_Project_1/index.html, FE_Project_2/index.html hoặc FE_Project_3/index.html
```

Cần có mạng để tải font, icon và Bootstrap từ CDN.

## Cấu trúc thư mục

```
Pet_Project_Mini/
├── FE_Project_1/          # Trang xem anime
│   ├── index.html
│   └── assets/ (css, images)
├── FE_Project_2/          # Landing page Softy Pinko
│   ├── index.html
│   └── assets/ (css, images)
├── FE_Project_3/          # Tra cứu đáp án Vô Song Giáo
│   ├── index.html
│   ├── style.css
│   ├── js.js
│   └── img/
└── Console_GameCaro/      # Game Cờ Caro bằng C++
    ├── BaoCao.docx
    └── GameCaroConsole/   # Solution Visual Studio
```

## Tác giả

**Thiện Nguyễn** — [@thiennguyenk01](https://github.com/thiennguyenk01)

Đây là các dự án cá nhân phục vụ việc học. Thiết kế và nội dung thuộc về chủ sở hữu gốc.
