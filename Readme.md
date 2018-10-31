This project is about how to use github.

Ghi chú: <id> ở đây tượng trưng cho id hiện ra khi nhấn git log
		 <tên file> là tên của file muốn thực hiện cùng với câu lệnh
		 Cái text editor trong Git tương tự như Vim bên Linux

- Lecture1: // git init -> Khởi tạo 1 folder thành 1 folder chứa git
			// git status -> Kiểm tra trạng thái của folder chứa git
			// git add <ten_file> -> Thêm file có tên là "ten_file" vào staging area
			// git commit m "message" -> Commit hết các file đã thêm vào staging area (đưa vào responsitory)

- Lecture2: // git log -> Xem các lần đã commit, nội dung gồm có 1 chuỗi để tách chuỗi đó ra show log, nội dung commit (message).
			// git show <id> -> ID là chuỗi mà đã đưa ra sau khi chạy git log
			// git diff -> Xem sự khác nhau nếu có 1 hoặc nhiều file mới modified, xem xong thoát ra nhất esc xong rồi nhấn q(quit) (như bên vim trong linux)

- Lecture3: // Working directory -> Thư mục hiện hành đang hoạt động với git. Mặc định mới vào sẽ ở đây nè.
			// Staging Area -> Sau khi add 1 item thì item đó sẽ vô chỗ này.
			// Responsitory -> Sau khi commit thì item nó sẽ ở đây.

- Lecture4: // git checkout -- <ten_file> -> Xóa modified của file đó.
			// git reset ten_file -> Đưa file hiện tại đang trong Staging Area về lại file cũ của nó.

- Lecture5: // git branch -> Xem hiện tại Respository có bao nhiêu nhánh (branch)
			// git checkout -b <tên branch> -> Tạo nhánh mới cho Respository nếu <tên nhánh> là đường dẫn thư mục thì tự tạo thư mục. VD: Feature/ahihi
			// git checkout <tên branch> -> Chuyển qua nhánh <tên nhánh>, nếu chưa có nhánh đó thì báo lỗi.
			// git branch -d <tên branch> -> Xóa nhánh có tên là <tên nhánh> ở trong respository.
			// git merge <tên brank> -> Merge nhánh hiện tại với <tên nhánh>. VD: git checkout master
																				  git merge Feature/dog
																				  git branch -d Feature/dog
																				  -> Nghĩa là merge master với dog trong file Feature, sau đó xóa file Feature đó.

- Lecture6: // git reset --soft <id> -> <id> ở đây là các id lấy từ git log, câu lệnh loại tất cả các commit ở trên nó, đưa hết lại về staging area
			// git reset --mixed <id> -> ..................................., câu lệnh đưa hết tất cả các commit ở trên nó về working directory
			// git reset --hard <id> -> ..................................., xóa hết các commit ở trên nó (nguy hiểm vcl)

- Lecture7: // git revert <id> -> Xóa hết thay đổi của commit đó so với commit trước đó. Lợi hơn bên git reset.

- Lecture8: // 