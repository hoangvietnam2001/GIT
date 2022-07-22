# Terms

    * Repository (Repo)
        - Thư mục dự án của chúng ta
    * Branch ( cành )
        - 1 dự án có nhiều cành khác nhau (cành mặc định là master)
    * Confilct ( Xung đột )
    * Local
    * Remote
# Commands

# git init : biến dự án thành 1 repo (dự án có thể dùng git)
# git status : thấy được trạng thái của dự án, thấy được những thay đổi
# git add : Chuẩn bị lưu lại thời điểm của dự án ( git add file_name) -  ví dụ đánh git add index.html thì file index sẽ chuẩn bị được lưu còn file note thì chưa 
(git add . : chuẩn bị lưu lại tất cả file)# git reset : set lại trạng thái không chuẩn bị lưu nữa
# git commit -m 'ghi chú' : đánh dấu thời điểm thay đổi dự án
# git log : xem lại thời điểm, chi tiết thay đổi
# git log --oneline : xem commit gọn hơn
# git checkout id_commit : trở lại dự án trước id commit
# git checkout master : trở về hiện tại của dự án
    (git checkout {branch_name}) - cành mặc định là master
# git branch : xem branch hiện tại
# git checkout -b {branch_name} : tạo 1 branch mới
# git merge {branch_name} : Tổng hợp các branch lại với nhau
# git branch -d {branch_name} : Xóa branch

## Kết hợp GIT với GITHUB
> TH1: Đẩy từ local repo đẩy lên remote : Nếu đẩy như thế này thì tên của repo trên GITHUB phải trùng với tên dự án ở local máy tính của bạn
# git push : đẩy local repo lên remote repo
    git push {url_name} {branch_now}
# Cách tạo alias : 
    git remote add {alias_name} {url_name}
   Cách dùng : git push {alias_name} {branch_now}

> TH2 : Kéo dự án từ remote repo trên github về máy tính của chúng ta
# git clone {url_name} : tạo 1 dự án kéo từ trên remote về máy tính của chúng ta tại thư mục đang đứng

## code . : khởi chạy dự án hiện tại lên vs

- Khi thay đổi dự án đã clone về local mà muốn đẩy lại github thì chỉ việc 'git push' thôi chứ không cần 'git push {url_name} {branch_now}' 
## Sẽ có TH tạo ra 1 branch ở local, làm sao đẩy local branch này lên remote repo ?

    1. git checkout -b {branch_name}
    2. git push -s {alias_name} {branch_name}

## Ngược lại muốn kéo 1 branch trên remote repo về local thì làm ntn ?

    1. git fetch {alias_name}
    2. git checkout -b {remote_branch_name}{alias_name}/{remote_branch_name}

## Nếu muốn merge, kết hợp các branch khác với master thì làm ntn ??

# git pull : gộp lại các branch

## Hiện tại git đang theo dõi tất cả các file của chúng ra vậy nếu muốn git không muốn theo dõi 1 file nào đó thì làm sao ? DÙNG git ignore

# git ignore : loại bỏ theo dõi của git với file mong muốn của chúng ta

