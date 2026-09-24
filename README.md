# 💻 Computer.Test — Công Cụ Kiểm Tra Phần Cứng Máy Tính Trực Tuyến

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vue.js](https://img.shields.io/badge/Vue.js_3-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

**Computer.Test** là một ứng dụng web đơn tệp (Single File Web App) hiện đại, siêu nhẹ và toàn diện, giúp người dùng kiểm tra nhanh chóng tình trạng hoạt động của toàn bộ phần cứng máy tính (Bàn phím, Chuột, Màn hình, Webcam, Micro, Loa, Pin và Tần số quét / FPS) trực tiếp trên trình duyệt web mà không cần cài đặt bất kỳ phần mềm nào.

---

## 📋 Mục Lục
- [✨ Tính Năng Nổi Bật](#-tính-năng-nổi-bật)
- [🔍 Chi Tiết Từng Chức Năng](#-chi-tiết-từng-chức-năng)
  - [1. ⌨️ Kiểm Tra Bàn Phím (Keyboard Test)](#1-️-kiểm-tra-bàn-phím-keyboard-test)
  - [2. 🖱️ Kiểm Tra Chuột & Lỗi Double Click (Mouse Test)](#2-️-kiểm-tra-chuột--lỗi-double-click-mouse-test)
  - [3. 🖥️ Kiểm Tra Màn Hình & Điểm Chết (Screen Test)](#3-️-kiểm-tra-màn-hình--điểm-chết-screen-test)
  - [4. 📷 Kiểm Tra Webcam (Webcam Test)](#4--kiểm-tra-webcam-webcam-test)
  - [5. 🎙️ Kiểm Tra Micro (Microphone Test)](#5-️-kiểm-tra-micro-microphone-test)
  - [6. 🔊 Kiểm Tra Loa & Âm Thanh (Speaker Test)](#6--kiểm-tra-loa--âm-thanh-speaker-test)
  - [7. 🔋 Kiểm Tra Pin & Sức Khỏe Pin (Battery Test)](#7--kiểm-tra-pin--sức-khỏe-pin-battery-test)
  - [8. 🎬 Kiểm Tra FPS & Độ Mượt Màn Hình (FPS Check - Vue 3)](#8--kiểm-tra-fps--độ-mượt-màn-hình-fps-check---vue-3)
- [🖥️ Chế Độ Toàn Màn Hình (Fullscreen Test Area)](#️-chế-độ-toàn-màn-hình-fullscreen-test-area)
- [🎨 Hỗ Trợ Giao Diện Sáng / Tối (Light & Dark Theme)](#-hỗ-trợ-giao-diện-sáng--tối-light--dark-theme)
- [🌐 Khả Năng Tương Thích Trình Duyệt](#-khả-năng-tương-thích-trình-duyệt)
- [🚀 Hướng Dẫn Sử Dụng](#-hướng-dẫn-sử-dụng)
- [📜 Giấy Phép (License)](#-giấy-phép-license)

---

## ✨ Tính Năng Nổi Bật

- 🚀 **100% Run on Client-Side**: Chạy trực tiếp trên trình duyệt, không cần máy chủ backend, không thu thập dữ liệu cá nhân.
- ⚡ **Siêu nhẹ & Tốc độ cao**: Xây dựng bằng HTML5, Vanilla JavaScript ES6+, Web Audio API, MediaDevices API và Vue 3 (Composition API).
- 📱 **Giao diện Responsive & Auto-Scale**: Tự động co giãn phù hợp với mọi độ phân giải màn hình từ Laptop đến PC Gaming siêu rộng.
- 🖵 **Chế độ Fullscreen độc lập**: Cho phép phóng to khu vực kiểm tra để thao tác không bị xao nhấp.
- 🌗 **Theme Sáng / Tối mượt mà**: Tự động tương thích với giao diện Sáng/Tối của hệ thống hoặc nền trang web.

---

## 🔍 Chi Tiết Từng Chức Năng

### 1. ⌨️ Kiểm Tra Bàn Phím (Keyboard Test)
Công cụ giúp kiểm tra độ nhạy, phím kẹt, liệt phím và khả năng gõ nhiều phím cùng lúc (N-Key Rollover).
- **Hỗ trợ 3 bố cục bàn phím**: `100% Full-size` (có phím số Numpad), `80% TKL (Tenkeyless)` và `60% Compact`.
- **Hệ điều hành linh hoạt**: Chuyển đổi giao diện phím giữa **Windows** (`Win`, `Ctrl`, `Alt`) và **macOS** (`Cmd ⌘`, `Option ⌥`, `Control ⌃`).
- **Âm thanh gõ phím chân thực**: Tạo hiệu ứng tiếng click phím bằng Web Audio API (có nút BẬT/TẮT âm thanh).
- **Thống kê chuyên sâu**:
  - Đếm tổng số lần nhấn phím (`Total Presses`).
  - Tốc độ gõ phím tức thì (`CPS - Clicks Per Second`) và tốc độ cao nhất (`Max CPS`).
  - Hiển thị thông tin mã phím kỹ thuật (`Event Code` & `Key Name`).
  - Nhật ký các phím vừa nhấn gần đây kèm mốc thời gian.
- **Phân loại trạng thái phím qua màu sắc**:
  - *Chưa nhấn*: Màu trung tính.
  - *Đang giữ phím*: Nổi bật màu xanh lục sáng.
  - *Đã nhận diện thành công*: Lưu vết màu xanh lá.

---

### 2. 🖱️ Kiểm Tra Chuột & Lỗi Double Click (Mouse Test)
Công cụ kiểm tra toàn diện các nút bấm chuột và phát hiện sự cố liệt / double-click tự động.
- **Kiểm tra 5 nút bấm chuẩn**: Chuột trái (Left), Chuột phải (Right), Nút cuộn giữa (Middle Click), Nút Back (Mouse 4) và Forward (Mouse 5).
- **Đo con lăn chuột (Scroll Wheel)**: Phát hiện hướng cuộn (Scroll Up / Scroll Down) và tốc độ lăn.
- **Bộ phát hiện lỗi Double Click (Debounce Bug Detector)**:
  - Tự động đo khoảng thời gian giữa 2 lần nhấp liên tiếp chính xác đến miligiây (`ms`).
  - Phân tích và cảnh báo màu đỏ nếu phát hiện nút chuột bị nảy đúp bất thường (thời gian phản hồi `< 80ms`).
  - Lưu nhật ký lịch sử click kèm cảnh báo nút hư hỏng switch.

---

### 3. 🖥️ Kiểm Tra Màn Hình & Điểm Chết (Screen Test)
Công cụ phát hiện điểm chết (Dead Pixels), điểm sáng (Stuck Pixels) và hở sáng màn hình.
- **5 Màu nền kiểm tra tiêu chuẩn**: Đen (`#000000`), Trắng (`#ffffff`), Đỏ (`#ff0000`), Xanh lá (`#00ff00`), Xanh dương (`#00ff00`).
- **Điều chỉnh độ sáng giả lập (0% - 100%)**: Giúp kiểm tra hiện tượng hở sáng viền (Backlight Bleeding) ở các mức độ sáng khác nhau.
- **Chế độ phủ kín toàn màn hình (Fullscreen Overlay)**: Click chuột hoặc bấm phím mũi tên để chuyển màu nhanh chóng, bấm `ESC` để thoát.

---

### 4. 📷 Kiểm Tra Webcam (Webcam Test)
Công cụ kiểm tra khả năng hiển thị, độ phân giải và quyền truy cập camera.
- **Tự động nhận diện danh sách Camera**: Liệt kê toàn bộ Webcam tích hợp, Webcam USB gắn ngoài hoặc Capture Card kết nối với máy tính.
- **Xem trực tiếp (Live Preview)**: Hiển thị hình ảnh thời gian thực với độ trễ tối thiểu thông qua `getUserMedia` API.
- **Đèn báo trạng thái**: Đèn LED xanh bừng sáng khi camera đang hoạt động ổn định, màu đỏ khi gặp lỗi hoặc bị từ chối quyền.

---

### 5. 🎙️ Kiểm Tra Micro (Microphone Test)
Công cụ test thu âm, độ nhạy micro và khả năng xử lý tiếng ồn.
- **Tự động chọn thiết bị đầu vào (Audio Input Device)**: Hỗ trợ chuyển đổi giữa Micro tai nghe, Micro thu âm USB hoặc Micro laptop.
- **Biểu đồ âm lượng thời gian thực (Audio Spectrum / DB Meter)**: Sử dụng Web Audio API `AnalyserNode` hiển thị thanh cường độ âm thanh trực quan khi bạn nói.
- **Thu âm & Phát lại ngay lập tức (Voice Recorder & Playback)**: Cho phép ghi âm mẫu tối đa 10 giây và nghe lại ngay để kiểm tra chất lượng âm thanh, độ trong và tiếng rè.

---

### 6. 🔊 Kiểm Tra Loa & Âm Thanh (Speaker Test)
Công cụ test khả năng phát âm thanh phân kênh Stereo và dải tần số âm thanh của loa/tai nghe.
- **5 Kịch bản test âm thanh chuyên dụng**:
  1. *Loa Trái (Left Channel Only)*: Chỉ phát âm thanh sang bên trái.
  2. *Loa Phải (Right Channel Only)*: Chỉ phát âm thanh sang bên phải.
  3. *Cả 2 Loa (Stereo Both Channels)*: Kiểm tra cân bằng âm thanh 2 bên.
  4. *Âm Treble (High Frequency Pitch)*: Phát tần số cao để test loa tép.
  5. *Âm Bass (Low Frequency Subwoofer)*: Phát tần số trầm để test loa bass.
- **Sóng âm hoạt hình (Waveform Visualizer)**: Hiển thị dải sóng âm nhịp nhàng khi nhạc/tần số đang phát.
- **Thanh điều chỉnh âm lượng tổng (Master Volume)**: Điều chỉnh từ `0%` đến `100%` trực tiếp trên công cụ.

---

### 7. 🔋 Kiểm Tra Pin & Sức Khỏe Pin (Battery Test)
Theo dõi trạng thái dung lượng và thời lượng sử dụng pin đối với Laptop hoặc máy tính bảng Windows/macOS.
- **Thông số thời gian thực (Battery Status API)**:
  - Phần trăm dung lượng pin hiện tại (`%`).
  - Trạng thái Nguồn điện: Đang sạc (⚡ Charging) hoặc Đang xả pin (🔋 Discharging).
  - Ước tính thời gian sạc đầy hoặc thời gian sử dụng còn lại.
- **Cảnh báo pin yếu**: Đổi màu thanh hiển thị pin và xuất hiện banner cảnh báo khi pin xuống dưới `20%`.
- **Tích hợp lệnh tạo Báo cáo Sức khỏe Pin chi tiết (Battery Report)**:
  - Cung cấp sẵn các câu lệnh PowerShell 1-click để người dùng kiểm tra chai pin, số lần sạc (Cycle Count) và dung lượng thiết kế (Design Capacity) trên Windows.

---

### 8. 🎬 Kiểm Tra FPS & Độ Mượt Màn Hình (FPS Check - Vue 3)
Công cụ benchmark kiểm tra tốc độ khung hình và độ mượt của màn hình (hỗ trợ màn hình 60Hz, 120Hz, 144Hz, 240Hz, 360Hz+).
- **🎬 So sánh Khung hình (Framerate Comparison)**:
  - Chạy đồng thời các làn chuyển động ở các mức FPS khác nhau (`15 vs 30 vs 60`, `30 vs 60 vs 120`, `60 vs 120 vs 144`, `60 vs 144 vs 240` hoặc Tuỳ chỉnh).
  - 2 chế độ hiển thị: *Thanh ngang mượt* & *Vật thể UFO*.
  - Tùy chỉnh tốc độ di chuyển (`480px/s` đến `3840px/s`).
- **📊 Phát hiện Trễ nhịp (Jank / Stutter Detector)**:
  - Vẽ đồ thị thời gian khung hình (Frame Time in `ms`) thời gian thực.
  - Tự động ghi nhận các khung hình bị khựng (`> 25ms`), tính toán **Điểm mượt (Jank Score 0-100%)** và lưu lịch sử trễ nhịp.
- **📜 Đánh giá độ mượt khi Cuộn (Scroll Jank Test)**:
  - Mô phỏng danh sách chứa nhiều khối giao diện nặng (Gradient, Shadow, Blur) để kiểm tra độ mượt khi cuộn trang web.
- **👻 Kiểm tra Hiện tượng Lưu ảnh / Bóng ma (Ghosting Test)**:
  - Cho các vạch kẻ và văn bản chạy tốc độ cao để kiểm tra thời gian đáp ứng (Response Time) của tấm nền màn hình (IPS, VA, TN, OLED).
- **Thanh thông tin phần cứng màn hình**: Hiển thị Độ phân giải màn hình, Tỷ lệ điểm ảnh (DPR) và Tự động đo Tần số quét thực tế (`Hz`).

---

## 🖥️ Chế Độ Toàn Màn Hình (Fullscreen Test Area)

Tất cả các công cụ được đặt gọn trong khu vực làm việc trung tâm. Người dùng có thể nhấn nút **"Phóng to khu vực Test"** (`⛶`) ở góc trên bên phải để ẩn đi các chi tiết thừa xung quanh và tập trung kiểm tra ở chế độ toàn màn hình.

---

## 🎨 Hỗ Trợ Giao Diện Sáng / Tối (Light & Dark Theme)

Ứng dụng sử dụng hệ thống biến CSS (`CSS Variables`) thông minh, tự động thay đổi màu sắc nền, màu chữ, viền và các điểm nhấn (`Accent Colors`) tương thích hoàn hảo với giao diện nền trang web hoặc giao diện hệ thống (Light Mode / Dark Mode).

---

## 🌐 Khả Năng Tương Thích Trình Duyệt

| Trình duyệt | Hỗ trợ Bàn phím / Chuột / Screen | Hỗ trợ Webcam / Micro / Loa | Hỗ trợ Battery API | Hỗ trợ FPS / Vue 3 |
| :--- | :---: | :---: | :---: | :---: |
| **Google Chrome** | ✅ 100% | ✅ 100% | ✅ 100% | ✅ 100% |
| **Microsoft Edge** | ✅ 100% | ✅ 100% | ✅ 100% | ✅ 100% |
| **Brave / Opera** | ✅ 100% | ✅ 100% | ✅ 100% | ✅ 100% |
| **Mozilla Firefox** | ✅ 100% | ✅ 100% | ⚠️ Hạn chế | ✅ 100% |
| **Apple Safari** | ✅ 100% | ✅ 100% | ⚠️ Hạn chế | ✅ 100% |

---

## 🚀 Hướng Dẫn Sử Dụng

1. **Mở trực tiếp**: Tải file `ComputerTest.html` về máy tính và nhấp đôi để mở bằng bất kỳ trình duyệt web nào.
2. **Nhúng vào Website / Blogger / WordPress**:
   - Sao chép toàn bộ nội dung trong file `ComputerTest.html`.
   - Dán vào bài viết hoặc trang HTML custom trên giao diện Blogger / WordPress của bạn.
3. Không cần cài đặt `node_modules` hay chạy lệnh build phức tạp!

---

## 📜 Giấy Phép (License)

Dự án này được phát hành dưới giấy phép **MIT License**. Bạn có thể tự do sử dụng, chỉnh sửa và chia sẻ cho mục đích cá nhân hoặc thương mại.