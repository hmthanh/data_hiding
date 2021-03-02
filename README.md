1. C.
	- Vô hình cao => nhìn qua thì không thấy
	- Tính bền vững không cao => có thể dễ dàng bị xóa
	- Sức chứa không nhiều => Chĩ chèn được 1 bit mỗi dòng

2. D. Tất cả có 10 khoảng trắng, chèn 7.
	Giả sử chèn bit 111 thì có dạng (_ là khoảng trắng)
	a_a__a_a__a_a__a__a__a__a__

3. 0: 10, 1: 01

4. d. Tất cả đều sai
	Dùng khoảng trắng cuối mỗi dòng thì mỗi dòng đều có thể chèn được 1 bit
	Còn chèn ở giữa thì hên xui, có thể không chèn được bit nào cả nếu không đủ khoảng trắng cần chèn để canh lề

5. b. Bền vững hơn nhưng khó cài đặt hơn
	Bền vững hơn vì không bị ảnh hưởng khi bị format
	Dễ cài đặt hơn, không phải tính toán nhiều, chỉ dựa theo yêu cầu để sinh ra số bit

6. 

	Start → noun verb

	1010

	10 -> noun → Alice | Bob | Fred | Barney
	[Fred] verb

	1 -> verb → went fishing where | went bowling where
	[Fred] [went bowling] where

	0 -> where → in Iowa | in Minnesota
	[Fred] [went bowling] [in Iowa]

	==> c. Fred went bowling in Iowa

7. Barney went bowling in Iowa
1110

=> B.

8. D. Khi có nhiều hơn một đường đi từ start symbol đến chuỗi văn bản chứa bit mật

	Khi rút trích mà có thể có nhiều đường đi từ start đếm symbol thì sai, khi đó kết quả rút trích có thể sẽ không chính xác
	
9. C. 8 bit, 0 tương ứng với màu đen

10. d. 24 byte

11. 
	Ảnh Bitmap (nonpalette-based)
		512×512 * 3bytes (1bytesRed - 1bytesG - 1bytesB) = 786432
		
	=> Loại A và C
	
	Ảnh PNG (palette-based)
		512×512* 1 bytes (index palette)+ palette = 262912 
	
	Loại B (Tối thiểu phải lưu index 1bytes : 512×512*1bytes = 262144 bytes > 768)
	
12. 10 (hệ bit) = 2 (hệ 10)
	Khi nhúng bit 1 : 11 (bit) = 3 (hệ 10)
	Khi nhúng bit 0 : 10 (bit) = 2 (hệ 10)
	
	=> B Giữ nguyên hoặc + 1
	
13. 8bit = 0000 0000 (hệ bit ~ 0 hệ 10) hoặc 1111 1111(hệ bit ~ 255 hệ 10)
	
	Nhúng : 0000 0000 -> 0000 0011 : từ 0 tăng lên 3 
	Nhúng : 1111 1111 -> 1111 1100 : từ 256 xuống 252 là 3 đơn vị
	
	=> B Thay đổi một lượng từ - 3 đến 3

14. Trong phương pháp LSB cho bài toán ẩn tin mật trên ảnh, nếu tăng số bit LSB được
sử dụng để nhúng (trong tổng cộng 8 bit) thì:

	D. Sức chứa tăng nhưng tính vô hình giảm
	Nhúng được nhiều bit mật hơn nhưng pixel bị thay đổi nhiêu hơn nên tính vô hình giảm
	
15. Để ý (5, 6, 9) gần với (5, 6, 10) ~ là màu RGB ở index 0 nhất và (5 + 6 + 9)%2 == 0
	=> C. 6 (5, 6, 9)
	
16. 
	(10, 0, 0)%2 = 0
	(7, 7, 2) %2 = 0
	(5, 5, 9) %2 = 1
	=> C. 001

17. Quantization là chia đi bảng quantization để lấy được các số có trọng số nhỏ hơn, khi nhân lại thì có thể không giống với ban đầu (lossy)

18. Tần số thấp -> ảnh 1 màu, tần số cao -> ảnh nhiều màu ~ nhiều gợn sóng
	Tần số thấp chứa nhiều màu nên hệ số cao hơn, tần số cao nhiều gợn sóng nên hệ số thấp
	
	=> d. Các hệ số DCT tần số thấp thường có độ lớn lớn, các hệ số DCT tần số cao
