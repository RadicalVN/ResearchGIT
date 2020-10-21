# test

Test đồng bộ dữ liệu từ serverDev (trên server repository) về serverDev (trong local repository)
B1: Check lần 1:
   - Mở file README.md trên branch serverDev (của server repository) -> chỉnh sửa nội dung file -> Điền tiêu đề + mô tả rõ sự chỉnh sửa -> commit changes.
   - Tạo remote (kết nối) giữa local repository và server repository: Mở Git Gui -> chọn remote -> chọn add ... -> điền name (tên remote - có thể có nhiều remote)
     và location (link server repository trên github - đuôi *.git)
   - Đồng bộ dữ liệu (merge): chọn merge -> chọn local merger ... (ctr + M) -> chọn tracking branch -> chọn origin/serverDev -> chọn merge
   - Kiểm tra kết quả: Vào folder (local repository) tìm file README.md để kiểm tra xem dữ liệu đã được đồng bộ chưa.
     KQ: dữ liệu từ branch serverDev (trên server repository) được đồng bộ về serverDev (trong local repository).
B2: Check lần 2: Lặp lại B1.
    KQ: dữ liệu từ branch serverDev (trên server repository) được đồng bộ về serverDev (trong local repository).
B3: Check lần 3: lặp lại B2.
    KQ: dữ liệu từ branch serverDev (trên server repository) được đồng bộ về serverDev (trong local repository).


Test đồng bộ dữ liệu từ local lên server.
B1: Check lần 4:
   - Mở file README.md trong folder (của local repository) -> chỉnh sửa nội dung file -> lưu lại.
   - Tạo remote (kết nối) giữa local repository và server repository: Mở Git Gui -> chọn remote -> chọn add ... -> điền name (tên remote - có thể có nhiều remote)
     và location (link server repository trên github - đuôi *.git)
   - Đồng bộ dữ liệu (push): chọn rescan (load sự thay đổi dữ liệu trong local repository) -> chọn stage changed
     -> commit (điền vào mô tả cho sự thay đổi dữ liệu này) -> chọn commit (tạo cam kết - thỏa thuận sự thay đổi)
     Sau khi commit ta sẽ có được 1 point trong lịch sử thay đổi của dữ liệu.
     -> chọn remote -> chọn push.
   - Kiểm tra kết quả: Vào branch serverDev (server repository) tìm mở file README.md để kiểm tra xem dữ liệu đã được đồng bộ lên chưa.
     KQ: dữ liệu từ branch serverDev (local repository) được đồng bộ lên serverDev (server repository).
B2: Check lần 5: Lặp lại B1.
    KQ: dữ liệu từ branch serverDev (local repository) được đồng bộ lên serverDev (server repository).
B3: Check lần 6: Lặp lại B1.
    KQ: dữ liệu từ branch serverDev (local repository) được đồng bộ lên serverDev (server repository).