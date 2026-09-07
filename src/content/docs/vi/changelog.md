---
title: "Nhật ký thay đổi"
---

## v1.16.23

### New Features

- (`/search hsr`) Thêm mục Kẻ Địch.
- (`/challenge hsr`) Thêm Chế Độ Hướng Đến Biển Sao vào thẻ Hồi Ức Hỗn Độn, Kể Chuyện Hư Cấu, và Ảo Ảnh Tận Thế.
- (`/challenge zzz`) Thêm Chế Độ Khó vào thẻ Tập Kích Nguy Cấp.
- (`/gacha-log import`) Thêm một-nút nhặp Lịch Sử Chỉnh Kênh cho Tài Khoản ZZZ HoYoLAB
- (`/mimo`) Thêm "Coi Lịch Sử Điểm".
- (`/accounts`) Thêm trạng thái và lần chạy tự động gần nhất cho tài khoản được chọn. 
- (`/profile zzz`) Thêm dử liệu thẻ nhân vật Sigrid.

### Improvements

- (`/search`) Tách thành các lệnh con `/search genshin` và `/search hsr`, tương tự như lệnh `/profile`..
- (`/gacha-log import`) Chỉ lấy các bản ghi mới thay vì toàn bộ lịch sử trong mỗi lần nhập dữ liệu.
- (`/gacha-log view`) Tự động cập nhật danh sách vật phẩm trong banner tiêu chuẩn để đảm bảo số liệu thống kê tỷ lệ thắng 50/50 luôn chính xác khi các vật phẩm giới hạn được đưa vào nhóm vật phẩm tiêu chuẩn.
- (`/challenge hsr`) Hiển thị đọi Hướng Đến Biển Sao dù màn Hướng Đến Biển Sao chưa được vượt qua.
- (`/challenge genshin stygian`) Khôi phục thông tin về điểm yếu và điểm mạnh của kẻ địch.
- (`/accompany`) Hiển thị nút bật/tắt tự động Ghé Thăm trong giao diện nhân vật.
- (`/notes`) Xóa cột và thông báo nhắc nhở về tính năng thám hiểm trong HSR, vì tính năng này không còn tồn tại trong trò chơi nữa.
- Ngừng gửi thông báo tin nhắn trực tiếp (DM) cho các tác vụ tự động đã được xếp hàng sau khi cài đặt tương ứng bị tắt, đồng thời hiển thị thời gian thực hiện hành động trên mỗi thông báo.
- Gộp tối đa 10 thông báo tác vụ tự động vào một tin nhắn trực tiếp (DM) duy nhất và loại bỏ các thông báo về tác vụ thành công đã cũ hơn 12 giờ.

### Bug Fixes

- (`/gacha-log view`) Khắc phục lỗi các nhân vật hạng S trong ZZZ quay được từ banner tăng tỷ lệ của chính họ lại bị tính là thua cơ chế 50/50.

## v1.16.22

### Tính năng mới

- (`/accompany`) Thêm lệnh Ghé Thăm để xem nhân vật ghé thăm HoYoLAB, đặt nhân vật bạn yêu thích, và bật tự động check-in.
- (`/settings`) Thêm các cài đặt mới liên quan tới ghé thăm nhân vật HoYoLAB và tự động check-in.
- (`/profile genshin`) Thêm kiểu thẻ Enka cho Genshin Impact.
- (`/profile hsr`) Thêm dử liệu cho nhân vật mới cho HSR, trong đó có Himeko SP.
- (`/profile zzz`) Thêm dử liệu cho nhân vật mới cho ZZZ v3.1.
- (`/profile zzz`) Thêm hỗ trợ cho nguyên tố Lưu Minh.
- (`/card-settings`)  Thêm hỗ trợ hiển thị roll thuộc tính phụ cho loại thẻ Enka của Genshin và HSR.

### Cải thiện

- (`/card-settings`)  Thiết kế lại Cài đặt hình ảnh và gộp vào cài đặt thẻ; nút cài đặt thẻ riêng trong `/profile` đã bị xóa.
- (`/card-settings`) Cho phép sử dụng hình ảnh riêng, với một cảnh báo khi chọn kiểu thẻ không hổ trợ chúng.
- (`/card-settings`) Hiển thị bản xem trước ảnh vẻ chỉnh thức dựa trên ảnh vẻ thẻ thực tế.
- (`/card-settings`) Đã loại bỏ sử dụng Pixiv cho ảnh tùy chỉnh, vì dịch vụ cung cắp tính năng không còn hoạt động.
- (`/profile genshin`) Đã loại bỏ kiểu thẻ hattvr; các cài đặt hiện có đã được chuyển sang kiểu thẻ Enka.
- Cải thiện tốc độ tự động hoàn thành và độ tin cậy cho lệnh Genshin và HSR.

### Sửa lỗi

- (`/profile`) Sửa lỗi Nhà Lữ Hành lựa chọn trước khi được chuyển dưới dạng thông số.
- (`/profile zzz`) Sửa lỗi cho W-Engine không có thuộc tính phụ.
- (`/profile zzz`) Sửa ID Skin sai của nhân vật Velina.
- (`/card-settings`) Sửa lỗi làm hổng do ID nhân vật va chạm giữa các trò chơi.
- (`/card-settings`) Sửa bộ chọn ảnh không mở trong trang ảnh hiện tại.
- (`/characters zzz`) Sửa lỗi hỏng khi có hơn 25 tùy chọn lọc phe phái.
- (`/characters genshin`) Sửa lỗi khi gửi lựa chọn bộ lọc trống.
- (`/challenge`) Hiển thị lịch sử khi giai đoạn hiện tại không có dử liệu.
- (`/challenge genshin`) Sửa lỗi phần thông tin sát thương của La Hoàn Thâm Cảnh biến mất khi một số cấp bậc không có dữ liệu.
- (`/events`) Khắc phục lỗi khi phần thưởng sự kiện có độ hiếm không xác định.
- (`/search`) Khắc phục lỗi tự động hoàn thành cho các mục phiên bản beta.
- Sửa lỗi liên kết tài liệu mở sai ngôn ngữ..

