Lệnh Ubuntu 
+ Vi: trình chỉnh sửa code như vs
     lệnh chạy : 
     + :q : thoát vi
     + vi tenfile.html  : vào chế độ no mode 
     + không lưu file thoát vi : :!
     + lệnh lưu : w
     + lưu và thoát : :x
+ cat :
     + In ra nội dung HTMl
     + cú pháp gộp hai file : cat file1. file2. > tên file mới 
+ echo :
     + In ra nội  dung không cần file 
     + tạo file có nội dung trên lệnh :  echo "<h1>hello<h1>" > echo.html (in nhiều nội dung >> )
+ tail :
    +  tail -f tên file : follow theo file những dòng cuối  
+ grep : 
     + tìm : cat tên file | grep dòng cần tìm  
+ cp : 
     + copy file cũ vòa file mới : cp tênfilecũ tênfilemới
     + copy tất cả file folder : cp -r filecũ filemới
+ mv : (di chuyển , đôỉ tên )
     + đổi tên file : mv filecũ file mới 
     + di chuyển dữ nguyên file : mv file folder/ (đổi tên file : mv file folder/newfile)
     + di chuyển folder với nhau : mv folder1 folder/
+ rm :
     + xóa file 1 hoặc nhiều file : rm namefile  ( không xóa được thư mục )
     + xóa file bên trong thư mục : rm -r namefile
+ rmdir :
     + xóa thư mục trống không xóa đc file bên trong : rmdir namefile
+ sudo: (Lệnh to nhất)

+ chmod : 
     + u=rmx : phân quyền nhóm user  |  ( "+" thêm 1 quyền "- ": Giữ nguyên loại bỏ quyền đó , "=" :giữ nguyên)
     + g=rx : phân quyền nhóm group  | 
     + o=r : phân quyền nhóm other   |

     ví dụ : ( chmod / index.js)
     + lệnh bỏ quyền viết : sudo chmod o-w index.js
          result: -rwxrwxr-x 1 duong duong 0 time index.js
+ chown : (Thay đổi chủ sở hữu)
     + sudo chown  root run.sh : xét quyền root cho file 
          result: -rwxr--r-- 1 root  duong time run.sh
     + sudo chown root:root run.h : Chỉ xét riêng quyền root ( tương tự khi bỏ quyền root : name:names)
          result : -rwxr--r-- 1 root  root  time run.sh
+ man : tra cứu lệnh thường dùng 
+ wget : (tải bằng commad)
     + wget linktải 
+ apt : ( quản lí thư viện )
     + sudo apt install thư viện
+ kill :
     + Ngừng tiến trình khi bị treo
          ví dụ : 
          pid
          953  0.0  0.0   3156  1056 pts/2    S+   time tail -f random.js
          + kill 953 : kết quả cửa sổ ngừng chạy (Terminated)
          + kill -9 953 : Kết quả thoát hẳn (Killed)
+ ping : (Tốc dộ kết nối của máy chủ)
     + kiểm tra ping : ping tên link    
+ passwd : (Đổi mật khẩu Ubuntu)
+ top : (tương tự task manager     )
     + Lệnh chạy : htop,tops
     + khi tiến trình ăn cpu sẽ dùng top
+ df : ( báo cáo dung lượng    đã dùng )
+ free : 
     ví dụ :
          Total:Bộ nhớ hệ thống tổng cộng.
          Used: Bộ nhớ đang sử dụng bởi các ứng dụng.
          Available:Ước tính bộ nhớ cho ứng dụng mới (không swap).
          Free:Bộ nhớ sẵn có cho các ứng dụng mới.
