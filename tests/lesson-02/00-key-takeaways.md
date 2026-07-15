# Lesson 02 - Key Takeaways

## Mục tiêu buổi học

- Hiểu Version Control System (VCS) là gì.
- Nắm được cách sử dụng Git để quản lý source code.
- Ôn tập các kiến thức JavaScript cơ bản để chuẩn bị học Playwright.

---

# 1. Version Control System (VCS)

## VCS là gì?

Version Control System (Hệ thống quản lý phiên bản) là công cụ giúp quản lý lịch sử thay đổi của source code.

### Lợi ích

- Lưu lại lịch sử thay đổi.
- Có thể quay lại phiên bản cũ khi cần.
- Hỗ trợ nhiều người cùng làm việc trên một dự án.
- Dễ dàng theo dõi ai đã thay đổi nội dung nào.
- Hạn chế việc ghi đè source code.

### Một số VCS phổ biến

- Git
- SVN
- Mercurial

Hiện nay Git là hệ thống quản lý phiên bản được sử dụng phổ biến nhất.

---

# 2. Git

## Git là gì?

Git là một Distributed Version Control System (DVCS).

Mỗi lập trình viên đều có một bản sao đầy đủ của repository trên máy tính của mình.

---

## Một số khái niệm

### Repository (Repo)

Là nơi chứa source code và toàn bộ lịch sử thay đổi.

Có hai loại:

- Local Repository
- Remote Repository (GitHub, GitLab, Bitbucket...)

---

### Working Directory

Là thư mục đang làm việc trên máy.

---

### Staging Area

Là khu vực tạm để chuẩn bị commit.

Thêm file vào staging bằng:

```bash
git add .
```

hoặc

```bash
git add filename
```

---

### Commit

Commit là việc lưu lại một phiên bản của source code.

Ví dụ:

```bash
git commit -m "Create lesson 02 notes"
```

---

### Push

Đẩy source code từ Local Repository lên Remote Repository.

```bash
git push
```

---

### Pull

Lấy source code mới nhất từ Remote Repository.

```bash
git pull
```

---

### Clone

Tải toàn bộ repository về máy.

```bash
git clone <repository_url>
```

---

## Một số lệnh Git thường dùng

Khởi tạo Git

```bash
git init
```

Kiểm tra trạng thái

```bash
git status
```

Xem lịch sử commit

```bash
git log
```

Thêm file

```bash
git add .
```

Commit

```bash
git commit -m "message"
```

Push

```bash
git push
```

Pull

```bash
git pull
```

Clone

```bash
git clone <url>
```

Xem branch

```bash
git branch
```

Chuyển branch

```bash
git checkout branch-name
```

Tạo branch mới

```bash
git checkout -b new-branch
```

---

# 3. JavaScript Basic

## Biến

Khai báo biến

```javascript
let name = "Playwright";
const age = 20;
var oldVariable = "Old";
```

Khuyến nghị:

- Ưu tiên dùng `const`
- Dùng `let` khi cần thay đổi giá trị
- Hạn chế dùng `var`

---

## Kiểu dữ liệu

Primitive Types

- Number
- String
- Boolean
- Null
- Undefined
- BigInt
- Symbol

Reference Types

- Object
- Array
- Function

Ví dụ

```javascript
const name = "Khoa";
const age = 29;
const isTester = true;

const skills = ["Git", "JavaScript", "Playwright"];

const person = {
    name: "Khoa",
    age: 29
};
```

---

## Toán tử

```javascript
+
-
*
/
%

==
===

!=
!==

>
<
>=
<=

&&
||
!
```

Nên sử dụng

```javascript
===
```

thay vì

```javascript
==
```

---

## Điều kiện

```javascript
if (score >= 8) {
    console.log("Good");
} else {
    console.log("Try again");
}
```

---

## Switch

```javascript
switch (day) {
    case 1:
        console.log("Monday");
        break;

    default:
        console.log("Unknown");
}
```

---

## Vòng lặp

For

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

While

```javascript
while (count < 5) {
    count++;
}
```

For...of

```javascript
for (const item of items) {
    console.log(item);
}
```

---

## Function

```javascript
function sum(a, b) {
    return a + b;
}
```

Arrow Function

```javascript
const sum = (a, b) => {
    return a + b;
};
```

Hoặc

```javascript
const sum = (a, b) => a + b;
```

---

## Array

```javascript
const numbers = [1, 2, 3];
```

Các hàm thường dùng

```javascript
push()

pop()

shift()

unshift()

map()

filter()

find()

includes()

forEach()
```

Ví dụ

```javascript
const evenNumbers = numbers.filter(n => n % 2 === 0);
```

---

## Object

```javascript
const student = {
    name: "Khoa",
    age: 29
};

console.log(student.name);
```

---

## Template String

```javascript
const name = "Khoa";

console.log(`Hello ${name}`);
```

---

## Destructuring

```javascript
const person = {
    name: "Khoa",
    age: 29
};

const { name, age } = person;
```

---

## Spread Operator

```javascript
const arr1 = [1,2];
const arr2 = [...arr1,3,4];
```

---

## Promise (Làm quen)

```javascript
const promise = new Promise((resolve) => {
    resolve("Done");
});
```

---

## Async/Await

```javascript
async function getData() {
    const data = await fetchData();
    return data;
}
```

Đây là cú pháp sẽ được sử dụng rất nhiều khi học Playwright.

---

# Tổng kết

Sau buổi học mình đã nắm được:

- Hiểu Version Control System là gì.
- Biết Git hoạt động như thế nào.
- Biết sử dụng các lệnh Git cơ bản.
- Biết tạo và quản lý repository.
- Hiểu cú pháp JavaScript cơ bản.
- Có nền tảng để tiếp tục học Playwright và viết Automation Test.

---

# Các lệnh Git cần nhớ

```bash
git init
git clone <url>
git status
git add .
git commit -m "message"
git push
git pull
git log
git branch
git checkout branch-name
git checkout -b new-branch
```