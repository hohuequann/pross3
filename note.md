# git là gì?

**keyword:** lưu trữ lịch sử thay đổi, hệ thống quản lý phiên bản, làm việc nhóm.

- Là hệ thống quản lý phiên bản phân tán (DVCS), một trong những hệ thống phổ biến hiện nay, cung cấp repository (repo) để lưu trữ toàn bộ lịch sử thay đổi. 
- hệ thống hỗ trợ nhiều người làm việc cùng một lúc (xây dựng dự án lớn)

**source control:** là khái niệm chung về quản lý code, có thể là google drive, github,... lưu trữ mọi thay đổi, có thể sao lưu và phục hồi khi cần, hỗ trợ nhiều người làm việc cùng lúc

**VCS**
- Version control system là hệ thống quản lý phiên bản, hệ thống sẽ lưu trữ tất cả các file trong toàn bộ dự án và lịch sử thay đổi. Mỗi 1 thay đổi được lưu là 1 ver.
- có thể lưu trữ nhiều ver khác nhau từ remote repo đã được clone về, thay đổi trên local và commit rồi push lên remote repo.
- có thể xem lại lịch sử thay đổi: ngày giờ, người sửa đổi, lý do thay đổi

**các thuật ngữ**
1. **Repository (repo):* kho chứa dự án, tất cả các ver, lịch sử sửa đổi. Gồm local repo và remote repo.
    - local repo: kho lưu trữ trên máy của mình
    - remote repo: kho lưu trữ trên các nền tảng (github, gitlab)

2. **Staging area*: khu vực đợi để được thêm vào nhánh (branch)

3. *branch*: ver độc lập của nhánh master, có thể tùy chỉnh cho đến khi commit và push lên remote

4. *conflict*: xung đột khi chỉnh sửa cùng 1 file trên 2 nhánh, sau đó merge lại sẽ xảy ra conflict. git cần biết mình muốn giữ lại đoạn nào.

5. *HEAD*: con trỏ, dùng để trỏ đến commit cuối cùng và nhánh đang hoạt động  

6. *clone*: sao chép toàn bộ dự án trên server (remote)

7. *pull*: lấy và merge code từ remote về local để đồng bộ code. 

8. *push*: đẩy code từ local lên remote sau khi đã chỉnh sửa các nhánh

9. *fetch*: lấy code từ remote về local. khác với pull, fetch chỉ tải code và ko merge vào nhánh hiện tại

10. *tag*: 

11. *upstream*: là cầu nối giữa remote repo và local repo

# tại sao phải có git? 
vì có nhiều tiện ích hỗ trợ trong việc:
    - theo dõi lịch sử thay đổi, có thể quay về commit cũ
    - hỗ trợ làm việc nhóm: dễ dàng hợp nhất code, git sẽ báo có xung đột (conflict) nếu thấy sự khác biệt.
    - có thể chỉnh sửa mà ko cần internet.
    - dễ dàng khôi phục nếu lỡ xóa file hoặc gặp lỗi.

# git hoạt động ntn?