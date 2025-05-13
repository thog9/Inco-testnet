# Inco Testnet Scripts

Bộ sưu tập các script Python được thiết kế để tương tác với **Inco Testnet**, một mạng thử nghiệm blockchain dành cho các ứng dụng phi tập trung. Script chính, `main.py`, cung cấp giao diện dòng lệnh (CLI) thân thiện để thực hiện các thao tác như mint token, shield/unshield USDC, triển khai hợp đồng thông minh và gửi giao dịch. Được xây dựng bằng `web3.py`, các script này hỗ trợ thực thi không đồng bộ và cung cấp đầu ra song ngữ (tiếng Anh và tiếng Việt).

## ✨ Tính năng

### Tính năng chung

- **Hỗ trợ đa tài khoản**: Thực hiện các thao tác trên nhiều ví bằng khóa riêng từ file `pvkey.txt`.
- **Giao diện CLI màu sắc**: Sử dụng `colorama` để tạo đầu ra sinh động với viền và màu sắc.
- **Thực thi không đồng bộ**: Tận dụng `asyncio` để tương tác blockchain hiệu quả.
- **Xử lý lỗi mạnh mẽ**: Phát hiện và báo cáo lỗi giao dịch blockchain và RPC.
- **Hỗ trợ song ngữ**: Hỗ trợ đầu ra bằng tiếng Anh và tiếng Việt tùy theo lựa chọn người dùng.
- **Hỗ trợ proxy**: Tùy chọn sử dụng proxy qua file `proxies.txt` cho các yêu cầu mạng.

### Các Script Bao Gồm

1. **Mint USDC**: Mint token USDC trên Inco Testnet.
2. **Mint cUSDC**: Mint token cUSDC trên Inco Testnet.
3. **Shield USDC ➯ cUSDC**: Chuyển đổi USDC thành cUSDC thông qua hợp đồng shielding.
4. **Unshield cUSDC ➯ USDC**: Chuyển đổi cUSDC trở lại USDC thông qua hợp đồng unshielding.
5. **Triển Khai Hợp Đồng Thông Minh Mintair**: Triển khai hợp đồng thông minh Mintair trên Inco Testnet.
6. **Gửi TX (Ngẫu nhiên hoặc File)**: Gửi giao dịch ngẫu nhiên hoặc đến các địa chỉ trong `address.txt`.
7. **Triển Khai Hợp Đồng Token**: Triển khai hợp đồng token ERC20 trên Inco Testnet.
8. **Gửi Token ERC20 (Ngẫu nhiên hoặc File)**: Gửi token ERC20 đến các địa chỉ ngẫu nhiên hoặc trong `addressERC20.txt`.
9. **Triển Khai Hợp Đồng NFT**: Triển khai hợp đồng thông minh NFT trên Inco Testnet.

## 🛠 Yêu cầu trước khi sử dụng

Đảm bảo các yêu cầu sau được cài đặt và cấu hình:

- **Python**: Phiên bản 3.8 trở lên.
- **pip**: Trình quản lý gói Python.
- **Các gói phụ thuộc**: Cài đặt qua `pip install -r requirements.txt`. Các gói cần thiết bao gồm: ( `web3.py`, `colorama`, `asyncio`, `eth-account`, `aiohttp_socks` and `inquirer` ).
- **pvkey.txt**: File chứa khóa riêng (mỗi dòng một khóa) để tự động hóa ví.
- **Inco Testnet RPC**: Truy cập vào RPC của Inco Testnet (ví dụ: `https://sepolia.base.org` hoặc RPC dành riêng cho Inco).
- **proxies.txt** (tùy chọn): Địa chỉ proxy cho các yêu cầu mạng.

## 📦 Cài đặt

Thực hiện các bước sau để thiết lập dự án:

1. **Clone this repository:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
git clone https://github.com/thog9/Inco-testnet.git
```
```sh
cd Inco-testnet
```
2. **Install Dependencies:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
pip install -r requirements.txt
```
3. **Prepare Input Files:**
- Mở `pvkey.txt`: Thêm khóa riêng của bạn (mỗi dòng một khóa) vào thư mục gốc.
```sh
nano pvkey.txt
```
- Mở `address.txt`(tùy chọn): Thêm địa chỉ người nhận (mỗi dòng một khóa) cho `sendtx.py`, `nftcollection.py`, `deploytoken.py`, `sendtoken.py`, `proxies.txt`.
```sh
nano address.txt 
```
```sh
nano addressERC20.txt
```
```sh
nano contractNFT.txt
```
```sh
nano proxies.txt
```
```sh
nano contractERC20.txt
```
4. **Run:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
python main.py
```
- Chọn ngôn ngữ (Tiếng Việt/Tiếng Anh).

## Liên hệ

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099) 

----

BUYMECAFE: [BUY ME CAFE](https://buymecafe.vercel.app/)