## v1.16.21

### Tính năng mới

- (`/profile hsr`) Thêm đử liệu thẻ nhân vật HSR v4.3.
- (`/profile zzz`) Thêm đử liệu thẻ nhân vật ZZZ v3.0.
- (`/profile`) Thêm kiểu thẻ nhân vật Enka cho HSR và ZZZ.
- (`/profile zzz`) Hỗ trợ nhân vật với thuộc tính Phong.
- (`/characters zzz`) Hiển thị W-Engine và Trình độ kỹ năng.

### Cải thiện

- (`/profile`) Tăng tốc độ hiển thị thẻ bằng cách lưu trữ hình ảnh đã được thay đổi kích thước vào bộ nhớ cache.
- (`/characters`) Lưu vào bộ nhớ cache các trang đã được hiển thị để điều hướng nhanh hơn.
- (`/events`) Hiển thị thông báo rõ ràng về tính năng không được hỗ trợ đối với các trò chơi không có lịch sự kiện.
- (`/notes`) Hiển thị văn bản nhắc nhở trong thông báo đẩy trên thiết bị di động.

### Sửa lỗi

- (`/challenge hsr`) Xử lý dữ liệu Ải không đầy đủ trong Trọng Tài Dị Tướng, Hòi Ức Hỗn Độn và Kể Chuyện Hư Cấu mà không gây lỗi.
- (`/profile`) Sửa lỗi chỉ số cộng sát thương trong Genshin Impact mặc định sai là hệ Phong.
- (`/profile`) Khắc phục lỗi thẻ bài Genshin Impact do thiếu dữ liệu chỉ số và hình ảnh trang phục.
- (`/profile zzz`) Sửa vị trí hình ảnh của mẫu thẻ 2 cho các nhân vật ZZZ 3.0.
- (`/card-settings`) Khắc phục lỗi xác thực khi cấu hình nhân vật nhà lữ hành cho Genshin.
- (`/search`) Khắc phục lỗi khi mở trang Trích dẫn hoặc Truyện cho các nhân vật không có dữ liệu..
- (`/redeem`) Cải thiện việc xử lý lỗi khi đổi mã..
- Khắc phục lỗi tắt thông báo không có hiệu lực, điều này có thể dẫn đến việc tự động đổi tin nhắn trực tiếp không mong muốn.
- Nếu không có ngôn ngữ nào được thiết lập trong cài đặt, Discord sẽ tự động chuyển về ngôn ngữ mặc định của ứng dụng.

## v1.16.20

### Tính năng mới

- (`/profile zzz`) Thêm dữ liệu thẻ ZZZ v2.8.
- (`/profile zzz`) Thểm dữ liệu skin Miyabi cho thẻ nhân vật.

### Cải thiện

- (`/profile hsr`) Cải thiện logic hiển thị chỉ số trong thẻ nhân vật, bao gồm cả chỉ số tăng sát thương khi sử dụng nhân vật Vui Vẻ.

### Sửa lỗi

- (`/profile zzz`) Sửa một số nhân vật ZZZ thiếu Phim Ý Cảnh.
- (`/profile`) Giữ nguyên thứ tự các ký tự được truyền làm tham số..
- (`/gacha-log`) Hiển thị hình ảnh giữ chỗ cho các biểu tượng mục gacha bị thiếu.

## v1.16.19

### Tính năng mới

- (`/challenge hsr anomaly`) Giờ lấy dữ liệu từ 3 lần chạy gần nhất.
- (`/mimo`) Hỗ trợ hoàn thành các nhiệm vụ coi video bên Genshin.
- (`/notes`) Hỗ trợ nút mở ZZZ Bản Cloud Quốc Tế.
- (`/profile hsr`) Hiển thị Vạn Mệnh của Nhà Khai Phá thay vì yếu tố.

### Cải thiện

- (`/profile`) Thêm hỗ trợ cho các nhân vật HSR mới và Nhà Khai Phá - Vui Vẻ.
- (`/challenge zzz shiyu`) Ẩn chữ Thời gian hoàn thành trong các thẻ bố cục mới.

### Sửa lỗi

- (`/challenge hsr anomaly`) Sửa vị trí icon cho các khối ký tự trống.
- (`/profile zzz`) Sửa vị trí hiển thị hoặc thiếu hình ảnh skin cho nhân vật Aria và Nangong Yu.

## v1.16.18

### Tính năng mới

- (`/profile` ) Thêm hỗ trợ cho các nhân vật ZZZ 2.7 và HSR 4.1

## Sửa lỗi

- (`/characters zzz`) Sửa vấn đề hiệu năng khi có quá nhiều nhân vật.
- (`/events hsr`) Sữa Trọng Tài Dị Tướng hiển thị sai tên trong menu thả xuống.
- (`/card-settings`) Sửa lỗi truy vấn không hợp lệ cho ZZZ.
- (`/notes`) Khắc phục lỗi khi chuyển đổi tài khoản trong giao diện người dùng.
- (`/search`) Khắc phục lỗi khi tìm kiếm sách trong HSR.
- (`/profile zzz`) Sửa ảnh nhân vật Ảia hiển thi không chính sác trong thẻ đội hình.
- (`/profile zzz`) Sửa lỗi thiếu dử liệu thẻ skin nhân vận Pan Yinhu

