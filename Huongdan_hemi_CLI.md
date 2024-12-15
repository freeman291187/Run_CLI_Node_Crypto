# Hemi Network Miner by @freeman291187
---
- Tài liệu gốc - [Hemi_Miner_CLI](https://docs.hemi.xyz/how-to-tutorials/tutorials/setup-part-1)
- Watch Video - [Youtube](https://)

## 1. Binaries:
- Đi đến [binaries](https://github.com/hemilabs/heminetwork/releases)
- Tải tệp có dạng  **......_linux_amd64.tar.gz** phiên bản mới nhất về.
- Copy tệp này vào máy chủ inux 

- Bây giờ bắt đầu các dòng lệnh
```bash
mkdir hemi-miner
```
```bash
cd hemi-miner
```
  
```bash
sudo apt update && sudo apt upgrade -y
```
```bash
sudo apt install screen
```
```bash
screen -S hemi
```
```bash
tar xvf ....._linux_amd64.tar.gz
```
```bash
cd ....._linux_amd64 với tên File và thư mục bạn tạo trên máy chủ Linux.
```
- Lưu ý thay thế **....._linux_amd64.tar.gz** và **....._linux_amd64** với tên File và thư mục bạn tạo trên máy chủ Linux.

## 2. Xác nhận lại:
- Để đảm bảo bạn đã tải xuống đúng tệp nhị phân và có thể chạy chúng, hãy thực hiện lệnh bên dưới:
```bash
./popmd --help
```
- Thao tác này sẽ hiển thị menu trợ giúp cho popmd, cho biết rằng nó đã được cài đặt và hoạt động.

## 3. Tạo khóa công khai của bạn:
```bash
./keygen -secp256k1 -json -net="testnet" > ~/popm-address.json
```
```bash
cat ~/popm-address.json
```
- Kết quả tương tự bên dưới - Hãy chắc chắn bạn lưu lại nó

![image](https://github.com/user-attachments/assets/d035e6b8-f609-443c-b2fe-d9acbf83b1f6)

1. Private key : Khoá bí mật
2. pubkey_hash : Địa chỉ ví BTC

## 4. Nạp tiền vào Địa chỉ PoP Miner của bạn
- Tìm địa chỉ ví của bạn : Lấy địa chỉ BTC ở pubkey_hash, đây là địa chỉ Bitcoin testnet của bạn.
- Có thể vào Discord để nhận vòi tBTC: [Hemi](https://discord.com/invite/hemixyz)
- Hoặc liên hệ facebook: [FreeMan](https://www.facebook.com/freeman.crypto/) Để mua tBTC.
- Bạn tạo ví BTC bằng: [UniSat Wallet](https://unisat.io/), gởi cho [FreeMan](https://www.facebook.com/freeman.crypto/) Để mua tBTC.
## 5. Đặt biến
- Trong bảng điều khiển của bạn, hãy thực hiện các lệnh sau:
1. Thay thế **<private_key>** với giá trị khoá bí mật của bạn ở bước trên.
2. Thay thế **<fee_per_vB_integer>** với mức phí bằng sat/vB mà bạn muốn trả (Bình thường là 50, hoặc tuỳ ý bạn)

```bash
export POPM_BTC_PRIVKEY=<private_key>
export POPM_STATIC_FEE=<fee_per_vB_integer>
export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public
```
3. Kiểm tra mức phí hiện tại : [Mempool](https://mempool.space/testnet)
4. Nhìn vào số "**sat/vB**" numbers cho các mức ưu tiên phí giao dịch khác nhau. Nên đặt giá trị thành giá trị "High Priority-Ưu tiên cao" hoặc cao hơn một chút..
5. Chạy lại lệnh **POPM_STATIC_FEE** để thiết lập  environment variable from above each time you want to change the fee, and restart the PoP Miner afterwards.

## 6. khởi chạy Miner
```bash
./popmd
```
- Kết quả tương tự bên dưới

![image](https://github.com/user-attachments/assets/728af042-e6d3-454c-be69-c3dbeec860e3)

## 7. Cài đặt màn hình hiển thị
- Sau khi chạy sử dụng : CTRL A D (để tách khỏi màn hình)
- Để kiểm tra lại màn hình, hãy sử dụng:
```bash
screen -r hemi
```

---
- Kiểm tra trạng thái Miner : [Miner_Status](https://testnet.popstats.hemi.network/)

- Xong !! Hãy thoải mái trao đổi
- Facebook - [FreeMan](https://www.facebook.com/freeman.crypto/) 
- Github -  [FreeMan](https://github.com/freeman291187/) 
