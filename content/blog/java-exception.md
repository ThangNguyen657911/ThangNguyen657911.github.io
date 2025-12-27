---
title: "Xử lý Exception trong Java"
date: 2025-01-03
category: "Java"
description: "Cách xử lý lỗi khi lập trình Java"
---

1. Exception là gì? (Hierarchy trong Java)
Exception là một sự kiện làm gián đoạn luồng thực thi bình thường của chương trình. Trong Java, tất cả các ngoại lệ đều là đối tượng (Object) và bắt nguồn từ lớp cao nhất là Throwable.

Error: Những lỗi nghiêm trọng hệ thống (như OutOfMemoryError) mà lập trình viên thường không thể xử lý được.

Exception: Những tình huống mà chúng ta có thể dự đoán và xử lý:

Checked Exception: Lỗi xảy ra tại thời điểm Compile-time (ví dụ: IOException). Java bắt buộc bạn phải xử lý nó thì mới cho chạy code.

Unchecked Exception (Runtime): Lỗi xảy ra khi chương trình đang chạy (ví dụ: NullPointerException, ArrayIndexOutOfBoundsException). Thường do lỗi logic của người viết code.

2. "Bộ khung" 5 từ khóa quyền lực
Để xử lý Exception, Java cung cấp cho bạn 5 từ khóa cơ bản: try, catch, finally, throw, và throws.

Try - Catch: Lưới đỡ an toàn
Bạn đặt những dòng code "nguy hiểm" vào trong khối try. Nếu có chuyện gì xảy ra, khối catch sẽ tóm lấy lỗi đó.

Finally: Dọn dẹp chiến trường
Dù có lỗi hay không, khối finally luôn luôn được thực thi. Đây là nơi lý tưởng để đóng kết nối Database hoặc đóng File.

Throw & Throws: "Đùn đẩy" trách nhiệm
throw: Dùng để chủ động tung ra một ngoại lệ (ví dụ: tuổi âm thì không cho đăng ký).

throws: Khai báo ở tên hàm để cảnh báo người dùng hàm này: "Cẩn thận nhé, hàm này có thể gây ra lỗi đấy!".