# AI-Project5

Câu 1.

- Chạy vòng lặp qua training data
  - Tìm training data có điểm lớn nhất

Câu 2.

- Khai báo list kết quả
- Chạy vòng lặp 100 lần
  - Với mỗi lần lập lấy ra key có value lớn nhất trong weights thêm vào list kết quả
  - gán value của key vừa lấy ra = -9999999

Câu 3.

- Loop
- Làm tưởng tự với câu 1
- Phần cập nhật: theo phần mô tả của tài liệu
  - Check accuracy:
  - 2 vòng loop lồng nhau trên validationData -> validationLabels
  - Tìm labelMax -> Tính tổng số labelMax = validationLabels[i]
  - Cập nhật weights = gridWeights[Cmax]

Câu 4.
Chạy loop (x -> DIGIT_DATUM_WIDTH, y -> DIGIT_DATUM_HEIGHT)
Nếu (x, y) là khoảng trắng và chưa thăm: thêm vào thăm, gọi hàm determineWhiteRegion(), số vùng trắng += 1
Hàm determineWhiteRegion(): sử dụng BFS để tìm khoảng trắng liên tiếp từ vị trí hiện tại
Cập nhật features[số vùng trắng] = 1, còn lại features = 0

Câu 5.

- Tương tự câu 1
  labelMax != trainingLabel[i]:
- Cập nhật weight:
  weight += trainingData[0]trainingLabel[i]]
  weight -= trainingData[0][labelmax]

Câu 6.

- Các features được xây dựng bằng cách lấy khoảng cách Manhattan ngắn nhất
