# Hướng dẫn sử dụng git
## Thiết lập ban đầu
`$ git config --global user.name "<Tên người dùng>"`

`$ git config --global user.email "<Địa chỉ mail>"`

> Lưu ý: --global là thiết lập cho toàn hệ thống. Bỏ đi nếu bạn chỉ cần thiết lập riêng cho file của mình

* **Thiết lập trình soạn thảo**
 
`$ git config --global core.editor <ten phan mem soan thao>`

* **Thiết lập phần mềm so sánh sự thay đổi**

`$ git config --global merge.tool vimdiff`

* **In màu cho phần xuất ra của git**
 
`$ git config --global color.ui auto`

## Kiểm tra cấu hình và trợ giúp 
`$ git config --list`

`$ git config {key}`

`$ git help <verb>`

`$ git <verb> --help`

`$ man git-<verb>`

## Tạo một kho chứa git
* **Khởi tạo kho chứa**

`$ git init`

* **Sao chép từ một kho chứa**

`$ git clone [url]`

## Kiểm tra trạng thái tập tin
`$ git status`

## Theo dõi các tập tin mới từ lần commit trước
`$ git add <ten file>`

`$ git add .`

## Commit thay đổi 
`$ git commit -m ""`
 
* Them -a vào commit sẽ bỏ qua bước `git add` 

## Kiem tra lich su thay doi
$ git log

## Bo qua tap tin theo doi bang lenh
$ git rm --cached <ten file>

##  Bỏ qua tập tin theo dõi bằng file .gitignore

> **Cách viết file .gitignore:**

- Dòng trống hoặc có dấuu "#" sẽ được bỏ qua.
- Mẫu có kết thúc bằng "/" để chỉ định một thư mục
- Không theo dõi tập tin bằng "*" ở đầu câu.
- Phủ định lênh bằng cách thêm "!" vào trước

**Ví dụ :**

`# a comment` - dòng này được bỏ qua

`*.a` - không theo dõi tập tin có đuôi .a `

`!lib.a` - theo dõi tập lib.a, mặc dù bạn đang bỏ qua tất cả tập tin .a ở trên

`/TODO` - chỉ bỏ qua tập TODO ở thư mục gốc, chứ không phải ở các thư mục con subdir/TODO

`build/` - bỏ qua tất cả các file trong thư mục biuld

`doc/server/arch.txt`       
`doc/*.txt` - bỏ qua doc/notes.txt, không phải 
# bỏ qua tất cả tập .txt trong thư mục doc/
doc/**/*.txt

## Kiểm tra chi tiết thay đổi
`$ git diff`

`$ git diff --cached`

##Xóa tập tin và bỏ theo dõi
`$ git rm <ten file>`

##Di chuyển file,đổi tên file mà không phải dùng lại lệnh `git add`##

`$ git mv file_from file_to`


# Xem lịch sử commit
`$ git log`

`-p` : hien thi noi dung thay doi

`--word-diff` : xem thay doi mot cach tong quat

`--stat` : xem thay doi mot cach tom tat

`$ git log --pretty=oneline`

> Ngoài `oneline` con co `short`,`full` và `fuller`

`$ git log --pretty=format:"%h - %an, %ar : %s"`

 
## In lich su thay doi 
`$ git log --since=2.weeks`

 

