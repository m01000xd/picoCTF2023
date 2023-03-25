![image](https://user-images.githubusercontent.com/122852491/227704464-df46062e-bf8b-4c98-ad43-c94a480dc8fd.png)

Chal yêu cầu chúng ta chơi một trò chơi tên là CoreWars. Sau khi nghiên cứu trên google một lúc, thì đây là định nghĩa về CoreWars:

![image](https://user-images.githubusercontent.com/122852491/227704601-961cd80a-4fdc-4d0e-8dca-a4c2076e3c89.png)

"CoreWars là một trò chơi lập trình nơi các chương trình assembly cố gắng tìm cách để tiêu diệt nhau trong bộ nhớ của máy tính mô phỏng"

Đây là những thứ nền tảng khi chơi CoreWars:

![image](https://user-images.githubusercontent.com/122852491/227704896-771a18e9-0561-4679-aecd-deedf470a956.png)

* Ngôn ngữ được sử dụng trong CoreWars là Redcode, 1 ngôn ngữ assembly
* Redcode được chạy bởi một chương trình tên là MARS (Memory Array Redcode Simulator)
* Các chương trình của đối thủ cạnh tranh được gọi là "warriors", được viết bằng Redcode, do MARS quản lý
* Đơn vị cơ bản không phải là byte, mà là dòng lệnh.
* MARS thực hiện 1 lệnh tại 1 thời điểm.


Vậy thì Redcode trông như thế nào ? Chương trình CoreWars đơn giản nhất là Imp:

![image](https://user-images.githubusercontent.com/122852491/227705980-fa9dfff6-a9f6-4a0e-a29e-8ee96494d24e.png)

Đây là 1 câu lệnh assembly đơn giản, nó sao chép dòng ở địa chỉ 0 sang dòng ở địa chỉ 1.

Challenge cung cấp cho chúng ta server để chơi. Theo chal, đối thủ của chúng ta là Imp, và: 

![image](https://user-images.githubusercontent.com/122852491/227706674-28a73db9-123a-4615-a794-0936874f42cf.png)

Nó bắt chúng ta làm thế nào để luôn luôn thua, không được hòa trong trò chơi CoreWars này.

E thử chạy server trên Linux:

![image](https://user-images.githubusercontent.com/122852491/227706767-340a0b97-1d1f-45f2-bfe9-058415b68b06.png)

![image](https://user-images.githubusercontent.com/122852491/227706834-613ab2cf-01e7-4d53-b84f-87ec4f49c402.png)

Nếu thêm dòng mov 0, 1 như trên rồi mới end thì nó sẽ trả về hòa, mà challenge yêu cầu phải luôn luôn thua, không được hòa. Vậy e nghĩ để thua thì chỉ cần mỗi dòng end. E chạy lại server, và flag hiện ra:

![image](https://user-images.githubusercontent.com/122852491/227707008-53873c0e-ed42-4c7b-9e7c-3853ee290c2d.png)



* Flag: picoCTF{h3r0_t0_z3r0_4m1r1gh7_a7bf8a57}
