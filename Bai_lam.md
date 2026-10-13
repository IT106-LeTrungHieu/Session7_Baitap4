# BÀI TẬP 4 – CHỌN CÁCH DỰ BÁO PHẠM VI CHO SPRINT 6

**Vai trò:** Vy (Developer), phối hợp với Lan (Scrum Master) chuẩn bị phương án cho Sprint Planning.

## Phần 1 – Đề xuất hai cách dự báo

### 1. Cơ sở chung

- Velocity của 5 Sprint gần nhất: **18, 20, 19, 15, 13 SP**; chỉ tính các PBI đạt Definition of Done.
- Average Velocity: **(18 + 20 + 19 + 15 + 13) / 5 = 17 SP/Sprint**.
- Velocity Range quan sát được: **13–20 SP**. Hai Sprint gần nhất đạt 15 và 13 SP, cho thấy kết quả gần đây thấp hơn trung bình 5 Sprint.
- Planning Capacity Sprint 6: **186 giờ**, giảm **26 giờ**, tương đương **26 / 212 × 100 ≈ 12,3%** so với Sprint 5. Con số 186 giờ đã tính thời gian làm quen của Minh và 3 ngày nghỉ của Hà, nên không trừ thêm lần nữa.
- Capacity là thời gian sẵn có trong Sprint tới; Velocity là lượng SP đã Done trong quá khứ. **Không quy đổi SP sang giờ và không suy ra Velocity phải giảm đúng 12,3%.** Việc thay Khoa bằng Minh còn tạo ra bất định về kiến thức dự án và phối hợp.

### 2. Cách A – Lấy Average Velocity làm mốc, chọn tổ hợp PBI đủ rõ gần mốc

**Bản chất:** Dự báo từ kết quả trung bình trong quá khứ, sau đó chọn các PBI đủ rõ, có tổng SP gần nhưng không vượt mốc 17 SP. Đây là phương án đơn giản để đem ra so sánh; chưa điều chỉnh đầy đủ theo Capacity và rủi ro nhân sự.

**Dự báo phạm vi: 15 SP**, gồm:

| Thứ tự trong Product Backlog | PBI | SP | Căn cứ chọn |
|---|---|---:|---|
| 1 | Hẹn giờ đặt xe trước | 5 | Acceptance Criteria đầy đủ; giúp khách chủ động thời gian đặt xe. |
| 3 | Gửi SMS khi tài xế sắp đến | 3 | Hợp đồng SMS đã ký; hỗ trợ khách trong lúc chờ. |
| 4 | Chat với tài xế | 5 | Acceptance Criteria đầy đủ; hỗ trợ trao đổi khi chờ. |
| 5 | Giao diện chủ đề Tết | 2 | Acceptance Criteria đầy đủ; được chọn thêm để tổng phạm vi gần mốc trung bình. |
| | **Tổng** | **15** | |

17 SP là mốc tham khảo, còn 15 SP là tổng của tổ hợp PBI thực tế được đề xuất. Không thêm PBI chưa rõ chỉ để đạt đúng 17 SP. Phương án này có nhược điểm là chọn thêm giao diện Tết dù đóng góp ít cho mục tiêu giúp khách chủ động khi chờ tài xế.

### 3. Cách B – Dự báo theo Sprint Goal và Capacity, đối chiếu Velocity Range

**Bản chất:** Bắt đầu từ kết quả khách hàng cần đạt, chọn PBI phục vụ kết quả đó và đủ rõ, rồi để Developers kiểm tra khả năng hoàn thành bằng kế hoạch công việc trong Capacity 186 giờ. Velocity Range và các Sprint gần nhất chỉ là dữ liệu đối chiếu mức hợp lý, không phải công thức tính phạm vi.

**Dự báo phạm vi ban đầu: 13 SP**, gồm:

| Thứ tự trong Product Backlog | PBI | SP | Căn cứ chọn |
|---|---|---:|---|
| 1 | Hẹn giờ đặt xe trước | 5 | Giúp khách chủ động lên kế hoạch chuyến đi. |
| 3 | Gửi SMS khi tài xế sắp đến | 3 | Giúp khách biết thời điểm cần chuẩn bị đón xe. |
| 4 | Chat với tài xế | 5 | Giúp khách trao đổi trực tiếp về điểm đón và việc chờ xe. |
| | **Tổng** | **13** | |

13 SP nằm ở đầu thấp của khoảng 13–20 SP, bằng kết quả Sprint 5 và phù hợp với hướng thận trọng khi Capacity giảm, đội đổi thành viên. Đây là **dự báo có điều kiện**, không phải khẳng định 186 giờ chắc chắn hoàn thành 13 SP. Trong Planning, Developers cần phân rã công việc, xem phụ thuộc, công việc kiểm thử/tích hợp và khả năng hỗ trợ Minh; nếu kế hoạch chưa khả thi thì thương lượng giảm phạm vi với Đức.

