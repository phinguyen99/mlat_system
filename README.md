# mlat_system
This repository describes all the steps, which are already installed and set up in our system
1. Tải và cài đặt Tailscale
   Trên Ubuntu, theo command sau đây:
   
   curl -fsSL https://tailscale.com/install.sh | sh
   
   Theo tài khoản của anh Nguyễn Anh Tuấn
   gmail:tuancoiz4@gmail.com
2. Tải và cài đătj driver cho RTLSDR
3. Tải và cài đặt dump 1090 của flightaware
   link: https://github.com/flightaware/dump1090
   Chú ý chạy file deb xuất ra:
   $ sudo dpkg -i dump1090-fa_10.0.1~bpo11+1_amd64.deb 
4. tar 1090 wiedehpf
   https://github.com/wiedehopf/tar1090
5. mlat client
   git clone trước, sau đó tạo virtual environment bên trong thư mục mlat-client
8. viết Service
   $ sudo nano /etc/systemd/system/mlat-client.service
   copy file Service vào, chú ý sửa tên User, và địa điển lat, lon, alt, dẫn nguồn directory
10. 
