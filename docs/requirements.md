Hệ thống quản lý bệnh viện
1) Giới thiệu đề tài
- Xây dựng cơ sở dữ liệu quản lý bệnh nhân chạy trên sql server, hỗ trợ lưu trữ và quản lý thông tin bệnh nhân, bác sĩ, khoa khám bệnh, lịch khám, hồ sơ bệnh án, thuốc, đơn thuốc, dịch vụ y tế và hóa đơn.
- Hệ thống tập trung vào khám chữa bệnh ngoại trú.
2) Mục tiêu
- Quản lý dữ liệu tập trung và hạn chế trùng lặp.
- Đảm bảo tính chính xác và toàn vẹn của dữ liệu.
- Hỗ trợ tra cứu thông tin bệnh nhân và lịch sử khám.
- Hỗ trợ quản lý đơn thuốc, dịch vụ và thanh toán.
- Hỗ trợ thống kê phục vụ công tác quản lý bệnh viện.
3) Phạm vi và chức năng
3.1) Quản lý khoa
  lưu mã khoa, tên khoa và thông tin liên hệ. Mỗi bác sĩ trực thuộc 1 khoa.
3.2) Quản lý bác sĩ
  Lưu mã bác sĩ, họ tên, ngày sinh, giới tính, số điện thoại, email và khoa trực thuộc.
3.3) Quản lý bệnh nhân
  Lưu mã bệnh nhân, họ tên, ngày sinh, giới tính, số điện thoại, địa chỉ và ngày tạo hồ sơ.
3.4) Quản lý lịch khám
  Ghi nhận bệnh nhân, bác sĩ phụ trách, thời gian khám, lý do khám và trạng thái lịch khám.
3.5) Quản lý hồ sơ bệnh án
  Lưu thông tin triệu chứng, chuẩn đoán, kết luận và ngày lập hồ sơ sau khi bệnh nhân được khám.
3.6) Quản lý thuốc và đơn thuốc
  Quản lý danh mục thuốc, đơn vị tính, đơn giá và số lượng tồn.
  Lưu thông tin đơn thuốc, thuốc được kê, liều dùng và số lượng.
3.7) Quản lý dịch vụ y tế
  Quản lý danh mục dịch vụ, đơn giá và các dịch vụ thực tế trong quá trình khám chữa bệnh.
3.8) Quản lý hóa đơn
  Ghi nhận hóa đơn liên quan đến hồ sơ bệnh án, ngày lập và trạng thái thanh toán.
3.9) Thống kê và báo cáo
  Hỗ trợ thống kê lượt khám theo thời gian, số lượt khám theo bác sĩ hoặc khoa, lịch sử khám của bệnh nhân, thuốc tồn thấp và doanh thu dịch vụ.
4) Đối tượng sử dụng
- Nhân viên tiếp nhận: quản lý thông tin bệnh nhân và lịch khám.
- Bác sĩ: tra cứu lịch khám, lập hồ sơ bệnh án và kê đơn thuốc.
- Nhân viên quản lý thuốc: theo dõi danh mục thuốc và số lượng tồn.
- Nhân viên thu ngân: quản lý hóa đơn và trạng thái thanh toán.
- Ban quản lý: tra cứu số liệu và báo cáo tổng hợp.
5) Quy tắc nghiệp vụ
- Mỗi khoa có một mã khoa duy nhất.
- Mỗi bác sĩ có một mã bác sĩ duy nhất và phải trực thuộc 1 khoa.
- Mỗi bệnh nhân có một mã bệnh nhân duy nhất.
- Mỗi lịch khám thuộc về một bệnh nhân và một bác sĩ.
- Một lịch khám có thể chưa phát sinh hồ sơ bệnh án, mỗi bệnh án chỉ liên kết tối đa 1 hồ sơ.
- Mỗi hồ sơ bệnh án thuộc 1 lịch khám.
- Một hồ sơ bệnh án có thể có nhiều đơn thuốc.
- Một đơn thuốc có thể chưa nhiều loại thuốc, một loại thuốc có thể xuất hiện trong nhiều đơn thuốc.
- Một hồ sơ bệnh án có thể sử dụng nhiều dịch vụ y tế, một dịch vụ có thể sử dụng ở nhiều hồ sơ.
- Một hồ sơ bệnh án có thể chưa có hoặc có tối đa 1 hóa đơn trong phạm vi hệ thống.
- Số lượng thuốc phải lớn hơn không, đơn giá không được âm.
- Các mã định danh không được trùng lặp.
- Chỉ số liệu dịch vụ được ghi nhận hợp lệ mới được sử dụng để thống kê doanh thu dịch vụ.
6) Công nghệ
- Hệ quản trị cơ sở dữ liệu: Microsoft SQL Server.
- Công cụ quản trị: SQL Server Management Studio (SSMS).
- Công cụ thiết kế ERD: draw.io hoặc công cụ tương đương.
- Quản lý mã nguồn và tài liệu: GitHub.
7) Sản phẩm dự kiến
- Tài liệu yêu cầu nghiệp vụ.
- Sơ đồ ERD và thiết kế cơ sở dữ liệu.
- Script tạo database, bảng, ràng buộc và dữ liệu mẫu.
- Các truy vấn SQL, View, Index và Stored Procedure theo yêu cầu đề bài.
- Trigger .
- Hướng dẫn và kết quả kiểm thử backup/restore.
- Báo cáo và slide thuyết trình.
