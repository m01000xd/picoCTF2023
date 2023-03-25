Tải file timer.apk về máy.

File apk, vậy chúng ta lại lên http://www.javadecompilers.com/ để decompiler

Kết quả trả về: 

![image](https://user-images.githubusercontent.com/122852491/227442438-76acca1d-c0e9-4b6c-afb4-fe37c08582b4.png)

Thử vào sources folder, rà soát các kiểu thì cũng chẳng có thêm được gì. Vậy nên e quay lại vào folder resources.

![image](https://user-images.githubusercontent.com/122852491/227442713-17a9871d-2cbc-47f0-a9a4-7fe1909f4a48.png)

Bỏ qua 3 folder trên, ta thử xem xét 4 file lẻ kia xem có gì.

File đầu là AndroidManifest.xml, e thử mở trong NotePad, và may thay:

![image](https://user-images.githubusercontent.com/122852491/227443025-c329074b-193e-4a5e-ab1f-5d335c4fb9dc.png)

![image](https://user-images.githubusercontent.com/122852491/227443126-32f9b1db-f047-4d2a-b7a2-49cea400fcf8.png)

* Flag: **picoCTF{t1m3r_r3v3rs3d_succ355fully_17496}**