### 4. Xử lý PBI số 2 và thứ tự Product Backlog

**Chưa chọn “Theo dõi vị trí tài xế trên bản đồ” (13 SP) ở cả hai cách**, vì chưa có Acceptance Criteria cho trường hợp mất tín hiệu GPS. PBI này vừa lớn vừa thiếu rõ ràng, nên đưa vào ngay sẽ tạo rủi ro cho Sprint Goal; việc nó đứng thứ 2 không tự động khiến nó phù hợp để nhận vào Sprint.

Vy và Lan đề xuất Đức cùng Developers làm rõ hành vi khi mất GPS, cách thông báo cho khách và điều kiện kiểm thử; cân nhắc tách thành các PBI nhỏ có giá trị và ước lượng lại. Việc chọn các PBI số 3 và 4 khi PBI số 2 chưa rõ cần được trao đổi với Đức trong Planning. Các PBI chưa Done của Sprint 5 đã trở lại Product Backlog, không tự động chuyển sang Sprint 6; đề bài cũng chưa cung cấp nội dung và SP để đưa chúng vào dự báo.

## Phần 2 – So sánh hai cách

| Tiêu chí | Cách A: Average Velocity → 15 SP | Cách B: Sprint Goal + Capacity, đối chiếu Velocity Range → 13 SP |
|---|---|---|
| Phản ánh thay đổi Capacity | **Nhược điểm (–):** Mốc 17 SP tổng hợp cả các Sprint có điều kiện nhân sự khác; chưa phản ánh đầy đủ Capacity giảm và thời gian làm quen của Minh. | **Ưu điểm (+):** Kiểm tra kế hoạch theo 186 giờ, ngày nghỉ và thay đổi nhân sự; dùng lịch sử để đối chiếu, không giảm SP theo một tỷ lệ máy móc. |
| Bảo vệ Sprint Goal | **Nhược điểm (–):** Có 3 PBI phục vụ sự chủ động của khách, nhưng thêm giao diện Tết để gần mốc SP làm phân tán thời gian khỏi mục tiêu chính. | **Ưu điểm (+):** Cả 3 PBI đều phục vụ sự chủ động trước và trong lúc chờ xe; tránh PBI GPS chưa rõ và không đưa giao diện Tết vào phạm vi ban đầu. |
| Dễ giải thích với Product Owner | **Ưu điểm (+):** Công thức trung bình đơn giản, danh sách PBI và tổng 15 SP dễ kiểm tra; cần nói rõ 17 SP không phải mức bắt buộc. | **Ưu điểm (+):** Giải thích bằng kết quả khách hàng, danh sách PBI cụ thể và điều kiện nhân sự; Đức dễ thấy lý do chọn 13 SP và hoãn PBI GPS. |

## Phần 3 – Lựa chọn và phương án mang vào Sprint Planning

### 1. Lựa chọn

**Chọn cách B, với dự báo ban đầu 13 SP.** Phương án có căn cứ từ cả ba yếu tố: lịch sử Velocity (13–20 SP, hai Sprint gần nhất 15 và 13 SP), Capacity sắp tới giảm còn 186 giờ và mức độ rõ của các PBI. Phạm vi tập trung vào kết quả khách hàng thay vì cố đạt trung bình 17 SP hoặc chỉ tiêu 20 SP.

### 2. Sprint Goal đề xuất

> **Khách hàng có thể chủ động lên lịch chuyến đi và phối hợp đón xe nhờ nhận thông báo tài xế sắp đến và trao đổi trực tiếp với tài xế.**

Danh sách PBI đề xuất cho Sprint Backlog:

1. **Hẹn giờ đặt xe trước – 5 SP.**
2. **Gửi SMS khi tài xế sắp đến – 3 SP.**
3. **Chat với tài xế – 5 SP.**

**Tổng dự báo: 13 SP.** Trong Planning, Developers và Đức thống nhất Sprint Goal, làm rõ các chi tiết còn cần thiết và Developers kiểm tra kế hoạch để đạt Definition of Done. Nếu không đủ khả năng hoàn thành cả ba PBI, ưu tiên thương lượng giảm phạm vi, chẳng hạn hoãn Chat, đồng thời điều chỉnh câu chữ Sprint Goal cho đúng kết quả khả thi trước khi chốt.

### 3. Phản hồi đề nghị nhận 20 SP của quản lý

“20 SP có nằm trong khoảng Velocity cũ của đội, nhưng đó là kết quả quá khứ, không chứng minh Sprint 6 đủ khả năng nhận mức này khi Capacity giảm và đội thay thành viên. Velocity chỉ tính PBI Done và không nên trở thành KPI hay chỉ tiêu phải tăng; đội đề xuất dự báo ban đầu 13 SP để tập trung vào Sprint Goal, sau đó kiểm tra tính khả thi trong Planning. Chúng ta nên theo dõi khả năng đạt Sprint Goal và giá trị khách hàng nhận được thay vì ép số SP tăng trở lại.”
