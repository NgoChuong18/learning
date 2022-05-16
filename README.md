# Tìm hiểu Git

- Hệ thống lưu trữ, quản lý tài liệu, source code dùng chung cho những người tham gia cùng dự án. Lưu trữ toàn bộ lịch sử, tác vụ đã thực hiện.
- **Repostory**: kho lưu trữ code. Gồm 2 loại:
	- local repository: khởi tạo ở máy
	- server repository: khởi tạo trên server
# Các lệnh
## git init 
- Khởi tạo 1 git repos ở thư mục gốc.
- Cách dùng: git init

## git add

- Thêm thay đổi vào stage trong thư mục làm việc.
- Cách dùng: git add file_name, git add .

## git commit

- Thông báo để Git lưu lại các sự thay đổi vào repo.
- Cách dùng: git commit -m "message"

## git branch
- Chia nhỏ thành các nhánh đề giải quyết từng chức năng hoạt động riêng lẻ.
- Cách dùng: 
	- tạo mới branch git branch <branchname>
	- chuyển đổi làm việc giữa các branch. git checkout <branchname>
	- Xóa local branch. git branch -d <branchname>(khi fully merged) || git branch -D <branchname>(khi not fully merged)

## git push
- Đưa các commit từ  local lên server.
- Cách dùng: git push --
	-  `-u`  đẩy và tạo một upstream (luồng upload tương ứng với nhánh của local), hay sử dụng cho lần đầu đẩy lên server.
	-   `--all`  đẩy tất cả các nhánh lên server
	-   `--tags`  đẩy tất cả các tag lên server
	-   `--delete`  xóa một nhánh chỉ ra trên server
	-   `--origin beta` đẩy nhánh beta lên repo origin
## git pull
- Tự động lấy toàn bộ dữ liệu từ branch trên repo gộp vào branch đang làm// thay đổi ngay
- Cách dùng: git pull branchname

## git fetch
- Tải về dữ liệu từ repo về branch đang làm// không thay đổi ngay mà chỉ theo dõi.
- Cách dùng: git fetch branchname

## git merge
- Sử dụng để gộp các nhánh vào nhau.// lấy toàn bộ commit 2 branch
- Cách dùng: git merge 

## git rebase
- Sử dụng để gộp các nhánh vào nhau.// gộp commit 2 branch rebase
- Cách dùng: git rebase
- 
## git clone
- Copy 1 repo từ server về máy local
- Cách dùng: git clone

## git reset
- Dùng để hủy commit khi chưa thực hiện push, hủy git add, hủy đưa file vào staging
- Cách dùng: git reset --