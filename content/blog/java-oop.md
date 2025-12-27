---
title: "Lập trình hướng đối tượng trong Java"
date: 2025-01-02
category: "Java"
description: "Các khái niệm OOP trong Java"
---

🏛️ 4 Trụ cột của OOP: Những "quyền năng" cốt lõi
Để một ngôn ngữ được coi là hướng đối tượng thực thụ như Java, nó phải tuân thủ 4 nguyên lý vàng:

1. Tính Đóng gói (Encapsulation)
Hãy tưởng tượng một viên thuốc. Bạn biết công dụng của nó, nhưng không cần biết bên trong chứa những bột gì hay hóa chất gì. Trong Java, chúng ta sử dụng các Access Modifiers (private, public, protected) để che giấu dữ liệu bên trong lớp, chỉ cho phép truy cập qua các hàm getter và setter.

Lợi ích: Bảo vệ dữ liệu khỏi việc bị thay đổi tùy tiện từ bên ngoài.

2. Tính Kế thừa (Inheritance)
Bạn không cần phải chế tạo lại bánh xe. Nếu bạn đã có lớp Xe, bạn có thể tạo lớp XeCon kế thừa từ nó. XeCon sẽ có sẵn mọi đặc điểm của Xe (bánh xe, động cơ) và chỉ cần thêm những thứ riêng biệt (số cửa, loại phim cách nhiệt). Trong Java, chúng ta dùng từ khóa extends.

Lợi ích: Tái sử dụng mã nguồn, tiết kiệm thời gian và công sức.

3. Tính Đa hình (Polymorphism)
Cùng một mệnh lệnh "Kêu đi!", nhưng con Chó sẽ "Gâu gâu", còn con Mèo sẽ "Meo meo". Trong Java, đa hình cho phép một đối tượng có thể thực hiện một hành động theo nhiều cách khác nhau (thông qua Overriding và Overloading).

Lợi ích: Giúp chương trình linh hoạt, dễ dàng mở rộng mà không cần sửa đổi cấu trúc cũ.

4. Tính Trừu tượng (Abstraction)
Khi lái xe, bạn chỉ cần biết đạp ga là xe chạy, đạp phanh là xe dừng. Bạn không cần quan tâm piston chuyển động ra sao hay xăng đốt cháy thế nào. Java thực hiện điều này thông qua Abstract Class và Interface.

Lợi ích: Giúp lập trình viên tập trung vào hành động (xe làm được gì) thay vì cách thực hiện (xe làm điều đó như thế nào).
