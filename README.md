# Trên Web
Truy cập liên kết bên dưới, vào Profile điền Email lưu lại, quay lại Dashboard bấn CONNECT là Done!
Contribute to Nexus zkVM Prover : https://beta.nexus.xyz/

# Linux Server
1. Bước 1

```sh sudo apt update && sudo apt upgrade -y ```

2. Bước 2

sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
3. Bước 3: Cài đặt Rust

sudo curl https://sh.rustup.rs -sSf | sh

4. Bước 4: Add Rust to path

source $HOME/.cargo/env
export PATH="$HOME/.cargo/bin:$PATH"
rustup update

rustc --version
sudo apt install -y protobuf-compiler

5. Buwowcs5: Run Prover
Open screen
screen -S nexus
Run:

sudo curl https://cli.nexus.xyz/install.sh | sh
Enter prover id (watch youtube video to know how to get)

To minimize screen: CTRL+A+D
To retun screen: screen -r nexus
To run the prover again if faced any issues

sudo curl https://cli.nexus.xyz/install.sh | sh

3. Save Prover ID file

You'll get a prover-id file in /root/.nexus/ representing your unique contribution ID to Prover Node