## v1.16.17a

### Cải thiện

- Cập nhật tin nhắn mẹo "Bạn có biết" - ngày 1 tháng 4 năm 2026

## v1.16.17

### Tính năng mới

- (`/profile hsr`) Thêm hỗ trợ cho các nhân vật mới trong Honkai: Star Rail 4.0, bao gồm Vận Mệnh Vui Vẻ mới.
- (`/challenge zzz shiyu`) Thêm hỗ trợ cho Bảo Vệ Trụ Shiyu v2.
- (`/profile zzz`) Thêm dữ liệu thẻ cho các nhân vật ZZZ 2.6.

### Sửa lỗi

- (`/challenge zzz shiyu`) Sửa lỗi render thẻ và xử lý lỗi khi tải dữ liệu Bảo Vệ Trụ Shiyu.
- (`/characters hsr`) Sửa lỗi bộ lọc bị hỏng khi thiếu số lượng nhân vật theo vận mệnh.
- (`/events zzz`) Sửa lỗi phân tích đối tượng vũ khí.
- (`/profile hsr`) Sửa lỗi định dạng phần trăm xếp hạng cho các build hạng cao.
- (`/notes`) Sửa lỗi thiếu khoảng thời gian nhắc nhở Thể Lực cho Honkai Impact 3rd.
- Sửa lỗi xuống dòng trong ngôn ngữ zh-CN và các ngôn ngữ khác.

## v1.16.16

### Tính năng mới

- (`/profile zzz`) Thêm dữ liệu thẻ nhân vật ZZZ 2.5, bao gồm trang phục của Jane Doe.
- (`/profile hsr`) Thêm hỗ trợ ban đầu cho loại Vận Mệnh Vui Vẻ.
- (`/gacha-log`) Thêm hỗ trợ cho các loại banner mới của ZZZ (chỉ nhập chính thức).
- (`/build zzz`) Hiển thị tác giả hướng dẫn và ngày cập nhật cuối trong tổng quan.

### Cải tiến

- (`/build zzz`) Cải thiện khoảng cách và khả năng đọc của các phần hướng dẫn.

### Sửa lỗi

- (`/gacha-log upload`) Sửa lỗi nhập UIGF v4.1 không hoạt động.
- (`/notes`) Cho phép đặt thời gian thông báo ghi chú thực tế lên 0 giờ trước (tức là thông báo chính xác vào lúc đó).
- (`/mimo`) Vô hiệu hóa tính năng rút thăm tự động cho Genshin Du Lịch Mimo.
- (`/mimo`) Xử lý lỗi -510001 khi lấy nhiệm vụ của Genshin Du Lịch Mimo.

## v1.16.15

### Tính năng mới

- (`/build zzz`) Thêm lệnh để hiển thị build nhân vật cho ZZZ.
- (`/profile hsr`) Thêm dữ liệu thẻ The Dahlia.
- (`/mimo`) Bật lại hỗ trợ Mimo Du Lịch cho Genshin Impact.
- (`/mimo`) Thêm hỗ trợ cho các loại nhiệm vụ Mimo Du Lịch mới của Genshin Impact.
- Cải thiện phát hiện phông chữ để xử lý tốt hơn tiếng Ả Rập và các chữ viết không phải La-tinh.

### Cải tiến

- (`/profile hsr`) Cải thiện màu sắc thẻ của Dahlia.
- Triển khai cập nhật không gián đoạn – bot sẽ không còn bị offline trong quá trình cập nhật mã.

### Sửa lỗi

- (`/profile genshin`) Sửa KeyError khi chuyển đổi nhân vật Genshin Impact từ HoYoLAB.
- (`/gacha-log view`) Sửa lỗi thiếu biểu tượng vật phẩm cho nhật ký gacha HSR và ZZZ.
- (`/gacha-log view`) Sửa lỗi giao diện trên các thiết bị màn hình nhỏ.
- Sửa lỗi công tắc không trả về đúng `False` (Sai) khi tắt.
- Sửa một số vấn đề triển khai và lên lịch nội bộ.

## v1.16.14

### Tính năng mới

- (`/profile`) Thêm hỗ trợ các nhân vật mới cho ZZZ.
- (`/exploration`) Thêm các vùng mới.
- (`/events`) Thêm hỗ trợ cho ZZZ.

### Cải tiến

- (`/characters`) Mặc định lọc nhân vật theo cấp.
- (`/characters`) Thêm hiệu ứng phát sáng nhẹ của độ hiếm nhân vât cho nền thẻ nhân vật.
- (`/about`) Sử dụng URL giao thức Discord cho liên kết người dùng.
- Thêm nút cài đặt giả để diều hướng người dùng sử dụng `/settings`.

### Sửa lỗi

- (`/challenge genshin`) Sửa lỗi tràn văn bản cho thẻ Ảo Cảnh Hiểm Ác và thẻ Nhà Hát Giả Tưởng.
- (`/challenge genshin theater`) Sửa lỗi Thử Thách Thánh Bài không hiển thị khi ngôn ngử là Tiếng Việt.
- (`/challenge hsr anomaly`) Sửa lỗi tràn văn bản trong tên mùa.
- (`/settings`) Sửa lỗi không thể chọn tài khoản cho cài đặt Du Lịch Mimo.
- (`/settings`) Sửa lỗi tài khoản TOT có thể truy cập cài đặt nhắc nhở.
- (`/profile hsr`) Sửa lỗi vị trí vết tích trong thẻ nhân vật.
- (`/profile hsr`) Sửa lỗi thiếu biểu tượng thông kê cho một số nhân vật.
- (`/search`, `/profile zzz`) Sửa lỗi thiếu nhân vật như Ellen, Chiến Binh 11 trong tự động hoàn thành.
- (`/settings`) Sửa lổi cài đặt sai bị thay đổi khi nhấp vào các nút công tắc thông báo đổi quà.
- (`/profile zzz`) Sửa lỗi ảnh nhân vật Rina không được canh giữa trong thẻ đội.
- Đổi ẩn UID bằng ký tự 'x' thay vì '*' để tránh lỗi markdown.

