# Package Manager

## Khái niệm:

- Là công cụ dùng để quản lý các package trong dự án
- Nó tự động xử lý các phần phụ thuộc (dependency) của dự án theo nhiều cách khác nhau.

## Npm là gì ? 

- Npm : Node package manager
- Là 1 công cụ và quản lý các thư viện lập trình Js cho node.js
- Nó giúp cho các dự án mới tránh phải viết lại các thành phần cơ bản, các thư viện hay là các framework
- Nó gồm 3 phần: 
    -  a website quản lý các mặt về npm ( npmjs.com)
    -  a registry giúp truy cập về cơ sở dữ liệu gói JS công cộng đa dạng (kho lưu trữ)
    -  a command-line interface (CLI) Giao diện dòng lệnh tương tác với npm thông qua terminal (giao tiếp, tương tác)
- Khi cài thư viện thì nó cài từng thằng 1
- Nếu có ít bộ nhớ nên dùng npm

## YARN là gì?

- YARN: Yet Another Resource Negotiator
- Sản phẩm của FB in 10/2016
- Cũng giống như npm yarn cũng là 1 trình quản lý package
- Yarn ra đời với mục tiêu ban đầu là giải quyết được các nhược điểm của npm như hiệu suất và bảo mật. 

## Cài đặt NPM,YARN

### NPM 

- Project scope:
    -  npm install react react-dom => dependencies
    -  npm i react react-dom => dependencies

    -  npm install --save-dev react react-dom => devDependencies
    -  npm i -D react react-dom => devDependencies
-  Global
    -  npm i --global create-react-app
    -   npm i -g create-react-app

- Gỡ: npm uninstall -g create-react-app

### YARN

- Khi cài thư viện thì nó có thể cài song song
- Có thể cài thư viện nhanh hơn npm, nhưng không có nghĩa là nhanh gấp nhiều lần
- Nếu muốn nhanh hơn 1 xíu và thừa dung lượng thì có thể dùng yarn
- Yarn install:
    -  npm i -g yarn

------------------------------------------------------------------------------------------------

# SPA/MPA?

## SPA - Single-Page Application

- ReactJS là 1 trong những thư viện tạo ra SPA
- Các trang web lớn sử dụng SPA: Google, Facebook, Twitter
- Các SPA khác: F8, Shoppe, 30Shine, chotot, zingmp3

## Cách triển khai

- SPA - Single-Page Application -> SCR -> Client side rendering
- MPA - Multi-Page Application -> SSR -> Server side rendering
  
## Sự khác biệt

### SPA

- Được cho là cách tiếp cận hiện đại hơn
- Không yêu cầu tải lại trang trong quá trình sử dụng

### MPA

- Là cách tiếp cận cổ điển hơn
- Tải lại trang trong quá trình sử dụng ( click 
---
## So sánh

### Tốc độ

- SPA nhanh hơn khi sử dụng
    - Phần lớn tài nguyên được tải trong lần đầu
    - Trang chỉ tải thêm dữ liệu mới khi cần
- MPA chậm hơn khi sử dụng
    - Luôn tải lại toàn bộ trang khi truy cập và chuyển hướng

### Bóc tách

- SPA có phần Front-end riêng biệt
- MPA FE & BE phụ thuộc nhau nhiều hơn, được đặt trong cùng 1 dự án

### SEO

- SPA không thân thiện với SEO như MPA 
- Trải nghiệm trên thiết bị di động tốt hơn

### UX 

- SPA cho trải nghiệm tốt hơn, nhất là các thao tác chuyển trang
- Trải nghiệm trên thiết bị di động tốt hơn

### Quá trình phát triển

- SPA dễ dàng tái sử dụng code (component)
- SPA bóc tách FE & BE
    - Chia team phát triển song song
    - Phát triển thêm mobile app dễ dàng

### Phụ thuộc vào JS

- SPA phụ thuộc hoàn toàn JS
- MPA có thể không cần JS


# Tài liệu tham khảo:

- https://www.sitepoint.com/yarn-vs-npm/
- https://www.youtube.com/watch?v=30sMCciFIAM&list=PL_-VfJajZj0UXjlKfBwFX73usByw3Ph9Q&index=2

---------------------

# React-Dom

- DOM ( Document Object Model) là 1 thư viện giao diện người dùng giống như các phần tử, thuộc tính.
- Bất cứ khi nào phương thức setState() được gọi, ReactJS reset Dom ảo từ đầu.
- Việc tách biệt logic liên quan đến việc rendering ra khỏi DOM cho phép React chạy được trên nhiều môi trường khác nhau thay vì chỉ 1 môi trường duy nhất là trình duyệt
- Sử dụng Virtual DOM cho phép tính toán các thay đổi trên đó và áp dụng đồng thời các thay đổi đó lên Actual DOM khi cần thiết
- Thao tác DOM thường xuyên rất tốn kém và hiệu suất nặng.
- Khi thay đổi trạng thái xảy ra, DOM ảo được cập nhật và phiên bản trước đó và phiên bản hiện tại của DOM ảo được so sánh. Điều này được gọi là "diffing".
- Sau đó, DOM ảo sẽ gửi một bản cập nhật hàng loạt đến DOM thực để cập nhật giao diện người dùng.
- React sử dụng DOM ảo để nâng cao hiệu suất của nó.
- Nó sử dụng những gì có thể quan sát được để phát hiện những thay đổi trạng thái và chống đỡ.
- React sử dụng một thuật toán diffing hiệu quả để so sánh các phiên bản của DOM ảo.
- Sau đó, nó đảm bảo rằng các bản cập nhật theo đợt được gửi đến DOM thực để sơn lại hoặc kết xuất lại giao diện người dùng.

# Tài liệu tham khảo:
- https://viblo.asia/p/hieu-sao-ve-virtual-dom-trong-reactjs-bWrZngDblxw
- https://codestus.com/posts/react-virtual-dom-duoc-hieu-nhu-the-nao#h2-tom-tat-lai
- https://www.youtube.com/watch?v=zWOREJxiRVY&list=PL_-VfJajZj0UXjlKfBwFX73usByw3Ph9Q&index=11

---------------------

# JSX

- Nó giống như một syntax extension giúp code trở nên mượt và dễ đọc hơn
- Nó transform cú pháp dạng gần như XML về thành JS, giúp người lập trình có thể code React bằng cú pháp của XML thay vì sử dụng JS.
- Các XML elements, attributes và children được chuyển đổi thành các đối số truyền vào React.createElement

----------------------------------------------------------

# React.createElement(type,prop,childrens)

## React element types | React components

- React element types: string, function/class
- Khi sử dụng hàm làm componen thì tên hàm phải viết hoa chữ cái đầu mỗi từ 

## Props

- React elements
    - Sử dụng props giống như với attribute của thẻ HTML
- 2 props class, for => className,htmlFor
- Phải tuân theo quy ước có sẵn
- React components
- Sử dụng props giống như đối số cho component
- Tư do đặt tên props
    - Đặt theo camelCase
    - Có thể bao gồm dấu gạch ngang
- Chú ý:
    - Prop "key" là prop đặc biệt
    - Prop cơ bản là đối số của component
=> Props có thể là bất cứ dữ liệu gì 
    - Sử dụng destructuring 
