---
{"dg-publish":true,"permalink":"/ai-agent-system/muc-tieu-va-quy-tac/thiet-lap-quy-tac/","dg-note-properties":{}}
---


Cần xác định rõ các quy tắc nghiệp vụ nhằm thiết lập các logic như
- Thời gian trả hàng < 30 ngày, hàng trong tình trạng tốt
- Chính sách hoàn trả
	- Giá trị đơn hàng < 50$ được tự động hoàn tiền; 
	- >= 50$ cần quản lý duyệt.
- Chính sách đổi hàng
	- Hàng trong tình trạng tốt
	- Trong cùng danh mục loại hàng
- Route to Human: Khách hàng yêu cầu hoặc phát hiện cảm xúc tiêu cực 