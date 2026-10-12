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
  - `git rm --cached <file>`: Xoá file ở stage, untrack file, giữ ở directory.
  - `git rm <file>`: Xoá file ở stage và directory.
  - `git rm -r <folder>`: Xoá folder và tất cả những thứ nằm trong nó.
- `git commit -m`: Commit.
- `git log`: View commit log (Có thể thêm thuộc tính --oneline)
- `git push`: Push lên Remote Repo.
- `git restore`
  - `git restore --stage <file>`: Chỉ xoá file khỏi stage.
  - `git restore <file>`: Khôi phục file ở HEAD.

## 2. Xung đột Merge

- `git merge <file cần merge vào>` sau đó vào branch muốn giữ lại data, xoá những dòng noti sau đó merge lại.

## 3. File .gitignore

List những file không track, không được đưa vào git.

### Ví dụ

``` python

# Ignore file chứa biến môi trường, có thể có thông tin bí mật
.env

# Ignore thư mục môi trường ảo
venv/
.venv/

# Ignore thư mục cache của Python
__pycache__/

# Ignore tất cả file có đuôi .log
*.log

# Ignore file .tmp ở bất kỳ thư mục nào
*.tmp

# Ignore một file cụ thể
secret.txt

# Ignore thư mục build ở bất kỳ cấp nào
build/

# Ignore mọi file .csv
*.csv

# Ngoại lệ: không ignore file này
!important.csv

```
