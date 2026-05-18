# Hướng Dẫn Sử Dụng Hyper Hub

Hyper Hub là phần mềm điều khiển chuột HPW / HyperWork trên macOS. Cài 1 lần, dùng được mọi tính năng cho 3 dòng chuột: **Macro (MS02)**, **Silentium (MS01)**, **Silentium Gen 2 (MS01.G2)**.

> Hướng dẫn dành cho người dùng cuối — chỉ cần biết click chuột, không cần biết kỹ thuật.

---

## Mục lục

1. [App này dùng để làm gì?](#1-app-này-dùng-để-làm-gì)
2. [Cài đặt lần đầu](#2-cài-đặt-lần-đầu)
3. [Giao diện app](#3-giao-diện-app)
4. [Chọn chuột (Devices)](#4-chọn-chuột-devices)
5. [Màn hình SCANNING](#5-màn-hình-scanning)
6. [Tab Point & Scroll — Tốc độ chuột và cuộn](#6-tab-point--scroll--tốc-độ-chuột-và-cuộn)
7. [Tab Buttons — Gán nút chuột](#7-tab-buttons--gán-nút-chuột)
8. [Tab Macro — Ghi chuỗi thao tác tự động](#8-tab-macro--ghi-chuỗi-thao-tác-tự-động)
9. [Tab Ring — Vòng tròn 8 phím tắt](#9-tab-ring--vòng-tròn-8-phím-tắt)
10. [Tab Settings — Cài đặt chung](#10-tab-settings--cài-đặt-chung)
11. [Tự đổi profile theo app](#11-tự-đổi-profile-theo-app)
12. [Chuột MS02 có gì khác?](#12-chuột-ms02-có-gì-khác)
13. [Câu hỏi thường gặp](#13-câu-hỏi-thường-gặp)

---

## 1. App này dùng để làm gì?

Chuột HPW có nhiều nút phụ (nút bên, nút giữa, nút Sniper…). Mặc định macOS chỉ dùng được nút trái/phải. App **Hyper Hub** cho phép bạn:

- **Gán hành động cho từng nút** — vd nút bên cạnh bấm là `Copy`, `Paste`, hoặc mở Photoshop
- **Ghi macro** — chuỗi nhiều thao tác (vd: bấm 1 nút → tự gõ `Cmd+S`, đợi 1 giây, gõ `Esc`)
- **Vòng tròn 8 phím tắt (Action Ring)** — bấm 1 nút hiện ra menu hình tròn 8 ô, di chuột chọn ô để chạy
- **Đổi tự động** cài đặt khi sang app khác (vd: ở Photoshop chuột làm việc khác Final Cut)
- **Chỉnh DPI, tốc độ cuộn, đảo chiều cuộn** v.v.

**Cần macOS 11 trở lên**, dung lượng ~50MB.

---

## 2. Cài đặt lần đầu

### 2.1. Tải về và mở

1. Tải file `HyperHub-x.x.x.dmg` từ trang [GitHub Releases](https://github.com/hnaht95/hyper-hub-releases/releases/latest).
2. Mở file `.dmg` → kéo icon `Hyper Hub` vào thư mục `Applications`.
3. Mở app từ Launchpad hoặc gõ `Hyper Hub` ở Spotlight.

> App đã được Apple xác thực — mở thẳng, **không cần** click phải → Open như các phần mềm khác.

### 2.2. Cho phép 3 quyền

Lần đầu mở app, sẽ có 3 màn hình xin quyền:

| Quyền | Để làm gì |
|---|---|
| **Bluetooth** | Đọc/ghi cài đặt sang chuột Bluetooth, xem pin chuột |
| **Input Monitoring** (Theo dõi đầu vào) | Đọc tín hiệu chuột để biết bạn bấm nút nào |
| **Accessibility** (Trợ năng) | Gửi phím tắt thay cho chuột, mở vòng tròn 8 phím tắt |

Mỗi màn:
1. Bấm `Open System Settings` → macOS mở Cài đặt hệ thống
2. **Bật toggle Hyper Hub** trong danh sách
3. Quay lại app, bấm `Continue`

Lặp lại cho cả 3 quyền.

### 2.3. Kết nối chuột

3 cách kết nối, dùng cách nào cũng được:

- **Đầu thu 2.4G** (cái nhỏ cắm USB) — cắm vào máy, chuột tự kết nối
- **Bluetooth** — vào `Cài đặt hệ thống` → `Bluetooth`, ghép cặp với chuột Macro / MS01 / Silentium Gen 2
- **Cắm dây trực tiếp** vào USB (nếu chuột có cổng)

App sẽ nhận diện chuột trong vài giây. Khi đã kết nối, biểu tượng Bluetooth ở góc phải-trên app chuyển sang xanh.

---

## 3. Giao diện app

Cửa sổ app có 5 thẻ chính (đọc từ trái qua phải biểu tượng ở góc phải-trên):

| Tên thẻ | Dùng để |
|---|---|
| **Point & Scroll** | Chỉnh tốc độ chuột, tốc độ cuộn |
| **Buttons** | Gán hành động cho từng nút chuột |
| **Macro** | Ghi chuỗi thao tác tự động |
| **Ring** | Cài menu 8 phím tắt hình tròn |
| **Settings** | Cài đặt chung, ngôn ngữ, thông báo |

**Góc phải-trên cùng** có biểu tượng kết nối (xanh) hiển thị loại kết nối hiện tại — **BT**, **2.4G** hoặc **USB**. **Bấm vào** để mở danh sách chuột (xem mục 4).

> Khi chưa có chuột nào kết nối, app hiện màn hình **No Devices** che toàn bộ giao diện — không thấy biểu tượng này.

---

## 4. Chọn chuột (Devices)

Bấm biểu tượng kết nối ở góc phải-trên → hiện 3 thẻ chuột:

- **MACRO** (chính là MS02)
- **SILENTIUM** (MS01)
- **SILENTIUM GEN 2** (MS01.G2)

Mỗi thẻ hiển thị: ảnh chuột + tên + nhãn trạng thái (`BT` / `2.4G` / `Offline`).

**Màu sắc nói lên trạng thái:**

- **Màu xanh** (cả tên + nhãn) → chuột này **đang được chọn** (cài đặt áp dụng cho con này)
- **Màu trắng** (cả tên + nhãn) → chuột đang kết nối nhưng **chưa chọn** (bấm vào để chọn)
- **Trắng mờ** (ảnh chuột + tên + nhãn đều giảm độ sáng) → chuột **Offline / chưa kết nối / tắt nguồn**

Nhãn cụ thể:
- `BT` = đang kết nối qua Bluetooth
- `2.4G` = đang dùng đầu thu USB
- `Offline` = chưa kết nối / tắt nguồn

**Bấm vào thẻ** = chọn chuột đó. Mọi cài đặt sau đó (DPI, gán nút...) áp dụng cho chuột vừa chọn.

> Khi chỉ kết nối 1 chuột, app tự chọn — không cần làm gì.

**Nút "Quét lại"** ở góc phải-trên tab Devices: bấm để app dò lại toàn bộ chuột (BT + USB) ngay lập tức. Dùng khi chuột đã cắm/pair nhưng app chưa nhận diện.

---

## 5. Màn hình SCANNING

Khi chuột mất kết nối, app hiện màn hình **SCANNING** (nền tối + 9 chấm tròn nhịp sáng + chữ SCANNING…/ĐANG QUÉT…). Đây không phải lỗi treo — chỉ là báo "đang dò chuột, đợi chút".

### 5.1. Khi nào hiện

- Chuột hết pin / ngủ / ra ngoài vùng BT.
- Gạt sang mode chưa có kết nối (vd: Type A chưa cắm đầu thu).
- Rút đầu thu khi đang dùng 2.4G.

### 5.2. Khi nào KHÔNG hiện

- Gạt sang mode đã sẵn kết nối (đầu thu cắm sẵn / BT đã pair) → swap mượt.
- Lần đầu chọn chuột sau khi mở app.
- Bạn chủ động click chuột khác trong Devices tab.

### 5.3. Cách thoát

**Di chuột** một cái → app nhận input → SCANNING tự ẩn. Mọi cài đặt giữ nguyên.

> Overlay nuốt mọi click (tránh nhấn nhầm gây blank UI). Nếu chuột không bao giờ reconnect → quit app rồi mở lại.

---

## 6. Tab Point & Scroll — Tốc độ chuột và cuộn

Thẻ này chỉnh **cách con trỏ di chuyển** và **cách cuộn**.

### Bên trái: ảnh 3D con chuột đang dùng

Tự đổi theo chuột bạn chọn ở Devices.

### Bên phải: các phần điều chỉnh

**POINTER (chỉ MS02):**
- **DPI** — bấm số (800/1200/1600/2400/3200/6000) để đổi mức. Tự lưu vào chuột.
- **Polling Rate** (Tần số quét) — chọn 125 / 250 / 500 / 1000Hz. Cao = phản hồi nhanh (cho game).

> MS01, MS01.G2 dùng tốc độ chuột mặc định của macOS — không có phần POINTER này.

**MOUSE SCROLL** — 2 ô vuông toggle:
- **Reverse** — Standard (mặc định, giống Windows) / Natural (giống trackpad macOS).
- **Smooth** — bật/tắt cuộn mượt. Khi Smooth tắt, phần Scroll Speed/Feel bên dưới sẽ mờ đi.

**SCROLL SPEED** — thanh trượt: 1 cú lăn đi nhiều hay ít.

**SCROLL FEEL** — chọn 1 trong 5 preset cảm giác cuộn (kéo thanh trượt 5 mức):

| Preset | Cảm giác |
|---|---|
| **Linear** | Cuộn trả về tốc độ đúng, không gia tốc, dừng nhanh |
| **Smooth** | Mượt, gia tốc nhẹ, dừng từ từ |
| **Elastic** | Gia tốc nhẹ + đuôi dài (kiểu trackpad macOS) |
| **Snappy** | Phản hồi nhanh, dừng dứt khoát |
| **Heavy** | Gia tốc mạnh, đuôi dài — cảm giác "đậm tay" (mặc định) |

Đồ thị đường cong bên dưới là **preview** của preset đang chọn (read-only) — kéo qua các mức sẽ thấy hình đồ thị thay đổi tương ứng. Không bấm vào đồ thị được.

---

## 7. Tab Buttons — Gán nút chuột

Thẻ này gán hành động cho **từng nút trên chuột**.

### 3 cột

**Cột TRÁI — Danh sách profile**

- Profile "Global" (mặc định, áp dụng cho mọi app)
- Profile riêng cho từng app (vd Photoshop, Figma, Zalo...)
- Nút `+` ở dưới — bấm để thêm profile mới cho 1 app cụ thể

**Cột GIỮA — Ảnh chuột + chấm nút**

- Ảnh chuột bạn đang dùng
- Mỗi nút có 1 chấm tròn + nhãn (vd "Sniper", "Forward", "Back")
- Bấm vào chấm để chọn nút muốn cài đặt
- Nút đang chọn: chấm cam

**Cột PHẢI — Bảng chọn hành động**

- Trên cùng: tên hành động đang gán (vd `BACKWARD`)
- Ô tìm kiếm — gõ để lọc nhanh
- Danh sách hành động chia thành các nhóm (xem dưới)
- Bấm radio button = áp dụng ngay, không cần Save

### Các nhóm hành động

**ACTIONS (Hành động cơ bản)** — luôn có:
- Click trái / phải / giữa
- Forward / Back (mũi tên 2 bên)
- Scroll lên / xuống / trái / phải
- Open Website (mở trang web)
- Action Ring (mở vòng tròn 8 phím tắt — xem mục 9)
- **Mode Switch** — chuyển kết nối BT ↔ 2.4G (**chỉ Macro MS02**)
- **Fire Button** — bấm liên tiếp 8-10ms (cho game, **chỉ Macro MS02**)
- Default action (mặc định nhà sản xuất)
- Button off (tắt nút)

**GESTURE (Cử chỉ)** — giữ nút + kéo chuột:
- Mission Control, App Expose, Show Desktop
- Chuyển desktop trái / phải

**DPI** — chỉnh DPI (**chỉ MS02**)

**MULTIMEDIA**: Phát/Tạm dừng, bài trước, bài sau, tăng/giảm âm lượng, tắt tiếng

**SHORTCUT** (Phím tắt): Cut, Copy, Paste, Save, Undo, Redo... + nút "Custom" để nhập phím tắt riêng (vd `Cmd+Shift+P`)

**MACRO**: Toàn bộ macro bạn đã tạo (xem mục 8)

### Cách gán 1 nút

1. Chọn profile ở cột trái (vd "Global" hoặc "Photoshop")
2. Bấm chấm tròn của nút muốn cài (cột giữa)
3. Chọn hành động ở cột phải
4. Bấm thử nút trên chuột — phải chạy đúng

### Lưu ý

- Một số nút bị **khóa cứng** (vd DPI Cycle, Mode Switch trên MS01) — chấm có hiện nhưng không gán được, đó là quy định của hãng.
- Nút **Sniper** mặc định = Action Ring (vòng tròn 8 phím tắt).

---

## 8. Tab Macro — Ghi chuỗi thao tác tự động

Macro = chuỗi nhiều phím/click ghi sẵn. Bấm 1 nút → chạy lại cả chuỗi.

Ví dụ: macro "Lưu file":
1. Gõ `Cmd+S`
2. Đợi 0.5 giây
3. Gõ `Enter`

### 2 cột

**Cột TRÁI — Danh sách macro**
- Toàn bộ macro của profile đang chọn
- `+` để tạo mới
- `...` trên 1 macro → Đổi tên, Nhân đôi, Xóa, Xuất file

**Cột PHẢI — Khu vực ghi/sửa**
- Tên macro (đầu trang)
- Danh sách các bước (phím/click + thời gian chờ)
- Nút `Record` (Ghi) — bấm rồi gõ phím / click, app tự ghi lại
- Nút `Apply` (Áp dụng) — đẩy macro xuống chuột (chỉ MS02)

### Cách tạo macro

1. Bấm `+` ở cột trái → đặt tên (vd "Lưu nhanh")
2. Bấm `Record` → gõ chuỗi phím như bạn muốn macro chạy (vd `Cmd+S`)
3. Bấm `Stop` để dừng ghi
4. Bấm `Apply` để lưu vào chuột
5. Sang tab Buttons → gán macro vừa tạo cho 1 nút
6. Bấm nút đó → macro chạy

### 2 chế độ thời gian chờ

- **Use real delays** (Dùng thời gian thật) — giữ đúng tốc độ bạn gõ. Phù hợp với macro phức tạp.
- **Use min delay** (Dùng thời gian tối thiểu) — mọi bước đợi 10ms. Phù hợp với macro "bắn liên tiếp" trong game.

### 3 chế độ lặp

| Chế độ | Khi nào dùng |
|---|---|
| **Fixed** (Cố định) | Lặp đúng N lần rồi dừng (đặt N ở thanh trượt) |
| **Until key** (Đến khi bấm phím) | Lặp mãi cho đến khi bạn bấm 1 phím bất kỳ |
| **While hold** (Khi đang giữ) | Lặp khi giữ nút, nhả nút là dừng |

> Chuột Macro (MS02) hỗ trợ cả 3 chế độ. MS01 / MS01.G2 chỉ dùng được "Fixed".

### Giới hạn

- Mỗi profile chứa tối đa **32 macro**
- Mỗi macro tối đa **50 bước**

### Chia sẻ macro

- **Xuất:** `...` trên macro → "Export JSON" → lưu file `.json`
- **Nhập:** kéo file `.json` vào cột trái

---

## 9. Tab Ring — Vòng tròn 8 phím tắt

Action Ring = menu hình tròn 8 ô hiện ra **giữa màn hình** khi bấm 1 nút trên chuột (mặc định: nút Sniper). Di chuột chọn ô → bấm để chạy lệnh đó.

Dùng cho: phím tắt thường dùng trong từng app (vd Photoshop có Save, Copy, Paste, Undo, Brush, Eraser...).

### 3 cột

**Cột TRÁI — Danh sách app**
- "Global" (vòng tròn dùng cho mọi app khi không có profile riêng)
- Các app đã thiết lập riêng (Photoshop, Figma, Zalo...)
- `+` để thêm app mới

**Cột GIỮA — Vòng tròn 8 ô**
- 8 ô tròn xếp đều quanh tâm
- Mỗi ô có biểu tượng + tên hành động
- Bấm ô → chọn để chỉnh
- Ô đang chọn: viền cam
- **Dưới vòng tròn** hiện `SLOT N / {Tên App}` cho biết bạn đang chỉnh app nào

**Cột PHẢI — Bảng chọn hành động** (giống tab Buttons)

### Tạo vòng tròn cho 1 app

1. Cột trái: bấm `+` → chọn app (vd Photoshop)
2. App tự điền sẵn 8 ô cho Photoshop (Save, Copy, Paste, Undo, Redo...) nếu app đó có sẵn mẫu
3. Bấm ô để đổi hành động → chọn từ cột phải
4. Tự lưu, không cần Save

### Khi nào vòng tròn xuất hiện?

- Khi bạn đang dùng app nào, app đó có profile riêng → dùng vòng tròn của app đó
- Nếu app không có profile riêng → dùng vòng tròn Global

### Cách gọi vòng tròn

- Mặc định: bấm nút **Sniper** trên chuột
- Có thể gán nút khác sang Action Ring (tab Buttons)
- Khi vòng hiện ra: di chuột vào ô → bấm để chạy, hoặc click ra ngoài để hủy

---

## 10. Tab Settings — Cài đặt chung

### General (Tổng quan)

- **Language** — chọn Tiếng Việt / English. Khi đổi, app sẽ khởi động lại.
- **Use system font** — đổi sang font hệ thống (Apple SF Pro) thay vì font mặc định của app.
- **Color theme** — chế độ giao diện: theo hệ thống / Sáng / Tối
- **Open at login** — tự mở Hyper Hub khi đăng nhập máy

### Notifications (Thông báo)

Bật/tắt từng loại thông báo:

- **Khi đổi profile theo app** — hiện toast nhỏ ở góc phải-dưới
- **Khi đổi DPI** — overlay giữa màn hình hiện DPI mới
- **Khi pin yếu** — cảnh báo khi pin < 15% (chỉ MS02)
- **Khi đổi kết nối** — badge khi chuột chuyển BT ↔ 2.4G
- **Khi chạy gesture** — hiện tên hành động được kích hoạt

### About (Giới thiệu)

- Tên app + phiên bản hiện tại
- **Automatically install software updates** (Tự cài bản cập nhật) — mặc định **TẮT**:
  - Bật → app tự tải bản mới về và cài ở lần khởi động sau (im lặng)
  - Tắt → khi có bản mới, hiện popup hỏi bạn có muốn cài không
- `Check for Updates` (Kiểm tra cập nhật) — bấm để kiểm tra thủ công
- `Show release notes` — xem nhật ký cập nhật trên GitHub

### Advanced (Nâng cao)

- **Reset all profiles to defaults** — xóa toàn bộ profile + macro về mặc định
- **Reset permissions warnings** — bật lại cảnh báo thiếu quyền (sau khi đã tắt)
- **Export logs** — xuất file `.zip` log + dữ liệu để gửi cho bộ phận hỗ trợ debug

### Chế độ Dev (ẩn)

Dành cho người phát triển — bật bằng cách **bấm 7 lần liên tiếp vào ảnh chuột ở màn No Device** (khi chưa kết nối chuột). Người dùng bình thường không cần bật.

---

## 11. Tự đổi profile theo app

App sẽ **theo dõi** xem bạn đang dùng app nào (kiểm tra mỗi 1 giây). Khi bạn chuyển sang app khác:

- Nếu app đó có profile riêng → tự áp dụng profile đó (cài đặt nút, vòng tròn, DPI... đều đổi)
- Nếu app đó không có profile riêng → dùng profile Global

**Vd:**
- Đang dùng Safari → profile Global (Sniper = Action Ring chung)
- Chuyển sang Photoshop → tự đổi sang profile Photoshop (Sniper = Action Ring riêng cho Photoshop, các nút khác làm Save / Brush...)
- Chuyển sang Final Cut → tự đổi sang profile Final Cut

### Cách thêm profile cho 1 app

1. Vào tab Buttons hoặc Ring
2. Cột trái bấm `+`
3. Chọn app từ danh sách hệ thống (Photoshop, Figma, ...)
4. App tự tạo profile mới — bắt đầu gán nút / vòng tròn cho app đó

---

## 12. Chuột MS02 có gì khác?

Chuột Macro (MS02) là dòng cao cấp, có **chip riêng của HPW**. Hai dòng MS01 / MS01.G2 dùng chip phổ thông nên không có nhiều tính năng "nhớ trong chuột".

### Tính năng CHỈ có ở MS02

| Tính năng | MS02 | MS01 / MS01.G2 |
|---|:-:|:-:|
| Đổi DPI từ app | ✓ | ✗ |
| Đổi tần số quét (Polling) | ✓ | ✗ |
| **Chuột nhớ cài đặt** khi tắt app | ✓ | ✗ (mất khi tắt app) |
| Macro chạy ngay trong chuột | ✓ | ✗ (cần app chạy) |
| Chế độ lặp Until-key / While-hold | ✓ | ✗ |
| **Mode Switch** (đổi kết nối BT ↔ 2.4G bằng nút) | ✓ | ✗ |
| **Fire Button** (bấm liên tiếp cho game) | ✓ | ✗ |
| Xem **dung lượng pin** trong app | ✓ | ✗ |

### Tính năng CÓ ở tất cả

| Tính năng | Mọi chuột |
|---|:-:|
| Action Ring (vòng tròn 8 phím tắt) | ✓ |
| Đảo chiều cuộn, chỉnh tốc độ cuộn | ✓ |
| Chỉnh tốc độ chuột, gia tốc, làm mượt | ✓ |
| Đổi profile tự động theo app | ✓ |
| Cuộn ngang (MS01.G2 có con lăn ngang) | ✓ MS01.G2 |
| Phím media (Play/Pause...), gesture | ✓ |

### Khi tắt app, chuột nhớ gì?

- **MS02:** Mọi gán nút, macro, DPI... đều **lưu vĩnh viễn vào chuột**. Tắt app, rút USB, qua đêm — chuột vẫn nhớ.
- **MS01 / MS01.G2:** Cần Hyper Hub chạy nền để gán nút hoạt động. Tắt app → các nút trở về mặc định.

---

## 13. Câu hỏi thường gặp

### App không thấy bản cập nhật mới?

- App tự kiểm tra mỗi 24 giờ. Vào `Settings → About → Check for Updates` để kiểm tra ngay.
- Hoặc tải file `.dmg` mới nhất từ [trang GitHub](https://github.com/hnaht95/hyper-hub-releases/releases).

### App bị treo / crash?

- Cập nhật lên bản mới nhất (Settings → About → Check for Updates).
- Nếu vẫn lỗi, làm theo mục "Reset toàn bộ" bên dưới.

### Con trỏ đôi khi đứng yên?

- Hiện tượng này xảy ra khi chuột chuyển giữa Bluetooth ↔ 2.4G — macOS cần 1-3 giây để kết nối lại. Đợi chuột ổn định.
- Khi xảy ra, app sẽ hiện màn hình **SCANNING** (xem mục 5) để báo cho bạn biết đang dò kết nối.

### Tại sao app hiện màn hình SCANNING với 9 chấm tròn nhịp sáng?

- Đó là feedback hình ảnh báo "chuột đang chuyển mode / mất kết nối". Xem mục 5.
- Cách thoát: di chuột HPW → tự ẩn. Không có nút thoát thủ công (overlay nuốt mọi click).

### Gạt chuột sang mode khác mà KHÔNG thấy màn hình SCANNING?

- Nếu mode bạn vừa gạt sang **đã sẵn kết nối** (vd Type C → BT đã pair, hoặc đầu thu 2.4G đã cắm sẵn) — app **không hiện** SCANNING vì không cần đợi. Đây là hành vi đúng.
- Chỉ hiện SCANNING khi chuột đi vào trạng thái "không có kết nối nào sẵn sàng".

### Màn hình SCANNING không tự ẩn sau khi di chuột?

- Đảm bảo bạn di chuột là **chuột HPW** (không phải chuột phụ khác). App chỉ ẩn khi nhận input từ chuột HPW.
- Nếu chuột chưa kết nối lại được (pin yếu / ngoài tầm BT) — di chuột không phát tín hiệu → SCANNING giữ vô hạn. Quit app + mở lại để reset, hoặc bấm "Quét lại" trong tab Devices (nếu UI cho phép).

### Pin hiển thị sai (chỉ MS02)?

- 30 giây đầu sau khi mở app: pin có thể chưa cập nhật, đợi vài giây.
- Vừa chuyển kết nối: pin reset, đợi ~10 giây.
- MS01 và MS01.G2: **không hiển thị pin** trong app (giá trị không tin cậy nên đã ẩn).

### Không thấy "Mode Switch" trong danh sách gán nút?

- Tính năng này chỉ có trên chuột Macro (MS02). MS01 / MS01.G2 không hỗ trợ.

### Có 2 chuột HPW cùng kết nối?

- App hỗ trợ tốt. Mỗi chuột có cài đặt riêng (cuộn, tốc độ, profile).
- Một số trường hợp hiếm: pin hai chuột cùng loại (vd 2 con MS02) có thể hiển thị sai. Đợi vài giây để cập nhật.
- Khi chuột bạn đang dùng disconnect (gạt mode chưa kết nối, hết pin...), app tự chuyển sang chuột HPW khác đang online — **vẫn hiện SCANNING** để bạn biết. Di chuột HPW khác (chuột app vừa chuyển sang) → SCANNING ẩn, tiếp tục dùng chuột đó. Xem mục 5 để hiểu thêm.

### Reset toàn bộ về như mới cài

Mở `Terminal`, copy 3 dòng sau, dán vào, nhấn Enter:

```bash
rm -rf ~/Library/Application\ Support/HyperHub/
defaults delete com.hpw.mouse.configurator
tccutil reset All com.hpw.mouse.configurator
```

→ Mở lại Hyper Hub, cấp lại 3 quyền như lần đầu cài.

### Gửi log cho hỗ trợ

Vào `Settings → Advanced → Export logs` → app tạo file `.zip` chứa log + cấu hình. Gửi file này cho bộ phận hỗ trợ.

---

## Liên hệ & tài liệu khác

- **Tải app mới nhất:** https://github.com/hnaht95/hyper-hub-releases/releases
- **Báo lỗi / yêu cầu tính năng:** mở Issue trên GitHub
