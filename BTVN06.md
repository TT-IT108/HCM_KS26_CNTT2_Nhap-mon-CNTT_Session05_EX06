**Bài 6 : Thiết lập môi trường làm việc cho hệ thống Smart-Farm trên SoC** 

1.Bản phân tích luồng IPO cho toàn bộ quá trình thiết lập căn cứ số này.

\-Input: Thư mục Home (`~`) và file mẫu `t`emplate.ps1 trong Public.  
\-Process: Tạo thư mục, tạo file .env, sao chép và đổi tên file, kiểm tra cấu trúc.  
\-Output: Thư mục smart-farm có đủ 3 thư mục con bin, config, data và các file nằm đúng vị trí.  
 2.Nhật ký (Log) các câu lệnh PowerShell đã thực hiện.  
\- cd \~; 'bin','config','data' | ForEach-Object { New-Item \-ItemType Directory \-Path   "smart-farm\\\$\_" \-Force }  
\- New-Item \-ItemType File \-Path "\$HOME\\smart-farm\\config\\.env" \-Force  
\-Get-ChildItem "\$HOME\\smart-farm\\config" \-Force  
\- Get-ChildItem "\$HOME\\smart-farm" \-Recurse \-Force