## v1.16.13

### Tính năng mới

- (`/profile`) Hỗ trợ các nhân vật mới cho HSR và ZZZ.
- (`/challenge genshin theater`) Thêm hỗ trợ cho các Thử Thách Thánh Bài.
- (`/profile hsr`) Thêm thuộc tính nón ánh sáng cho các nhân vật HoYoLAB/Miyoushe.
- (`/challenge hsr anomaly`) Thêm hỗ trợ cho Trọng Tài Dị Tướng.
- (`/profile genshin`) Thêm hỗ trợ cho Người Mẫu Nam và Nữ.
- (`/gacha-log`) Thêm hỗ trợ cho Thiên Tinh Kỳ Vực.
- (`/settings`) Cải tiến giao diện người dùng cho lệnh cài đặt.

### Cải tiến

- (`/gacha-log view`) Cải tiến hiệu năng cho trình xem nhật ký Gacha.
- Cải tiến hiệu năng cho tự động điểm danh, tự động đổi mã, và các tác vụ tự động cho Mimo Du lịch.
- Cải thiện hiệu suất tổng thể của bot.

### Sửa lỗi

Có quá nhiều để liệt kê, vui lòng xem [toàn bộ nhật ký thay đổi (EN)](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.13).

## v1.16.12

Lưu Ý: Phiên bản này đã tạm thời vô hiệu hóa Du Lịch Mimo cho Genshin Impact do dich vụ gỡ bỏ bên HoYoLAB. Tính năng sẽ được kích hoạt lại khi dịch vụ được khôi phục.

### Tính năng mới

