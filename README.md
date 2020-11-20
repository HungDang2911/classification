# AI-Project5

Câu 1.

- Chạy vòng lặp qua training data
  - Tìm training label có điểm lớn nhất
  - Nếu y_value != trainingLabels[i]:
      self.weights[trainingLabels[i]] += trainingData[i]
      self.weights[y_value] -= trainingData[i]

Câu 2.

- Khai báo list kết quả
- Chạy vòng lặp 100 lần
  - Với mỗi lần lập lấy ra key có value lớn nhất trong weights thêm vào list kết quả
  - gán value của key vừa lấy ra = -9999999

Câu 3.

- Loop CGrid
- Làm tưởng tự với câu 1
- Phần cập nhật: theo phần mô tả của tài liệu
  - Check accuracy:
  - 2 vòng loop lồng nhau trên validationData -> validationLabels
  - Tìm labelMax -> Tính tổng số labelMax = validationLabels[i]
  - Cập nhật finalWeights = weights[Cmax]

Câu 4.
- Chạy loop (x -> DIGIT_DATUM_WIDTH, y -> DIGIT_DATUM_HEIGHT)
- Nếu (x, y) là khoảng trắng và chưa thăm: thêm vào thăm, gọi hàm dfs(), số vùng trắng += 1
- Cập nhật features

Câu 5.

- Tương tự câu 1
  labelMax != trainingLabel[i]:
- Cập nhật weight:
  weight += trainingData[0]trainingLabel[i]]
  weight -= trainingData[0][labelmax]

Câu 6.

- Các features được xây dựng bằng cách lấy khoảng cách Manhattan ngắn nhất
