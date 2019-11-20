# BabyPwn
  Points: 100
# Question
    What happen when you eat too much food at a moment? You can be buffer overflow or stomach overflow ?
    nc 34.80.245.238 33333
# Solution
     Đọc đề bài thì đây có thể là bài về buffer overflow (Lỗi tràn bộ đệm)
    Lỗi tràn bộ đệm là khi bộ nhớ bị ghi đè nhiều lần nên mình sẽ gửi 1 lượng lớn dữ liệu đến sever để làm vượt quá khả năng xử lí của chương trình, từ đó khai thác được lỗi tràn bộ đệm.
    Mở Terminal và netcat đến vị trí đề bài cho
         nc 34.80.245.238 33333
    Màn hình hiện ra dòng chữ:
         Input your name:
    Gõ một dãy chữ "a" dài và nhấn enter
         aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
   
# Flag
    miniCTF{S1mP13_Bu773r_0v3rf0w}

    
