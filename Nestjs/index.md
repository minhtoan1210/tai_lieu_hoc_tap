Lệnh khởi tạo dự án Nest nest new tên dự án
nếu như bị lỗi thì phải cài thêm một thư viện npm i -g @nestjs/cli để có thể khởi tạp được một số lệnh trong nest

Nest nó sẽ có cấu trúc rõ ràng hơn đó là mô hình MVC 

Model: Chứa dữ liệu và logic liên quan đến dữ liệu.
View: Trình bày dữ liệu cho người dùng.
Controller: Xử lý các tương tác của người dùng, cập nhật model và chọn view phù hợp.

Lệnh khởi tạo mới module: nest g module [tên thư mục]
Lệnh khởi tạo mới service: nest g service [tên thư mục]

constructor:  Nó được gọi tự động khi một đối tượng mới của class được tạo ra. 
super:  được sử dụng để tham chiếu đến đối tượng cha 

Trong một dự án thì chúng ta sẽ có rất nhiều app module nên để muốn xài được thì phải import tất cả về app module chính

sao khi demo xong thì tới phần sẽ kết nối với data thông qua docker 

chúng ta sẽ phải tạo 1 docker-compose.yaml  

sao khi set up xong thì ta sẽ chạy docker compose up -d 

sau đó t tiếp tục xài prisma giúp t trong quá trình tạo ra data mà không cần phải login vào tạo 
ta sẽ tạo ra npx prisma init 

sau khi set up xong ta có thể coi một số lệnh của prisma npx prisma --help

sau khi xong ta sẽ tạo ra 1 module có nhiệm vu cho toàn app dùng để kết nối xuống db nó sẽ gọi là một gờ lô bồ module

à nhớ muốn cho các module khác xài thì phải export ra ngoài để các module khác import vào và nhớ thêm thuộc tính @Global() dùng để áp dụng cho toàn bộ app

ta có thể kiểm tra đầu vào bằng class-validator và class-transformer