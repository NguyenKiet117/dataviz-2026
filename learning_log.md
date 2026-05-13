## Lỗi gặp phải & Cách khắc phục

### Lỗi 1: Markdown không render (không hiển thị heading, bold, bảng)
**Mô tả lỗi:**  
Viết #, **text**, bảng nhưng vẫn hiển thị như text thường.

**Nơi tìm giải pháp:**  
Thử phím **M** để chuyển cell sang Markdown và tra “jupyter markdown not rendering”.

**Kết quả:**  
Đã thành thạo cách chuyển cell sang Markdown và sử dụng cú pháp cơ bản.

---

### Lỗi 2: Nhầm lẫn giữa `pd.melt()` và `pd.pivot_table()`
**Mô tả lỗi:**  
Không hiểu rõ `melt` dùng để chuyển wide → long, còn `pivot_table` dùng để tạo bảng tổng hợp.

**Nơi tìm giải pháp:**  
Đọc tài liệu pandas.pydata.org và thử chạy nhiều ví dụ.

**Kết quả:**  
Đã phân biệt rõ công dụng của từng hàm và biết khi nào nên dùng.

---

## Tài nguyên tự học (YouTube)

**Video đã xem:**  
**"Learn Pandas in 30 Minutes - Python Pandas Tutorial"** của Tech With Tim  
Link: https://www.youtube.com/watch?v=EXIgjIBu4EU

**Điều học được:**  
Học được cách sử dụng `df.loc[]` và `df.iloc[]` một cách hiệu quả để chọn dữ liệu, cũng như cách kết hợp nhiều điều kiện lọc dữ liệu nhanh chóng. Video giúp mình hiểu rõ hơn về indexing trong pandas.

---

## Điều tự học được ngoài bài giảng

**Tìm hiểu thêm về `pd.cut()` và `pd.qcut()`**  
Mình tự tìm hiểu hai hàm này để **phân nhóm (binning)** dữ liệu số.  
- `pd.cut()`: Chia theo khoảng giá trị cố định (ví dụ: chia tuổi thành Trẻ em, Thanh niên, Trung niên).  
- `pd.qcut()`: Chia theo phân vị để các nhóm có số lượng gần bằng nhau.  
Rất hữu ích khi muốn chuyển cột `age` hoặc `fare` thành nhóm để phân tích và vẽ biểu đồ.

---

## Tóm tắt quá trình học

- **Điều khó nhất:**  
  Phân biệt và chọn đúng hàm phù hợp giữa `groupby`, `pivot_table`, `melt`, `crosstab` và `apply`.

- **Điều thú vị nhất:**  
  Dùng pandas phân tích Titanic và thấy dữ liệu lịch sử có thể kể lại câu chuyện rất rõ ràng (phụ nữ & trẻ em được ưu tiên, người giàu có lợi thế sống sót).

- **Câu hỏi còn chưa có câu trả lời:**  
  Ngoài giới tính, hạng vé và tuổi, còn những yếu tố nào (như vị trí cabin cụ thể hoặc thông tin về thủy thủ đoàn) ảnh hưởng mạnh nhất đến tỷ lệ sống sót trên tàu Titanic?