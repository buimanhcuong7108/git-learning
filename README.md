# Basic Git command line

## 1. CƠ BẢN

- `git init`: Khởi tạo directory đang ở là một Repo.
- `git clone <url>`: Clone về máy.
- `git status`: Hiện status của staging area.
- `git add`
  - `git add -A` hoặc `git add --all`: Thêm tất cả vào stage.
  - `git add .`: Thêm tất cả file/folder con vào stage, kể cả việc xoá file/folder.
  - `git add *`: Thêm tất cả file/folder con vào stage, chỉ thêm những thay đổi có thể nhìn thấy như: Thêm bớt file, modify file,...
- `git reset`:
  - `git reset --hard`: Cho về HEAD của commit trước tất cả các file.
  - `git reset --mixed` (mạc định): Xoá các file ở stage.
- `git rm`:
  - `git rm --cached <file>`: Xoá file ở stage, giữ ở directory.
  - `git rm <file>`: Xoá file ở stage và directory.
  - `git rm -r <folder>`: Xoá folder và tất cả những thứ nằm trong nó.
- `git commit -m`: Commit.
- `git log`: View commit log (Có thể thêm thuộc tính --oneline)
- `git push`: Push lên Remote Repo.
