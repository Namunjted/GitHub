# Huong dan git 

-------------------------------------------------------
## Thiet lap ban dau 
$ git config --global user.name "<Tên người dùng>"
$ git config --global user.email "<Địa chỉ mail>"

## Note:  --global la thiet lap dung cho toan he thong. bo di neu ban chi can thiet lap rieng cho file cua minh 

## Thiet lap trinh soan thao 
$ git config --global core.editor <ten phan mem soan thao>

## Phan mem so sanh su thay doi 
$ git config --global merge.tool vimdiff

## In mau cho phan xuat ra cua git 
$ git config --global color.ui auto

## Kiem tra cau hinh 
$ git config --list
$ git config {key}

## Tro giup
$ git help <verb>
$ git <verb> --help
$ man git-<verb>

------------------------------------------------------
## Khoi tao kho chua thu muc  git
$ git init

## Sao chep kho chua thu muc git
$ git clone [url]
----------------------------------------------------
## Kiem tra trang thai tap tin
$ git status

## Theo doi cac tap tin moi sau lan commit truoc
$ git add <ten file>
$ git add .

## Commit thay doi 
$ git commit -m ""
 
-Them -a vao commit se bo qua buoc git add 

## Kiem tra lich su thay doi
$ git log
-----------------------------------------------------
## Bo qua tap tin theo doi bang lenh
$ git rm --cached <ten file>
##  Bo qua tap tin dung .gitignore
Note : cach viet file .gitignore

- Dong trong hoac co dau "#" se duoc bo qua
- Mau co ket thuc bang "/" de chi dinh mot thu muc
- Khong theo doi cac tap tin co duoi "*"
- Phu dinh lenh bang cach them dau "!" vao truoc
--------------------------------
## Vi Du
[**Smart metering**](https://git-scm.com/book/vi/v1/C%C6%A1-B%E1%BA%A3n-V%E1%BB%81-Git-Xem-L%E1%BB%8Bch-S%E1%BB%AD-Commit)

# a comment - dòng này được bo qua
# không theo dõi tập tin có đuôi .a 
*.a
# nhưng theo dõi tập lib.a, mặc dù bạn đang bỏ qua tất cả tập tin .a ở trên
!lib.a
# chỉ bỏ qua tập TODO ở thư mục gốc, chứ không phải ở các thư mục con subdir/TODO
/TODO
# bỏ qua tất cả tập tin trong thư mục build/
build/
# bỏ qua doc/notes.txt, không phải doc/server/arch.txt
doc/*.txt
# bỏ qua tất cả tập .txt trong thư mục doc/
doc/**/*.txt

------------------------------
# Kiem tra chi tiet thay doi
$ git diff
$ git diff --cached
-----------------------------------------------
# Xoa tap tin
$ git rm <ten file>

# Di chuyen file ,noi dung file ma khong can phai dung git add lai
$ git mv file_from file_to

------------------------------------------------
# Xem lich su commit
$ git log

-p : hien thi noi dung thay doi
--word-diff : xem thay doi mot cach tong quat
--stat : xem thay doi mot cach tom tat

$ git log --pretty=oneline

Ngoai "oneline" con co short, full, và fuller

$ git log --pretty=format:"%h - %an, %ar : %s"

%H	Mã băm của commit
%h	Mã băm của commit ngắn gọn hơn
%T	Băm hiển thị dạng cây
%t	Băm hiển thị dạng cây ngắn gọn hơn
%P	Các mã băm gốc
%p	Mã băm gốc ngắn gọn
%an	Tên tác giả
%ae	E-mail tác giả
%ad	Ngày "tác giả" (định dạng tương tự như lựa chọn --date= )
%ar	Ngày tác giả, tương đối
%cn	Tên người commit
%ce	Email người commit
%cd	Ngày commit
%cr	Ngày commit, tương đối
%s	Chủ để
------------------------------------------------------
-p	        Hiển thị bản vá với mỗi commit.
--word-diff	Hiển thị bản vá ở định dạng tổng quan (word).
--stat	        Hiển thị thống kê của các tập tin được chỉnh sửa trong mỗi commit.
--shortstat	Chỉ hiển thị thay đổi/thêm mới/xoá bằng lệnh --stat.
--name-only	Hiển thị danh sách các tập tin đã thay đổi sau thông tin của commit.
--name-status	Hiển thị các tập tin bị ảnh hưởng với các thông tin như thêm mới/sửa/xoá.
--abbrev-commit	Chỉ hiện thị một số ký tự đầu của mã băm SHA-1 thay vì tất cả 40.
--relative-date	Hiển thị ngày ở định dạng tương đối (ví dụ, "2 weeks ago") thay vì định dạng đầy đủ.
--graph	        Hiển thị biểu đồ ASCII của nhánh và lịch sử tích hợp cùng với thông tin đầu ra khác.
--pretty	Hiện thị các commit sử dụng một định dạng khác. Các lựa chọn bao gồm oneline, short, full, fuller và format (cho phép bạn sử dụng định dạng riêng).
--oneline	Một lựa chọn ngắn, thuận tiện cho --pretty=oneline --abbrev-commit.
 
# In lich su thay doi 
$ git log --since=2.weeks

-(n)	Chỉ hiển thị n commit mới nhất
--since, --after	Giới hạn các commit được thực hiện sau ngày nhất định.
--until, --before	Giới hạn các commit được thực hiện trước ngày nhất định.
--author	Chỉ hiện thị các commit mà tên tác giả thoả mãn điều kiện nhất định.
--committer	Chỉ hiện thị các commit mà tên người commit thoả mãn điều kiện nhất định.
----------------------------------------------------------------------------
# Phuc hoi 

