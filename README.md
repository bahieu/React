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