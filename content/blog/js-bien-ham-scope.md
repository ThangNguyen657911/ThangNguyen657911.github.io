---
title: "Biến, hàm và scope trong JavaScript"
date: 2025-01-05
category: "JavaScript"
description: "Hiểu rõ cách khai báo và phạm vi biến"
---

1. Biến (Variables): Những chiếc hộp đựng dữ liệu
Trong JS hiện đại (ES6+), chúng ta có 3 cách để khai báo "chiếc hộp" của mình:

let: Dùng cho những giá trị có thể thay đổi (ví dụ: điểm số, tuổi tác).

const: Dùng cho những giá trị hằng số, không được phép gán lại (ví dụ: số Pi, ngày sinh). Mẹo từ blogger: Hãy luôn dùng const mặc định, chỉ đổi sang let khi bạn chắc chắn giá trị đó cần thay đổi.

var: "Cựu binh" từ thời cũ. Hiện nay rất ít dùng vì nó có nhiều cơ chế gây lỗi khó chịu (như hoisting).

2. Hàm (Functions): Cỗ máy thực thi công việc
Hàm là một đoạn mã được đóng gói để tái sử dụng nhiều lần. Thay vì viết đi viết lại 10 dòng code, bạn chỉ cần gọi tên hàm.

Có 2 cách khai báo phổ biến:
Function Declaration (Truyền thống):

function chaoHoi(ten) {

    return `Xin chào, ${ten}!`;

}


Arrow Function (Hiện đại & Gọn nhẹ):

const chaoHoi = (ten) => `Xin chào, ${ten}!`;

3. Scope (Phạm vi): "Vùng phủ sóng" của biến
Đây là phần khiến nhiều "newbie" đau đầu nhất. Scope quyết định nơi nào bạn có thể truy cập vào một biến.

🌎 Global Scope (Phạm vi toàn cầu)
Biến khai báo ngoài cùng của file. Mọi hàm, mọi dòng code đều nhìn thấy và dùng được nó.

Nguy hiểm: Nếu ai cũng có thể sửa, biến toàn cầu dễ bị "hỏng" lúc nào không hay.

🏠 Local / Function Scope (Phạm vi hàm)
Biến khai báo bên trong một hàm thì chỉ hàm đó mới dùng được. Ra ngoài cửa hàm là biến đó "biến mất".

📦 Block Scope (Phạm vi khối)
Áp dụng cho let và const. Biến nằm trong cặp ngoặc nhọn {...} (như của if hoặc for) thì chỉ sống trong đó thôi.