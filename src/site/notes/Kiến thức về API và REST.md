---
{"dg-publish":true,"permalink":"/kien-thuc-ve-api-va-rest/","tags":["gardenEntry"],"dg-note-properties":{}}
---

1. Đầu tiên, là khái niệm về **API**
	- Viết tắt của Application Programing Interface 
	- API cho phép chúng ta xây dựng chức năng cho phép 1 ứng dụng gửi yêu cầu đến ứng dụng khác ,và ứng dụng kia sẽ trả về thứ gì đó ? Thứ gì đó ở đây là Dữ liệu JSON . 
    - JSON  là JavaScript Object Notation, nó là 1 kí hiệu đối tượng trong JavaScript, có ưu điểm là nhẹ, dễ tryền trên internet, và được hỗ trợ hầu hết trên mọi ngôn ngữ . JSON được lưu trữ dưới dạng key : value (giống dictionary trong python)
	- Một khái niệm nữa liên quan tới API là **Endpoint**, nó trỏ đến một tài nguyên cụ thể trên server. Ta có thể hiểu đơn giản là một đại chỉ URL cụ thể mà ở đó phần mềm hoặc ứng dụng của bạn có thể giao tiếp với API để lấy tài nguyên.
    
2. Về REST 
	- Là viết tắt của REpresentational State Transfer (dịch là: Chuyển giao trạng thái đại diện).
	- Nó là một kiểu kiến trúc đưa ra tập hợp các quy tắc khi thiết kế ứng dụng web và định hướng cách máy tính giao tiếp với nhau qua internet . 
	- Nó gồm 6 constraint :
		1. Client - Serve : Kiến trúc phải phân tách rõ ràng giữa hai bên. Ví dụL Client chỉ lo hiện thị giao diện, còn Server chỉ lo việc lưu trữ dữ liệu và xử lí logic.
		2. Stateless : Đây là tính chất vô cùng quan trọng của REST. Server sẽ không lưu bất kì thông tin gì về client, vì vậy khi gửi request phải gửi lên đầy đủ tất cả thông tin cần thiết. Xong việc server quên luôn tk client.
		3. Cacheable : có thể lưu vào bộ nhớ đệm 
		4. Uniform Interface : cách thức giao tiếp giữa client và server phải tuân thủ theo 1 uniform. Luôn dùng URL để xác định tài nguyên( ENDPOINT) 
		5. Layered System : người dùng không  biết là đang kết nối trực tiếp với máy chủ hay qua các lớp trung gian khác
		6. Code on Demand (optional) : Máy chủ có thể tạm thời chuyển các đoạn mã có thể thực thi được (ví dụ như mã JavaScript) xuống cho Client.
		
3. 	