# Prioritized Product Backlog bằng MoSCoW: hệ thống mượn sách online (Release 1)

**Dữ liệu đề cho:** năng lực Release 1 khoảng **20 điểm**, tổng 12 hạng mục là **25 điểm** (S = 1, M = 2, L = 3). Must tối đa 5 hạng mục và khoảng 60% năng lực (khoảng 12/20 điểm).

---

## 1. Bảng phân loại 12 hạng mục kèm lý do

| # (đề) | Hạng mục | Điểm | Nhóm | Lý do (1 câu) |
|---|---|---|---|---|
| 1 | Đăng nhập/đăng ký tài khoản độc giả | 2 | **Must** | Cần biết ai đang mượn thì mới mượn và giới hạn số sách được, nên mọi hạng mục khác phụ thuộc vào nó. |
| 2 | Tìm kiếm sách theo tên/tác giả | 2 | **Must** | Độc giả không tìm được sách thì không có gì để mượn, và không có cách thay thế trên hệ thống online. |
| 3 | Mượn sách online (có giới hạn số sách) | 3 | **Must** | Là giá trị cốt lõi của MVP, thiếu thì hệ thống không còn là hệ thống mượn sách. |
| 4 | Gia hạn mượn sách online | 1 | **Should** | Quan trọng nhưng có cách tạm: độc giả đến quầy hoặc hỏi thủ thư để gia hạn. |
| 5 | Đặt trước sách khi hết (kèm thông báo) | 2 | **Should** | Giải quyết sách đang hết, nhưng bản phát hành vẫn dùng được nếu thiếu (độc giả tự quay lại kiểm tra), và phụ thuộc vào mục 3. |
| 6 | Đánh giá và bình luận sách sau khi đọc | 2 | **Could** | Không ảnh hưởng việc mượn trả, bỏ đi ít tác động, và còn phải kiểm duyệt nội dung. |
| 7 | Gợi ý sách theo sở thích cá nhân | 3 | **Won't** (lần này) | Tốn 3 điểm và cần dữ liệu lịch sử mượn mà bản đầu chưa có, nên chưa đáng làm ở Release 1. |
| 8 | Thông báo email khi sắp đến hạn trả | 1 | **Should** | Giúp giảm trả muộn, nhưng thủ thư vẫn có thể nhắc thủ công. |
| 9 | Xem lịch sử mượn sách của bản thân | 1 | **Should** | Tiện lợi, có cách tạm là hỏi thủ thư, chi phí thấp. |
| 10 | Thủ thư quản lý kho sách (thêm/sửa/xóa) | 3 | **Must** | Không có sách trong hệ thống thì không tìm kiếm và mượn được, và không có cách tạm trên hệ thống mới. |
| 11 | Chat trực tiếp với thủ thư | 3 | **Won't** (lần này) | Đã có cách thay thế (gọi điện, email, đến quầy), tốn 3 điểm và cần thủ thư trực liên tục. |
| 12 | Tích hợp đăng nhập Google/Facebook | 2 | **Could** | Đã có đăng ký thường nên thiếu vẫn dùng được, tích hợp bên thứ ba tốn 2 điểm và thêm rủi ro. |

**Tổng theo nhóm:**

| Nhóm | Hạng mục | Điểm |
|---|---|---|
| Must | 1, 2, 3, 10 | 2 + 2 + 3 + 3 = **10** |
| Should | 4, 5, 8, 9 | 1 + 2 + 1 + 1 = **5** |
| Could | 6, 12 | 2 + 2 = **4** |
| Won't | 7, 11 | 3 + 3 = **6** |
| **Tổng** | 12 hạng mục | **25** |

---

## 2. Tổng điểm công sức nhóm Must

**Must = 10 điểm = 10 / 20 = 50% năng lực Release 1, gồm 4 hạng mục.**

- **Nằm trong ngưỡng:** thấp hơn mức trần khoảng 60% (12 điểm) và không vượt giới hạn 5 hạng mục.
- Mình không nâng thêm hạng mục lên Must chỉ để "đủ 60%". Hạng mục thứ năm gần nhất là mục 5 (đặt trước), nhưng nó có cách tạm nên đúng nghĩa là Should.
- Should và Could (9 điểm) cộng với Must (10 điểm) là 19 điểm, vừa năng lực 20 điểm. Should và Could là **vùng đệm**: nếu trễ tiến độ thì cắt Could trước (mục 10 rồi mục 9), sau đó cắt Should từ cuối lên.

