# Những kiến thức cơ bản về Web Development

## 1. Internet là gì? LAN là gì? WAN là gì?

## 2. Website là gì?

## 3. Kiến trúc website như thế nào?

## 4. Cách thức web ngày nay hoạt động ra sao?

## 5. Web Server là gì?

## 6. Web Browser là gì?

## 7. HTTP Protocol là gì?

## 7. DNS là gì?

## 8. Địa chỉ IP là gì?

## 9. Domain là gì?

## 10. Mô hình Client - Server hoạt động ra sao?

## 11. Cookie, Session, Cache là gì?

## 12. HTTP, HTTPs là gì?

## 13. Chuyện gì xảy ra khi nhập vào một domain trên browser và nhấn enter?

- Sau khi enter, điều đầu tiên browser sẽ truy cập vào các bản ghi DNS (Domain Name Server) để tìm kiếm địa chỉ IP tương ứng với server host domain đó. Để có thể tìm kiếm được địa chỉ IP tương ứng, browser sẽ kiểm tra các bản ghi trong các cache theo thứ tự bao gồm: browser cache, OS cache, router cache và ISP cache. Nếu không tìm thấy địa chỉ IP nào tương ứng với domain thì DNS server của ISP sẽ thiết lập truy vấn DNS trên các máy chủ DNS trên internet để tìm kiếm địa chỉ IP chính xác.
- Sau khi browser nhận được thông tin về địa chỉ IP chính xác tương tứng với domain, nó sẽ thiết lập một kết nối với server tương ứng với giao thức TCP và được thực hiện thông qua quá trình bắt tay ba bước. Tại quá trình này client và server sẽ trao đổi thông điệp SYN (synchronize) và ACK (acknowledge):
  - Client gửi một SYN package đến server, yêu cầu mở một kết nối mới.
  - Nếu server đã mở port và có thể chấp nhận kết nối, nó sẽ trả về SYN/ACK packet tương ứng với SYN packet của client.
  - Client nhận SYN/ACK packet và công nhận nó bằng cách gửi một ACK packet đến server.
- Khi kết nối TCP được thiết lập, lúc này browser sẽ gửi request đến server.
- Server sẽ nhận được request, lúc này server sẽ xử lý request đó và trả vể response cho client. Trong response lúc này sẽ các file static như html, css hay js nếu như client yêu cầu truy cập vô một trang web; hoặc sẽ trả về data nếu như client yêu cầu lấy data.
- Nếu như client yêu cầu vô một trang web và sau khi nhận được response là một file html, thì client sẽ hiển thị nội dung HTML theo từng giai đoạn. Đầu tiên, clienet sẽ hiển thị cấu trúc tổng quan HTML, sau đó client sẽ gửi GET request lên server để yêu cầu bổ sung các file thành phần bổ sung kèm theo khác như các file css, js, ảnh,... Những file này sẽ được browser cache lại, do đó ở những lần truy cập sau thì những file này sẽ không cần phải request nữa.

Tham khảo: [What happens when you type a URL in the browser and press enter?](https://medium.com/@maneesa/what-happens-when-you-type-an-url-in-the-browser-and-press-enter-bb0aa2449c1a)

## 14. Mô hình OSI là gì?

## 15. Mô hình TCP/IP là gì?

## 15. Static website là gì? Dynamic Website là gì?

## 16. Server Side Rendering là gì? Client Side Rendering là gì?

### 1. Server Side Rendering

### 2. Client Side Rendering

## 17. Front-end là gì? Back-end là gì?
