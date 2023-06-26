# BNBS

## Cài đặt môi trường

1. Cài đặt Git trên máy tính của bạn. Để biết chi tiết, xem [hướng dẫn cài đặt Git](#cài-đặt-git).
2. Tải và cài đặt Python từ [trang web chính thức của Python](https://www.python.org/downloads/).
3. Tải và cài đặt Node.js từ [trang web chính thức của Node.js](https://nodejs.org/).

## Cài đặt Git

1. Truy cập vào trang web chính thức của Git tại https://git-scm.com/.
2. Tải xuống bản cài đặt Git cho Windows và cài đặt theo hướng dẫn.
3. Sau khi cài đặt xong, mở Command Prompt hoặc Terminal và kiểm tra phiên bản Git bằng lệnh sau:

   ```bash
   git --version
   
## Cài đặt các module cho node.js
1. Vào thư mục chương trình ấn chuột phải chọn git bash

2. Chạy lệnh sau để cài đặt các gói phụ thuộc:

   ```bash
   npm install axios web3 dotenv
## Tải dữ liệu từ dune
1. Tạo tài khoản dune
2. Tải file csv từ các querry trên dune cho các hệ như bnbs, erc-20, nrc-20 cái này tìm trên twitter
Querry của bnbs: https://dune.com/queries/2650449
3. Sau khi tải xong lưu file với tên data.csv
## Lọc dữ liệu
### Lọc dữ liệu theo tick
1. Lọc dữ để xuất ra tick muốn mint
2. Mở file filtter.py bằng notepad và chỉnh trong phần tick thành tick bạn muốn lọc
3. Chạy file filter.py sau khi chạy thành công sẽ có file mint.csv được tạo ra trong đây chứa toàn bộ các id mà tick đã mint
### Lọc id đã mint
1. Mở file parsingID.py bằng notepad
2. Sửa trong phần mint_instruction thành chuỗi utf-8 bạn muốn mint
3. Chỉnh id chạy từ 1 đến id mong muốn lọc (dực trên tổng cung và limit per mint để tính)
4. Chạy file parsingID.py sau khi hoàn thành sẽ nhận được file mintable.txt trong này chưa chuỗi utf-8 kèm id chưa mint sử dụng cho tool để mint
## Auto mint
1. Mở file .env bằng notepad sau đó điền địa chỉ ví, private key và gas limit
2. Chạy file mint.js bằng git