thường có độ lớn nhỏ (độ lớn = trị tuyệt đối của giá trị)

19. Sau khi chia thì tần số cao (quan trọng được giữ lại), tần số thấp (ít quan trọng) được loại bỏ

	=> c. Các hệ số DCT tần số thấp sẽ tăng độ lớn, các hệ số DCT tần số cao sẽ giảm độ
lớn

20. c. Mảng các hệ số DCT sau khi quantization
	quantization là bước làm mất mát thông tin nên cần nhúng sau khi đã làm mất mát thông tin
	
21. c. Không nên nhúng bit mật vào các hệ số tần số cao vì sẽ làm giảm hiệu suất nén
	=> Nhúng vào tần số cao thì phải lưu thông tin đến các hệ số tần số cao cuối cùng nên giảm hiệu suất nén

22. Khi thay các số trong bảng quantization bằng 1 sẽ giúp các hệ số ở giữa đó được giữ nguyên làm tăng tính vô hình.
	d. Để tăng tính vô hình và để tăng hiệu suất nén
	
23. C. “Bit depth” vừa thể hiện mức độ rời rạc hóa theo chiều x (thời gian), vừa thể hiện mức độ rời rạc hóa theo chiều y (cường độ)
	
24. 441000/44100 = 10s 
	B
	
25. b. “Mono” có một sóng, “stereo” có nhiều hơn một sóng

26. a. Độ trễ của echo
	Khoảng cách dộ trễ càng lớn thì sẽ càng nghe rõ được echo
	
27. trong phiên bản dịch trái của sóng stego
	Dịch trái của sóng stego (stego là bản sau khi nhúng) sẽ tương đương với 
	c. Vì tại đó có sự tương tự giữa thành phần sóng gốc trong sóng stego với thành phần sóng echo trong phiên bản dịch trái của sóng stego

28. b. Giá trị autocorrelation của sóng stego tại độ lệch k bằng 0 là lớn nhất và tại độ lệch k bằng độ trễ của echo là lớn nhì

29. c. Steganography đặt nặng về tính vô hình, watermarking đặt nặng về tính bền vững

30. b. Tính vô hình cao, tính bền vững cao, khi rút trích cần đến ảnh gốc

31. d. a và c

32. a. Trong watermarking, A thường chứa thông tin liên quan tới B; còn trong
steganography, A thường chứa thông tin không liên quan gì tới B


Tự luận :
k = 4
f(1) = 22, f(2) = 37, f(3) = 66, f(4) = 115, f(5) = 190

f(x) = 22*f_1(x) + 37*f_2(x) + 66*f_3(x) + 115*f_4(x) + 190*f_5(x)
f_1(x) = {(x-2)(x-3)(x-4)(x-5)}/{(1-2)(1-3)(1-4)(1-5)}
f_2(x) = {(x-1)(x-3)(x-4)(x-5)}/{(2-1)(2-3)(2-4)(2-5)}
f_3(x) = {(x-1)(x-2)(x-4)(x-5)}/{(3-1)(3-2)(3-4)(3-5)}
f_4(x) = {(x-1)(x-2)(x-3)(x-5)}/{(4-1)(4-2)(4-3)(4-5)}
f_5(x) = {(x-1)(x-2)(x-3)(x-4)}/{(5-1)(5-2)(5-3)(5-4)}

Thay f(0) ta được :

f_1(x) = {(0-2)(0-3)(0-4)(0-5)}/{(1-2)(1-3)(1-4)(1-5)} = 5
f_2(x) = {(0-1)(0-3)(0-4)(0-5)}/{(2-1)(2-3)(2-4)(2-5)} = -10
f_3(x) = {(0-1)(0-2)(0-4)(0-5)}/{(3-1)(3-2)(3-4)(3-5)} = 10
f_4(x) = {(0-1)(0-2)(0-3)(0-5)}/{(4-1)(4-2)(4-3)(4-5)} = -5
f_5(x) = {(0-1)(0-2)(0-3)(0-4)}/{(5-1)(5-2)(5-3)(5-4)} = 1

=> f(0) = 22*5 + 37*-10 + 66*10 + 115*-5 + 190*1 = 15