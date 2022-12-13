LINK BÀI LAB: https://www.vulnhub.com/entry/vulncms-1,710/

Tiến hành setup lab thành công 

![image](https://user-images.githubusercontent.com/72652376/125251254-51c19880-e321-11eb-84e5-5d23490fa39d.png)

Scan nmap:

![image](https://user-images.githubusercontent.com/72652376/125251718-cf85a400-e321-11eb-8313-3f2bf0d481e4.png)


Scan gobuster port 80:

![image](https://user-images.githubusercontent.com/72652376/125252326-6f433200-e322-11eb-8f44-764d14e14a6a.png)

Có 2 thư mục khác nằm trong file robots.txt. Xem từng thư mục

/home.html

![image](https://user-images.githubusercontent.com/72652376/125252506-a9143880-e322-11eb-9588-b65b56e58a6e.png)

Có vẻ gợi ý đổi tên host thành fsociety.web(truy cập /etc/hosts để thêm tên miền)

/about.html

![image](https://user-images.githubusercontent.com/72652376/125252590-bdf0cc00-e322-11eb-8aaf-e9b6f8a650f4.png)


Không nên dùng burce force tốn thời gian...:v 


Scan port 5000 thu được web sử dụng WPS:

![image](https://user-images.githubusercontent.com/72652376/125253828-065cb980-e324-11eb-94cc-b0dddc5bf745.png)


Scan được rất nhiều thư mục ẩn:

![image](https://user-images.githubusercontent.com/72652376/125254226-7703d600-e324-11eb-9294-16b70d0f6796.png)

![image](https://user-images.githubusercontent.com/72652376/125254289-87b44c00-e324-11eb-83bb-8010e4d49013.png)

Thử truy cập từng trang một...... 

/atom tải về một source code 

![image](https://user-images.githubusercontent.com/72652376/125254769-fb565900-e324-11eb-82a8-6013cfdf5baa.png)

Không scan được mà có thể truy cập được... Có vấn đề

![image](https://user-images.githubusercontent.com/72652376/125254896-1b861800-e325-11eb-96b8-e64c003e48c1.png)

Thử đổi đường dẫn xem code bên dưới có đổi không thì hiện giao diện cmd.


![image](https://user-images.githubusercontent.com/72652376/125255565-c565a480-e325-11eb-8fa6-2d8c8fca6963.png)

User và pass của joomla(port 8081)

![image](https://user-images.githubusercontent.com/72652376/125272141-b555c100-e335-11eb-8b9d-a5aa343d7935.png)


Tìm kiếm các trường hợp nhưng không thể đọc cũng không thể up root

![image](https://user-images.githubusercontent.com/72652376/125265976-8c323200-e32f-11eb-8753-cb2bf0d1ef6c.png)

![image](https://user-images.githubusercontent.com/72652376/125266059-9e13d500-e32f-11eb-9dfa-cb0c3c73230e.png)

Thu được 3 user

SCAN PORT 8081:

![image](https://user-images.githubusercontent.com/72652376/125272926-973c9080-e336-11eb-9a18-8da08268c4e3.png)

Login với thông tin thu được ở trên:

![image](https://user-images.githubusercontent.com/72652376/125273046-ba674000-e336-11eb-8702-1654c949bd18.png)

Tìm kiếm được tên user người dùng và chuỗi có thể là password

![image](https://user-images.githubusercontent.com/72652376/125273301-fac6be00-e336-11eb-9b21-7de0cd30acbc.png)

Login thành công thu được user.txt

![image](https://user-images.githubusercontent.com/72652376/125273461-25187b80-e337-11eb-87b4-10854e85e3c6.png)

Port 9001:

![image](https://user-images.githubusercontent.com/72652376/207228003-14f991e3-6688-4adf-8012-b0b5df512349.png)

![image](https://user-images.githubusercontent.com/72652376/207228074-66ed4390-12d8-4e1b-91b0-e15da7aee74d.png)

Link: https://www.exploit-db.com/exploits/41564


OR unix/webapp/drupal_drupalgeddon2 msfconsole

![image](https://user-images.githubusercontent.com/72652376/207228171-339af964-f8fe-4f6a-adcd-ea5fda9c3012.png)

![image](https://user-images.githubusercontent.com/72652376/207228279-a3ff77a7-907e-4a77-b3dc-a61a7cd2b555.png)


cat tyrell.pass

Username: tyrell

Password: mR_R0bo7_i5_R3@!_

SSH vào tài khoản trên.

Kiểm tra để leo thang:

![image](https://user-images.githubusercontent.com/72652376/207228637-1e3d6d2b-921d-4297-ac8a-62bd26c97855.png)

![image](https://user-images.githubusercontent.com/72652376/207228697-471f0be5-32c6-4e3f-9f43-f38a171e173e.png)

Oke dễ rồi bây giờ thực hiện lên root là xong

![image](https://user-images.githubusercontent.com/72652376/207228749-b3575eb8-186b-4d0c-b7cc-4f869d336603.png)

Done !!

