# CE118_Project
design MUL_DIV_32bit_unsign \n
Bộ nhân chia số 32-bit không dấu bao gồm bộ nhân số 32-bit không dấu ghép với bộ chia số 32-bit không dấu lại với nhau và được lựa chọn/khởi động bằng cách truyền tín hiệu tích cực mức cao vào chân start của mỗi bộ. Do chưa khắc phục được việc chỉ cho 1 bộ nhân hoặc chia được hoạt động tại cùng một thời điểm nên nếu truyền 2 tín hiệu tích cực mức cao vào cả 2 chân start của 2 bộ sẽ làm cho cả hai cùng hoạt động.
Giá trị số chia chỉ có thể khởi tạo tối đa 31 bit do cần 1 bit để làm bit dấu, nếu không thì khi chuyển thành số bù 2 để thực hiện phép trừ với số bị chia sẽ làm cho bit MSB sai, mà bộ chia dùng tín hiệu của bit lớn nhất đó để quyết định giá trị kế tiếp của số bị chia 