---

## 3. Product Backlog có thứ tự (1 đến 12)

| Thứ tự | Hạng mục (# đề) | Nhóm | Điểm | Phụ thuộc và lý do đứng ở vị trí này |
|---|---|---|---|---|
| 1 | Đăng nhập/đăng ký (#1) | Must | 2 | Nền tảng, mọi hạng mục khác cần biết người dùng. |
| 2 | Thủ thư quản lý kho sách (#10) | Must | 3 | Phải có sách trong hệ thống trước khi tìm kiếm và mượn. |
| 3 | Tìm kiếm sách (#2) | Must | 2 | Phụ thuộc #2 (có sách để tìm), là bước độc giả cần trước khi mượn. |
| 4 | Mượn sách online (#3) | Must | 3 | Phụ thuộc đăng nhập, kho sách và tìm kiếm. Là giá trị cốt lõi. |
| 5 | Đặt trước sách khi hết (#5) | Should | 2 | Phụ thuộc mượn sách. Giá trị cao nhất trong Should vì giải quyết trường hợp sách hết. |
| 6 | Thông báo email sắp đến hạn trả (#8) | Should | 1 | Phụ thuộc mượn sách (cần có hạn trả). Rẻ và giảm rủi ro trả muộn. |
| 7 | Gia hạn mượn sách (#4) | Should | 1 | Phụ thuộc mượn sách. Rẻ, đi cùng thông báo sắp đến hạn. |
| 8 | Xem lịch sử mượn (#9) | Should | 1 | Phụ thuộc mượn sách. Tiện ích, đứng cuối Should vì ít khẩn cấp nhất. |
| 9 | Đăng nhập Google/Facebook (#12) | Could | 2 | Phụ thuộc đăng nhập (đã ở vị trí 1). Giảm rào cản đăng ký, ít rủi ro hơn mục 10. |
| 10 | Đánh giá và bình luận (#6) | Could | 2 | Phụ thuộc đăng nhập và mượn sách. Cần thêm kiểm duyệt nội dung. |
| 11 | Gợi ý sách theo sở thích (#7) | Won't | 3 | Phụ thuộc dữ liệu lịch sử mượn (vị trí 8 và 4). Nên xem xét sớm nhất ở bản sau. |
| 12 | Chat trực tiếp với thủ thư (#11) | Won't | 3 | Phụ thuộc đăng nhập. Tốn nhân lực trực, xem xét sau. |

**Kiểm tra quy tắc phụ thuộc:** mọi hạng mục phụ thuộc đều có hạng mục mà nó cần ở nhóm cao hơn hoặc cùng nhóm và **đứng trước** nó (ví dụ #5 đặt trước ở vị trí 5, sau mượn sách ở vị trí 4). Hai hạng mục Won't (#7, #11) vẫn được giữ trong backlog và chỉ đánh dấu chưa làm ở giai đoạn này.

---

## 4. Tự phản biện

Người khác có thể xếp mục 12 (đăng nhập Google/Facebook) lên Should vì nó giảm rào cản đăng ký và tăng số độc giả, nhưng mình giữ Could vì đã có đăng ký thường, thiếu vẫn dùng được, và tích hợp bên thứ ba tốn 2 điểm kèm rủi ro. Với mục 11 (chat), người ta có thể lập luận chat giúp độc giả hỏi nhanh nên là Should, nhưng mình xếp Won't vì đã có cách thay thế (gọi điện, email, đến quầy), tốn 3 điểm và cần thủ thư trực liên tục. Với mục 7 (gợi ý sách), có thể lập luận gợi ý làm tăng lượt mượn nên là Could, nhưng bản đầu chưa có dữ liệu lịch sử và hạng mục tốn 3 điểm. Nếu có thêm bằng chứng, ví dụ khảo sát cho thấy phần lớn độc giả muốn đăng nhập bằng Google hoặc nhóm còn dư năng lực, mình sẵn sàng đổi nhãn, và các mục Won't vẫn được giữ trong backlog cho bản sau.