- (`/profile`) Thêm hỗ trợ cho các nhân vật mới trong ZZZ và HSR.
- (`/gacha-log import`) Sử dụng [script riêng](https://github.com/studiobutter/gacha-stuff) để nhập nhật ký Gacha.
- (`/challenge zzz shiyu`) Thay Thời Gian Hoàn Thành Nhanh Nhất cho Tổng Thời Gian Hoàn Thành.
- (`/challenge genshin stygian`) Thêm điểm yêu của kẻ thù và thông tin sức mạnh.
- Thêm hỗ trợ cho thành phố Nod-Krai.

### Cải tiến

- (`/profile`) Thêm khả năng xử lý lỗi mạnh mẽ hơn cho các yêu cầu API của Enka Network.
- (`/profile`) Thêm xử lý lỗi cho các yêu cầu API đội hình Enka Network.
- (`/profile`) Thêm xử lý lỗi cho API tạo thẻ của bên thứ ba.
- (`/accounts`) Xử lý lỗi API Discord OAuth2
- (`/notes`) Thêm mô tả cho các đầu vào khác nhau trong hộp thoại cài đặt lời nhắc.
- Do lỗi Discord, hình ảnh WEBP không thể sao chép được, vì vậy hiện tại chúng tôi gửi đồ họa thông tin dưới dạng PNG.

### Sửa lỗi

- (`/gacha-log view`) Sửa lỗi các nhân vật trong Duyên Phận Tinh Tú không được coi là 50/50 thua (lệch).
- (`/gacha-log view`) Sửa độ hiểm của vật phẩm không đúng cho một số vật phẩm trong ZZZ.
- (`/search`) Sửa lỗi các nhân vật ZZZ chưa phát hành thỉnh thoảng được hiển thị trong tự động hoàn thành.
- (`/upload`) Sửa vấn đề tải ảnh lên.
- (`/challenge genshin stygian`) Sửa lỗi tràn văn bản cho một số kẻ thù.
- (`/challenge zzz assault`) Sửa lỗi về truy cập icons bangboo cho những lần thử thách trước
- (`/gacha-log view`) Xử lý nhập loại banner không hợp lệ.
- (`/challenge`) Sửa lỗi vấn đề với menu thả xuống giai đoạn thử thách khi có hơn 25 thử thách.

## v1.16.11

### Tính năng mới

- (`/search`) Thêm Nhà Khai Phá (Băng).
- (`/accounts`) Thêm ID thiết bị cho đăng nhập bằng email, nên bạn có thể thấy thiết bị Hoyo Buddy trong Trung Tâm Tài Khoản HoYoverse.

### Sửa lỗi

- (`/profile zzz`) Thêm enka.py để hợp với định dạng API mới.
- (`/profile`) Sửa lỗi kết quả Enka luôn đưa ra bằng tiếng Anh.
- (`/exploration`) Sửa lỗi tràn văn bản cho Danh Vọng Bộ Tộc.
- Sửa lỗi phiên dịch với ngôn ngữ en-GB.

## v1.16.10

### Tính năng mới

- (`/profile hsr`) Hỗ trợ các nhân vật mới: Hysilens & Cerydra.
- (`/gacha-log upload`) Hiển thị lỗi khi tài khoản game và dữ liệu nhập từ game khác nhau.

### Cải tiến

- (`/gacha-log import`) Cải thiện hiệu năng nhập dữ liệu
- Lưu trữ dữ liệu thường dùng như cài đặt và cài đặt thẻ để cải thiện hiệu suất.
- Che đi 5 số trong UID thay vì 3.

### Sửa lỗi

- (`/profile zzz`) Sửa lỗi thiếu hình ảnh trang phục cho thẻ đội hình.
- (`/profile zzz`) Sửa lỗi thiếu dữ liệu cho Trang Phục Mùa Hè của Alice
- (`/profile zzz`) Sửa lỗi gây ra bởi dữ liệu trang phục
- (`/profile zzz`) Sửa lỗi các build trên Enka Network thỉnh thoảng không hiện lên.
- (`/search`) Sửa lỗi "nội dung chưa phát hành" được hiển thị trong tìm kiếm tự động hoàn thành bình thường

## v1.16.9

### Tính năng mới

- (`/profile zzz`) Thêm hỗ trợ cho Enka Network.
- (`/about`) Thêm links vào trong lệnh.
- Thêm lệnh `/changelog`, `/invite` và `/help`.
- Thêm hỗ trợ cho Wiki với ngôn ngữ Trung Quốc Giản Thể và Tây Ban Nha.
- Thêm [trang trạng thái](https://status.seria.moe/?category=Hoyo%20Buddy) để kiểm tra trạng thái bot.

### Cải tiến

- (`/settings`) Lệnh này bây giờ chỉ bạn có thể thấy thôi.

### Sửa lỗi

- (`/accounts`) Sửa lỗi về vấn để đăng nhập
- (`/gacha-log manage`) Sửa lỗi vật sai hạng cho tính năng xuất của ZZZZ
- (`/gacha-log view`) Sửa lỗi tên vật là "???" cho banner Hợp Tác Nhân Vật và Nón Ánh Sáng của HSR.
- (`/profile genshin`) Sửa lỗi tin nhắn nhúng không có người chơi được hiển thị khi nguồn dữ liệu chính là HoYoLAB

## v1.16.8

### Tính năng mới

- (`/challenge zzz shiyu`) Thêm thời gian hoàn thành.
- (`/challenge hsr`) Ẩn Màn Hoàn Thành Nhanh.
- (`/challenge hsr`) Thêm lựa chọn "Hiển thị UID".
- (`/gacha-log`) Hổ trợ banner hợp tác HSR
- (`/profile zzz`) Thêm hỗ trợ nhân vật mới: Alice và Yuzuha.
- (`/profile zzz`) Thêm hỗ trợ cho trang phục nhân vật.
- Bot sẽ không ngoại tuyến khi cập nhật mã nguồn.

### Cải tiến

- (`/profile hsr`) Cải thiện vị trí chữ cho Mẩu thẻ 2.
- (`/events`) Cải thiện độ tương phản màu sắc trong chế độ sáng.
- (`/gacha-log view`) Thay đổi đường dẫn ứng dụng web khi đổi loại banner.
- (`/search`) Câu chuyên nhân vật HSR giờ hiển thị một cách gọn gàng hơn.
- Cải thiện hiệu suất tính năng tạo ảnh bằng bộ nhớ đệm tốt hơn.
- Lưu ảnh dưới dạng webp thay vì png để giảm kích thước của tập tin.

### Sửa lỗi

- (`/redeem`) Sửa lỗi mã viết thường không tính là đã đổi.
- (`/characters genshin`) Sửa một vài vấn đề về vị trí chữ.
- (`/characters genshin`) Sữa ảnh của một số nhân vật được hiển đưới phong cách khác
- (`/profile hsr`) Sửa một số lỗi phong chứ trong tên của nón ánh sáng trong mẫu thẻ 2

## v1.16.7

### Tính năng mới

- Thêm hỗ trợ Tiếng Ả Rập
- (`/challenge genshin`) Thêm tính năng tạo thẻ Ảo Cảnh Hiểm Ác
- (`/profile zzz`) Thêm từ viết tắt cho "Tự Tích Thiểm Năng" cho mẫu thẻ 4.

### Cải tiến

- (`/accounts`) Hiển thị một trang khi lấy tài khoản.
- (`/accounts`) Cập nhật đường dẫn file APK cho đăng nhập bằng Miyoushe.
- (`/accounts`) Cập nhật đường dẫn URL cho đăng nhập qua Miyoushe.
- (`/accounts`) Thêm trường nhập dữ liệu cho aaid khi thêm tài khoản Miyoushe.
- Tạo hình ảnh nhanh hơn bằng cách sử dụng nhiều lõi CPU.
- Vị trí văn bản trong hình ảnh chính xác hơn.

### Sửa lỗi

- (`/profile zzz`) Sửa vị trí hình ảnh của Yixuan cho mẫu thẻ 1.
- (`/profile zzz`) Sửa lỗi thuộc tính "Xuyên Giáp" không được dịch ở mẫu thẻ 4.
- (`/search`) Vô hiệu hóa mục La Hoàn Thâm Cảnh.
- (`/search`) Sửa lỗi không có lựa chọn tự động hoàn thành cho danh mục đĩa.

## v1.16.6

### Tính năng mới

- (`/profile zzz`) Hỗ trợ dữ liẹu nhân vật ZZZ v2.0.
- (`/profile zzz`) Thêm hỗ trợ cho Người Đại Diên Mệnh Phá và dữ liệu Lục Quán Xuyến.
- (`/gacha-log import`) Xử lý các ngoại lệ authkey.
- Thêm ngày kỷ niệm có thể bỏ qua.

### Cải tiến

- (`/profile zzz`) Bỏ khoảng cách trong tên Người Đại Diện trong nền.

### Sửa lỗi

- (`/characters genshin`) Xử lý nhân vật không có nguyên tố.
- (`/challenge genshin theater`) Xử lý ID không hợp lệ của các nhân vật.

## v1.16.5

### Tính năng mới

- (`/profile hsr`) Thêm dử liệu thẻ nhân vật v3.3
- (`/profile hsr`) Thêm hỗ trợ cho nhân vật đi Vận Mệnh Ký Ức để sử dụng mẫu thẻ StarRailCard.
- (`/profile`) Xử lý lỗi thời gian chờ yêu cầu API của Enka Network.
- (`/search`) Bật lại danh mục nội dung chưa phát hành.

### Sửa lỗi

- (`/redeem`) Xóa tham số 'người dùng' khỏi lệnh.
- (`/mimo`) Xóa mờ UID khi nhúng tác vụ Mimo Du Lịch tự động.
- (`/upload`) Xử lý các tệp hình ảnh quá lớn.
- (`/search`) Sửa lỗi công thức tính toán không chính xác cho chỉ số nhân vật và hình nón ánh sáng.
- (`/accounts`) Sửa lỗi tùy chọn 'trang tiếp theo' không hoạt động khi người dùng có hơn 25 tài khoản.

## v1.16.4

### Tính năng mới

- (`/profile genshin`) Hỗ trợ Nhà Lữ Hành không nguyên tố.
- Thêm phông chữ Hindi.

### Cải tiến

- (`profile`) Loại bỏ dữ liệu nhân vật từ bộ nhớ đệm.
- Thêm hạn chế cho bộ lọc nhật ký Gacha

### Sửa lỗi

- (`/events`) Sữa lỗi không tìm thấy banner thông báo.
- (`/challenge genshin theater`) Sữa lỗi không hiển thị dử liệu Nhà Hát Giả Tưởng.
- (`/profile`) Sữa lỗi tương thích liên quan đến Build trên Enka Network.
- (`/mimo`) Sửa lỗi người dùng Miyoushe có thể truy cập lệnh.
- (`/notes`) Bỏ qua lỗi bảo trì khi kiểm tra ghi chú thời gian thực.
- (`/lb view`) Loại bỏ bảng xếp hạng thành tựu cho Honkai Impact 3
- (`/farm reminder`) Đã sửa lỗi tên mục là "..."

## v1.16.3

### Tính năng mới

- (`/profile zzz`) Đã thêm dữ liệu thẻ của Vivian & Hugo.
- Đã thêm bản dịch tiếng Bồ Đào Nha (Brazil).
- Đã thêm bản dịch tiếng Nhật.

### Cải tiến

- (`/profile zzz`) Đã điều chỉnh vị trí hình ảnh của một số nhân vật.
- (`/profile zzz`) Các lớp hình ảnh được cải thiện cho các mẫu thẻ.

### Sửa lỗi

- (`/notes`) Đã sửa lỗi thông báo biến áp tham số không hoạt động.
- (`/gacha-log upload`) Đã sửa lỗi độ hiếm của mục sai đối với một số phương thức nhập ZZZ.

## v1.16.2

### Tính năng mới

- (`/profile hsr`) Thêm dữ liệu thẻ cho Castorice & Anaxa.

### Sửa lỗi

- (`/profile zzz`) Sửa vị trí thẻ hình của Pulchra trong Mẫu thẻ Hoyo Buddy 2.
- (`/build genshin`) Sửa lỗi di vật vị trí emoji không được hiển thị đúng cách trong ứng dụng của tôi.

## v1.16.1

### Tính năng mới

- (`/gacha-log upload`) Thêm hỗ trợ nhập dữ liệu gacha từ trình khởi chạy [Starward](https://github.com/Scighost/Starward)
- (`/redeem`) Thêm cài đặt thông báo
- (`/accounts`) Thêm hướng dẫn để lấy aaid để thêm các tài khoản Miyoushe.
- Thêm nút ẩn UI

### Cải Tiến

- (`/search`) Đã xóa danh mục "nội dung chưa phát hành", hãy xem [tin nhắn này](https://discord.com/channels/1000727526194298910/1042428379120545873/1346413266737561660) để biết lý do.
- (`/characters`) Cho phép không chọn gì cho các bộ lọc.
- Tăng hiệu suất cho các tác vụ tự động.

### Sửa Lỗi

Đã sửa nhiều lỗi khác nhau, hãy xem [nhật ký thay đổi đầy đủ](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.1) để biết thêm chi tiết.

## v1.16.0

### Tính năng mới

- (`/profile`) Thêm Xem trước Mẫu thẻ trong cài đặt thẻ
- (`/profile`) Hiển thị ảnh tùy chỉnh sẵn có trong menu mẫu thẻ
- (`/notes`) Tăng giới hạn Sức mạnh Khai Phá lên 300.
- (`/notes`) Thêm nút mở trò chơi.
- (`/search zzz`) Thêm menu cấp độ Kỹ Năng Cốt Lõi.
- (`/gacha-log import`) So sánh UID của nhật ký đến với UID của tài khoản đang được nhập vào.
- Tự động cài đặt ngôn ngữ của người dùng mới dựa trên ngôn ngữ của ứng dụng Discord.

### Cải Tiến

- (`/redeem`) Cải thiện UX bằng cách sữa không phản hồi khi đang đổi mã.
- (`/gacha-log`) Làm tham số tài-khoản bắt buộc để tránh sự bối rối.
- Hiển thị thông báo lỗi tốt hơn cho lỗi "Thiếu quyền" và "Tin nhắn bị AutoMod chặn".
- Hiển thị văn bản đơn giản trong quá trình thiết lập tài khoản.

### Sửa Lỗi

- Sửa nhiều lỗi và cải tiến.
- Cải thiện phiên dịch Tiếng Việt.

## v1.15.7

### Tính năng mới

- (`/web-events`) Đã thêm lệnh mới để xem các sự kiện web đang diễn ra và đặt thông báo để nhắc bạn khi có sự kiện mới.
- (`/notes`) Thêm nhắc nhở Tiến Độ Ủy Thác Trao Thưởng and Điểm Số Ridu Hàng Tuần cho ZZZ.
- (`/about`) Thêm nút Nhật Ký Cập Nhật.

### Cải Tiến

- (`/gacha-log view`) Cải thiện hiệu suất trang nhật ký gacha bằng cách khắc phục sự cố bộ đệm.
- (`/about`) Đã loại bỏ các thay đổi git mới nhất.
- (`/mimo`) Sắp xếp các mặt hàng của Du Lịch Mimo shop từ đắt nhất đến rẻ nhất khi tự động mua.
- Cải thiện các phiên dịch của các ngôn ngữ khác.
  
### Sửa Lỗi

- (`/characters genshin`) Sửa lỗi KeyError gây ra bởi Nhà Lữ Hành Không Nguyên Tố.
- (`/characters genshin`) Sửa cấp độ Thiên Phú không chính sác cho Kamisato Ayaka.
- (`/stats`) Sửa lỗi "Không tìm thấy bản ghi thẻ cho ..." cho ZZZ.
- (`/build genshin`) Sửa lỗi "Không có danh sách khối để vẽ".
- (`/gacha-log view`) Sửa lỗi tỉ lệ thắng 50/50 không chính sác.
- (`/gacha-log view`) Sửa lỗi xác thực 422 trên ứng dụng web.
- (`/gacha-log view`) Xử lý kích thước đầu vào không hợp lệ.
- (`/gacha-log import`) Xử lý các loại Banner không hợp lệ khi nhập nhật ký gacha.
- (`/gacha-log import`) Sữa lỗi nhập UIGF.
- (`/mimo`) Xác nhận trạng thái nhiệm vụ hoàn thành trước khi gửi thông báo.
- (`/mimo`) Đã thêm khoảng thời gian ngủ giữa các lần hoàn thành nhiệm vụ để tránh bị giới hạn tốc độ.
- (`/mimo`) Loại bỏ thẻ HTML trên tên nhiệm vụ.
- (`/mimo`) Sửa lỗi sau khi mua một vật phẩm.
- (`/profile`) Sửa lỗi cài đặt thẻ từ các trò chơi khác bị trùng lập.
- (`/profile genshin`) Sửa lỗi Thiên Phú bổ sung được hiển thị trong thẻ đội.
- (`/profile genshin`) Sửa lỗi xác nhận cho nhân vật Mavuika.
- (`/search`) Đã sửa lỗi bộ chọn tinh chỉnh W-Engine không cập nhật giá trị đã chọn.
- (`/notes`) Sửa lỗi xác nhận cho Honkai Impact 3.
- (`/challenge zzz assault`) Đã sửa lỗi biểu tượng buff không được hiển thị.

## v1.15.6

### Tính năng mới

- (`/mimo`) Thêm hỗ trợ cho Genshin Du Lịch Mimo (sự kiện đã kết thúc từ thời điểm viết).
- (`/mimo`) Đã thêm tính năng rút thưởng tự động.
- (`/challenge zzz`) Thêm hỗ trợ cho Tập Kích Nguy Cấp.
- (`/profile hsr`) Thêm Mẫu thẻ 2.
- (`/notes`) Thêm thông tin Tiến Độ Ủy Thác Treo Thưởng và Điểm Số Ridu Hàng Tuần cho ZZZ

## Cải Tiến

- (`/check-in`) Giảm các yêu cầu API điểm danh trùng lặp.

## Sửa Lỗi

- (`/mimo`) Sửa lỗi gửi thông báo khi không có nhiệm vụ nào được hoàn thành và không có điểm nào được nhận.
- (`/mimo`) Sửa lỗi cách xác định các vật phẩm có giá trị.
- (`/mimo`) Xử lý lỗi -510001.
- (`/mimo`) Đã khắc phục sự cố trong đó các vật phẩm có giá trị được tính làm đồ trang trí cho HSR.
- (`/mimo`) Vô hiệu hóa nút rút thăm xổ số khi đạt đến giới hạn.
- (`/challenge zzz`) Sửa lỗi icon Bangboo sai trong thẻ.
- (`/events`) Sửa lỗi tiến trình của La Hoàn Thâm Cảnh.
- (`/gacha-log view`) Đã sửa lỗi số lần quay gacha từ độ hiếm cuối cùng.
- Đã sửa lỗi logic tạo thư mục hình ảnh tĩnh.

## v1.15.5

### Tính năng mới

- (`/mimo`) Tự động hoàn thành tác vụ yêu cầu bình luận trên một bài viết.
- (`/mimo`) Tự động hoàn thành tác vụ yêu cầu theo dõi một đề mục.
- (`/mimo`) Thêm tính năng rút thưởng.
- (`/mimo`) Thêm cài đặt thông báo.
- (`/profile zzz`) Thêm cài đặt hình ảnh để sử dùng ảnh Phim Ý Cảnh 3 cho thẻ nhân vật.
- (`/profile zzz`) Thêm dử liệu nhân vật Harusama và Miyabi
- (`/search`) Ẩn mục "nội dung chưa phát hành" trong một số máy chủ.

### Cải Tiến

- (`/mimo`) Hiển thị tiến độ tác vụ cho một số tác vụ nhất định.
- (`/mimo`) Hiển thị tên các tác vụ đã hoàn thành trong thông báo.
- (`/mimo`) Cải thiện hiệu suất của các tác vụ tự động.
- (`/challenge zzz shiyu`) Cập nhật bố cục của thẻ.
- (`/challenge zzz shiyu`) Tranh lấy dữ liệu người đại diện hai lần.
- Hiển thị liên kết mời máy chủ Discord trong phần chân trang bị lỗi.
- Bỏ đặt trạng thái tải mục khi có lỗi.
- Thêm nhãn bật/tắt cho các nút chuyển đổi.
- Logic yêu cầu API proxy được cải thiện.
- Cải thiện logic xử lý lỗi tác vụ tự động.

### Sửa Lỗi

- (`/mimo`) Đã thêm khoảng thời gian ngủ sau khi đổi mã quà tặng phần thưởng MMimo.
- (`/mimo`) Sửa lỗi tác vụ bị thiếu trong danh sách tác vụ.
- (`/mimo`) Sửa lỗi nhiệm vụ bình luận không được hoàn thành.
- (`/mimo`) Sửa lỗi gửi thông báo khi không có nhiệm vụ nào được hoàn thành.
- (`/mimo`) Chỉ hiển thị tài khoản HoYoLAB trong phần tự động điền.
- (`/mimo`) Sửa lỗi `QuerySetError` trong các tác vụ tự động.
- (`/mimo`) Đã sửa lỗi bình luận bài viết không bị xóaa.
- (`/mimo`) Xử lý các trường hợp Mimo Du Lịch không có sẵn cho trò chơi.
- (`/profile zzz`) Sửa lỗi điểm nổi bật của chỉ số phụ không được thêm vào thẻ.
- (`/profile zzz`) Sửa lỗi người đại diện được xác định là được lưu trong bộ nhớ đệm trong khi thực tế không được lưu.
- (`/characters zzz`) Sữa lỗi đếm sai số lượng người đại diện.
- (`/gacha-log upload`) Đã khắc phục sự cố khi nhập Nhật ký Gacha từ zzz.rng.moe.
- (`/redeem`) Sửa lỗi tài khoản Miyoushe được hiển thị trong tự động điền.
- (`/build genshin`) Xử lý tỷ lệ sử dụng bị thiếu đối với một số ký tự.
- (`/events`) Đã sửa lỗi các banner Bước Nhảy HSR trong tương lai được hiển thị là "chưa có sẵn".
- Thích ứng với các khóa ZenlessData mới.
- Đã khắc phục sự cố với API Hakushin.
- Nắm bắt các ngoại lệ chung trong phương thức `dm_user`.

## v1.15.4

### Tính năng mới

- (`/build genshin`) Hiển thị thông tin về sức mạnh tổng hợp của một nhân vật.
- (`/mimo`) Thêm lênh quản lý Mimo Du Lịch

### Cải Tiến

- (`/build genshin`) Cải thiện thiết kế thẻ nhân vật
- (`/notes`) Sử dụng API Lịch Sự Kiện để kiểm tra Sự kiện Vị Diện Nứt Vỡ.

### Sửa lỗi

- (`/build genshin`) Sửa một số vấn đề về UI.
- (`/events`) Sửa một số vấn đề làm cho lệnh không thể truy cập được.
- (`/gacha-log upload`) Sửa lỗi `ValidationError` với dữ liệu UIGF.
- (`/gacha-log upload`) Sửa lỗi `KeyError` với UIGF phiên bản cũ hơn 3.0.
- (`/search`) Sửa các lựa chọn tự động hoàn thành trùng lặp.

## v1.15.3

Lỗi code trong phiên bản trước đã xẩy ra lỗi "nhiều yêu cầu quá, vui lòng thử lại" khi người dùng đăng nhập, vui lòng xem [bài đăng này](./too-many-requests.md) để biết thêm thông tin.

### Tính năng mới

- (`/profile zzz`) Thêm bộ chọn để chọn thuộc tính phụ mà bạn muốn tô đậm.
- (`/profile hsr`) Thêm dữ liệu thẻ Fugue và Sunday.

### Cải Tiến

- (`/redeem`) Ẩn link mã đổi bằng chính mã đó.
- (`/challenge genshin theater`, `/challenge genshin abyss`) Hiển thị nguyên tố Nhà Lữ Hành trong thẻ.
- (`/accounts`) Thêm thông báo lỗi tùy chỉnh cho lỗi "nhiều yêu cầu quá".

### Sửa lỗi

- Sửa lỗi nơi các lệnh không được dịch sang ngôn ngữ khác.
- Sửa lỗi nơi các cách thức hết thời gian chờ không được đóng đúng cách.
- Sửa API logic thử lại và logic xử lý lỗi.
- Sửa lỗi `ValueError` trong một số lệnh.
- Sửa lỗi cách thức hết thời gian chờ quá ngắn.
- Xử lý lỗi `KeyError` trong điểm cuối chuyển hướng máy chủ web.
- (`/profile`) Xử lý lỗi `EnkaAPIError` khi lấy dữ liệu từ Enka Network API.
- (`/profile`) Xử lý lỗi Enka Network API hết thời gian chờ cổng kết nối một cách nhẹ nhàng.
- (`/profile`) Sửa lỗi `BadRequestError` khi tạo ảnh AI.
- (`/profile`) Sửa lỗi `BadRequestError` khi tải ảnh lên.

## v1.15.2 và trước đó

Các nhật ký thay đổi trước đó đã được viết trong kênh #updates trong [Máy chủ Discord](https://link.seria.moe/hb-dc) của chúng tôi.
