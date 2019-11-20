# Garbage Collection
   Points: 919
# Question
    Can you analyze it?
# Hint
    wireshark
    http
# Solution
   Dựa vào hint đề cho thì mình dùng wireshark để giải.
   Download file ở đề bài.
   Mở wireshark lên và open file ở đề bài.
   Hint thứ 2 là http nên ta bắt đầu dùng filter để lọc http.
   Nhập http tại ô "Apply a display filter". Ta đã bắt được hàng trăm gói tin http mà thứ ta cần chỉ có ở 1 hoặc 1 số ít gói tin.
   Vậy nên ta dùng đến Export HTTP Object để thu hồi được 1 list các đối tượng được lấy từ các gói tin mà wireshark bắt được.
   Mở tính năng như sau: File -> Export object -> http.
   Nhận thấy 1 list các đối tượng trang uis, kéo xuống thì thấy web tinyupload chuyên dùng để upload trơ trọi giữa rừng uis :v. trong đó có 2 link upload file
   Quay lại filter http, tìm 2 đường link file-upload đó. Nhấp vào link và xem thông tin Hypertext Transfer Procol
   Kéo xuống bên dưới sẽ thấy đường link đi đến web nhưng một đường link là 2/3 và 3/3. 
    Truy cập đến đường link 3/3: [Full request URI: http://s000.tinyupload.com/file_uploaded.php?file_id=30631520752547918930&del_id=15198429202580371804&gk=acunetix_wvs_invalid]
   thì thấy 1 picture được upload lên. 
   Download picture về và thấy là một mã QR code. Quét mã QR ta nhận đc đường link đến notepad online.
   Đến đó ta thấy flag
      "A little fun on the big journey
      Forensic is fun!
      Welcome to PIS Club.
      Here is your flag!!!

      miniCTF{m0`_tR0n9_D0^n9_R@'c_ThA^t_THu'_D1}"
# Flag
       miniCTF{m0`_tR0n9_D0^n9_R@'c_ThA^t_THu'_D1}
