---
{"dg-publish":true,"permalink":"/ai-agent-system/quy-trinh-hoat-dong/","tags":["excalidraw"],"dg-note-properties":{"excalidraw-plugin":"parsed","tags":["excalidraw"]}}
---

==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠== You can decompress Drawing data with the command palette: 'Decompress current Excalidraw file'. For more info check in plugin settings under 'Saving'


# Excalidraw Data

## Text Elements
    User Channel
    - Web Chat
    - Email
    - Discord
{ #QAXBlnWE}


Gateway
- Auth/SSO,PII, Rate limit,Dedupe
{ #m7n4id8D}


Relational DB
{ #jd2lngwg}


Auth
{ #PD62H3XA}


User Auth, 
Fetch Chat/Email
{ #PnKyrdBn}


Ask a question:
I want to refund my Macbook Pro
{ #SWgIbzaC}


Q&A Agent
- speak to user all the time
{ #YwPhcM4e}


Respond to the user real-time
{ #NSBMxORL}


Router Agent
- understand user intent
- decides agent routing
{ #iLSH63NY}


Human
{ #gsDytk0i}


Detect critical emotion
{ #5jO66xcm}


Planner Agent
- decides functional calling

Or, a deterministic workflow
{ #bE2hlc5i}


Decide to take the
Return Route Action
{ #7BPifCgC}


Bước 1: Tiếp nhận và Xác thực (Gateway)
Khách hàng nhắn tin qua Web Chat hoặc Email.

API Gateway kiểm tra danh tính (SSO), bảo mật thông tin cá nhân (PII) và giới hạn tần suất gửi tin (Rate limit) để tránh spam.

Bước 2: Phân loại ý định (Router Agent)
Router Agent đóng vai trò "lễ tân". Nó phân tích câu hỏi của khách (ví dụ: "Tôi muốn trả cái áo này") để quyết định chuyển tiếp cho Agent chuyên trách nào.

Human-in-the-loop: Nếu Router nhận thấy khách hàng đang cực kỳ giận dữ (qua phân tích cảm xúc), nó sẽ ngắt AI và chuyển thẳng cho nhân viên hỗ trợ là người thật.

Bước 3: Giao tiếp thời gian thực (Q&A Agent)
Để đạt mục tiêu phản hồi < 1 giây, Q&A Agent sẽ trả lời ngay lập tức các câu xã giao hoặc thông báo "Đợi tôi một chút để kiểm tra". Nó đóng vai trò là "CEO" điều phối luồng hội thoại chính.

Bước 4: Lập kế hoạch và Thực thi (Planner Agent & Function Calling)
Đây là phần quan trọng nhất. Nếu khách muốn trả hàng, Return Planner Agent sẽ được kích hoạt:

Kiểm tra chính sách: Agent truy cập Vector DB để xem mặt hàng này có được trả không.

Function Calling (Gọi hàm): AI tự động gọi các công cụ (Tools) bên thứ ba:

Shopify API: Để kiểm tra trạng thái đơn hàng hiện tại.

Stripe API: Để thực hiện lệnh hoàn tiền tự động.

Logistics API (3PL): Để tạo nhãn vận chuyển cho khách gửi hàng lại.

Bước 5: Cập nhật và Phản hồi
Sau khi các API thực thi xong, Planner Agent báo cáo kết quả cho Q&A Agent.

Q&A Agent tổng hợp lại và trả lời khách hàng: "Xong rồi! Tiền đã được hoàn về thẻ của bạn, hãy kiểm tra email để lấy nhãn trả hàng."
{ #St6AYTIr}


Vector DB
(FAQs, Policies)
{ #X2Su3Xpe}


Check Policy via VectorDB
{ #7Jv8sQOB}


Policy / Guardrails
- Capability Tokens, RBAC, human approvals, read back ( confirmation)
{ #lgaIkUCT}


Align with policy
{ #WZynqixB}


Inform the Agent
{ #UlfNmWdC}


Shopify API
- track orders status, Return Merchandise Auth (RMA), exchanges
{ #cyRSTnk0}


If it fits the policy, call Shopify API for return
{ #liTkzfTq}


Stripe API
- Payment / Refund
{ #u2361Vyp}


Payment / Refund done
{ #7RU9Rflm}


Return the latest status of return back to Q&A Agent to talk to the user
{ #7HdpPnnQ}


CRM
- write / fetch deal pipeline
- creat / update tickets
{ #XV0XXnJv}


    Observalbility, Metric & Evals
{ #3V2MbPO0}


