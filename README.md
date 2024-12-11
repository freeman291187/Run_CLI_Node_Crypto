# Nexus Prover by @freeman291187

## Phương pháp 1: Web Browser
Truy cập liên kết này để đóng góp vào Nexus zkVM: https://beta.nexus.xyz/
Điền Email của bạn vào, lưu lại ở phần **Profile**, quay lại **Dashboard** bấm nút **CONNECT** để bắt đầu kiếm Point.


## Phương pháp 2: Linux Server
**1. Cài đặt Dependecies**
```console
sudo apt update && sudo apt upgrade -y
```
**2. Cài đặt các gói**
```console
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```
**3. Cài đặt Rust**
```console
sudo curl https://sh.rustup.rs -sSf | sh
```
**4. Thêm Rust vào đường dẫn**
```console
source $HOME/.cargo/env
export PATH="$HOME/.cargo/bin:$PATH"
```
```console
rustup update

rustc --version
```
```console
sudo apt install -y protobuf-compiler
```

**5. Chạy Prover**

*Dọn sạch màn hình:*
```console
screen -S nexus
```
*Chạy:*
```console
sudo curl https://cli.nexus.xyz/install.sh | sh
```
- Nhập ID Prover: Là dãy ký tự phía dưới góc bên phải màn hình, có dạng PROVER ID:

Thu nhỏ màn hình: `CTRL+A+D`

Để quay lại màn hình: `screen -r nexus`

Để chạy lại trình kiểm tra nếu gặp bất kỳ vấn đề nào:
```console
sudo curl https://cli.nexus.xyz/install.sh | sh
```

**3. Lưu File ID Prover**

Bạn sẽ nhận được 1 File có tên `prover-id` trong thư mục `/root/.nexus/` đại diện cho ID đóng góp duy nhất của bạn cho Prover Node.


---
- Xong !! Hãy thoải mái đặt câu hỏi thông qua Facebook
- Facebook - https://www.facebook.com/freeman.crypto/
- Youtube - 
