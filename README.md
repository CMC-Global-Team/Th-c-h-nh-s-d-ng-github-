# Thực hành Git & GitHub - Git Cheat Sheet

## Mục tiêu
- Hiểu và làm quen với Git và GitHub.
- Thực hành các thao tác cơ bản: commit, push, pull, branch, merge.
- Quản lý phiên bản code và hợp tác nhóm hiệu quả.

---

## Bảng Cheat Sheet Git

| Nhóm lệnh | Lệnh | Mô tả / Ví dụ |
|-----------|------|----------------|
| **Cấu hình Git** | `git config --global user.name "Tên của bạn"` | Cấu hình tên người dùng |
| | `git config --global user.email "email@domain.com"` | Cấu hình email |
| | `git config --global color.ui auto` | Hiển thị màu trong terminal |
| **Tạo repo** | `git init` | Khởi tạo repo Git mới |
| | `git clone <url>` | Sao chép repo từ GitHub về máy |
| **Kiểm tra trạng thái** | `git status` | Kiểm tra file modified/staged/untracked |
| | `git log` | Xem lịch sử commit |
| | `git log --oneline` | Xem lịch sử commit gọn |
| **Thêm file & commit** | `git add <file>` | Thêm file vào staging |
| | `git add .` | Thêm tất cả file mới/sửa đổi |
| | `git commit -m "Thông điệp"` | Commit các thay đổi |
| | `git commit -am "Thông điệp"` | Thêm & commit file đã tracked |
| **Branch** | `git branch` | Xem danh sách branch |
| | `git branch <tên-branch>` | Tạo branch mới |
| | `git checkout <tên-branch>` | Chuyển sang branch khác |
| | `git checkout -b <tên-branch>` | Tạo + chuyển branch mới |
| | `git merge <tên-branch>` | Gộp branch vào branch hiện tại |
| **Remote** | `git remote -v` | Xem remote |
| | `git remote add origin <url>` | Thêm remote repo |
| | `git push origin main` | Push branch main lên GitHub |
| | `git push origin <branch>` | Push branch khác lên GitHub |
| | `git pull origin main` | Lấy thay đổi từ GitHub |
| **So sánh & kiểm tra** | `git diff` | Xem khác nhau giữa working directory & staging |
| | `git diff --staged` | Xem khác nhau giữa staged & last commit |
| **Xóa & di chuyển file** | `git rm <file>` | Xóa file & staging |
| | `git mv <old> <new>` | Đổi tên/di chuyển file |
| **Hồi phục / Revert** | `git checkout -- <file>` | Hủy thay đổi trong working directory |
| | `git reset HEAD <file>` | Hủy staging file |
| | `git revert <commit>` | Tạo commit đảo ngược commit cũ |
| | `git reset --hard <commit>` | Quay lại commit trước (cẩn thận!) |
| **Tag & Release** | `git tag` | Xem danh sách tag |
| | `git tag <tên-tag>` | Tạo tag mới |
| | `git push origin <tên-tag>` | Push tag lên GitHub |
| **Khác** | `git stash` | Lưu tạm thay đổi chưa commit |
| | `git stash apply` | Lấy lại thay đổi đã stash |
| | `git fetch` | Lấy thay đổi từ remote nhưng không merge |
| | `git rebase <branch>` | Rebase branch (thay đổi lịch sử commit) |

---

## Hướng dẫn nhanh
1. Tạo repo:
```bash
git init
git remote add origin <url>
