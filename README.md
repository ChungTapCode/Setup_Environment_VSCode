# Setup_Environment_VSCode
Các bước dẫn cài môi trường cho VSCode

# Command
# Cách 1:
* Bạn vào trình duyệt mà bạn hay dùng và search "tdm-gcc" 
* Link : https://jmeubank.github.io/tdm-gcc/download/
* Sau đó bạn tải cái thứ 2 nếu là máy 64 bit, còn 32 bit thì tải cái cuối cùng 
* Sau khi tải cài đặt về thì bạn vào windown gõ "terminal" 
* Ghi 3 lệnh sau :
* gcc --version 
* g++ --version 
* gdb --version
* Nếu nó hiện ra các phiên bản thì có nghĩa là được rồi nhé
* Sau dó bạn vào VSCode tải "C/C++" và "Code Runner" 
* Sau đó viết một chương trình cơ bản và run code để chương trình chạy nhé 
* Vậy xong cách 1 rồi 

# Cách 2:
* Bạn lên mạng search mingw và tải nó về 
* Link : https://sourceforge.net/projects/mingw-w64/
* Bạn tải về sau đó nhập lệnh sau: 
* pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain
* Nhớ là lúc tải cứ nhấn ok thôi nhé để sau k bị sai đường dẫn 
* Sau đó bạn vào This PC và theo đường dẫn này: C:\msys64\ucrt64\bin sao chép nó
* Sau đó bạn vào Windown và tìm : Edit environment variables for your account.
* Sau đó nhấn User variables và nhấn New sau đó dán đường dẫn "C:\msys64\ucrt64\bin " vào đó 
* Sau đó bạn vào terminal và nhấn 3 lệnh lúc nãy để check
* gcc --version 
* g++ --version 
* gdb --version
* Nhưng khi cài cái này có thể bị thiếu trình biên dịch vậy nên bạn nếu nó báo lỗi khi bạn nhập gdb --version thì bạn phải cài thêm , nếu không báo gì có nghĩa là xong rồi đó , bạn vào vscode để code thôi 
* Nếu thiếu bạn có thể làm theo cách sau : mở windown tìm mingw và nhập lệnh sau: 
* pacman -S mingw-w64-x86_64-gdb  
* Sau đó nhập lệnh gdb --version kiểm tra lại nhé 
* Vậy là bạn hoàn thành xong cách 2 rồi đó , chúc các bạn thành công   
