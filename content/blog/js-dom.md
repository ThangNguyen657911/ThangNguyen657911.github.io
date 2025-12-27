---
title: "DOM và thao tác HTML bằng JavaScript"
date: 2025-01-06
category: "JavaScript"
description: "Thao tác HTML thông qua DOM"
---

🌳 DOM là gì? (Document Object Model)
Hãy tưởng tượng trang HTML của bạn là một cái cây. Mỗi thẻ HTML (<div>, <h1>, <p>) là một "nhánh" hoặc "chiếc lá". Trong lập trình, chúng ta gọi cái cây này là DOM Tree.

Khi trình duyệt tải trang web, nó biến tất cả các thẻ HTML thành các Object (đối tượng) mà JavaScript có thể hiểu và chỉnh sửa được.

🛠 Thao tác HTML bằng JavaScript: 4 Bước "Thần thánh"
Để thay đổi bất cứ thứ gì trên trang web, bạn cần đi theo quy trình: Tìm -> Sửa -> Đổi -> Lắng nghe.

1. Tìm kiếm (Selecting Elements)
Trước khi muốn "phẫu thuật" một phần tử, bạn phải tìm thấy nó đã.

document.getElementById('id'): Tìm nhanh bằng ID (duy nhất).

document.querySelector('.class'): Tìm bằng CSS Selector (cực kỳ linh hoạt và mạnh mẽ).

2. Thay đổi nội dung (Changing Content)
Sau khi đã "tóm" được phần tử, bạn có thể đổi nội dung của nó ngay lập tức:

.innerText: Thay đổi văn bản thuần túy.

.innerHTML: Chèn hẳn một đoạn mã HTML mới vào bên trong.

3. Thay đổi diện mạo (Changing CSS)
JavaScript có thể can thiệp trực tiếp vào style của phần tử:

const box = document.querySelector('.box');

box.style.backgroundColor = 'blue';

box.style.borderRadius = '10px';

4. Lắng nghe sự kiện (Event Listeners)
Đây là lúc ma thuật thực sự xảy ra. Bạn bắt trình duyệt phải "chờ" người dùng làm gì đó rồi mới hành động.

Click: Khi người dùng bấm nút.

Submit: Khi gửi form.

Keydown: Khi nhấn một phím trên bàn phím.


