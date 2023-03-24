Bài này khá đơn giản. Đầu tiên tải file ret về máy.

![image](https://user-images.githubusercontent.com/122852491/227438586-67ba5989-4e82-4dfd-bfc0-575380cb8b88.png)

Đây là file elf, ta mở nó trong IDA

![image](https://user-images.githubusercontent.com/122852491/227438838-54859c4f-adf1-483f-9e48-a64da6aece08.png)

F5 để decompile

![image](https://user-images.githubusercontent.com/122852491/227439318-a42165a4-e475-4e92-8add-7dcbf92ea905.png)

ở dòng 8, đập vào mắt ta sẽ tưởng rằng đây chính là flag. Nhưng nếu để ý kỹ, flag có dạng: picoCTF{...}. Thử nhìn lại 1 lần nữa, dòng 14: 

![image](https://user-images.githubusercontent.com/122852491/227439947-b99a2a65-c7cb-47b0-980b-a5db4e5001c6.png)

"Password correct, please see flag: picoCTF{3lf_r3v3r5ing_succe55ful_7851ef7d}" => flag

* Flag: picoCTF{3lf_r3v3r5ing_succe55ful_7851ef7d}

