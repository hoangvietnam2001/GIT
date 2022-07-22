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



