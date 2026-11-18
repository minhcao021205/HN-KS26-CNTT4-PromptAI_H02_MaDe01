# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 01
- **Họ tên:** Vũ Cao Minh
- **Lớp:** KS26-CNTT4
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt tour ra JSON

**KET QUA AI**

```text
[  
{  
"ma_tour": "SP2N",  
"ngay_khoi_hanh": "2026-12-20",  
"nguoi_lon": 2,  
"tre_em": 1,  
"loai_phong": "doi",  
"ghi_chu": null  
},  
{  
"ma_tour": null,  
"ngay_khoi_hanh": "2027-01-05",  
"nguoi_lon": 3,  
"tre_em": 0,  
"loai_phong": null,  
"ghi_chu": "1 người ăn chay"  
},  
{  
"ma_tour": null,  
"ngay_khoi_hanh": null,  
"nguoi_lon": 4,  
"tre_em": 0,  
"loai_phong": "doi",  
"ghi_chu": "Ông nội đi xe lăn"  
}  
]
```

**Link trò chuyện:** https://chatgpt.com/share/6afd02fb-2528-83ec-af0c-3ea47d9b70bd

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
# **BẢNG BÁO GIÁ TOUR DL3N – ĐÀ LẠT 3 NGÀY 2 ĐÊM**

**Thông tin đoàn:**

-   5 người lớn.
    
-   2 trẻ em (8 tuổi và 10 tuổi).
    
-   1 trẻ em (3 tuổi).
    
-   1 người lớn ở phòng đơn.
    
-   Giá tour người lớn: 3.200.000 đồng/người.
    

## **Bước 1. Tính tiền người lớn**

Số người lớn: 5 người.

\[ 5 \times 3.200.000 = 16.000.000 \]

**Tiền người lớn = 16.000.000 đồng.**

## **Bước 2. Tính tiền trẻ em**

Trẻ em từ 5–11 tuổi tính 70% giá người lớn.

Giá tour một trẻ em:

\[ 3.200.000 \times 70\% = 2.240.000 \]

Hai trẻ em (8 và 10 tuổi):

\[ 2 \times 2.240.000 = 4.480.000 \]

Bé 3 tuổi dưới 5 tuổi được miễn phí:

\[ 1 \times 0 = 0 \]

**Tiền trẻ em = 4.480.000 đồng.**

## **Bước 3. Tính tiền tour**

Tiền tour = Tiền người lớn + Tiền trẻ em.

\[ 16.000.000 + 4.480.000 = 20.480.000 \]

**Tiền tour trước giảm giá = 20.480.000 đồng.**

## **Bước 4. Tính giảm giá đoàn**

Đoàn có 5 người lớn nên đủ điều kiện giảm 5%.

Mức giảm giá:

\[ 20.480.000 \times 5\% = 1.024.000 \]

Tiền tour sau giảm:

\[ 20.480.000 - 1.024.000 = 19.456.000 \]

**Tiền tour sau giảm = 19.456.000 đồng.**

## **Bước 5. Tính phụ thu**

Có 1 người lớn ở phòng đơn.

Phụ thu phòng đơn: 800.000 đồng/người.

\[ 1 \times 800.000 = 800.000 \]

**Tổng phụ thu = 800.000 đồng.**

Lưu ý: Phụ thu không được giảm giá.

## **Bước 6. Tính tổng tiền**

Tổng tiền = Tiền tour sau giảm + Phụ thu.

\[ 19.456.000 + 800.000 = 20.256.000 \]
```

**Link trò chuyện:** https://chatgpt.com/share/6afd0373-3040-83ec-8dad-f6186ffab9be

### b) Kiểm tra kết quả AI

- Kết luận của AI là đúng, đầy đủ các bước

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{  
"loai_su_co": "khach_san",  
"so_khach": 2,  
"so_dem_bi_anh_huong": 2,  
"tom_tat": "Khách sạn 3 sao thay thế khách sạn 4 sao trong 2 đêm đầu, phòng ẩm mốc."  
}
```

**Link trò chuyện:** https://chatgpt.com/share/6afd03f6-7e88-83ec-9a83-5374ffdf4a0d

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
### **BẢNG CHẤM ĐIỂM CÂU TRẢ LỜI NHÂN VIÊN TƯ VẤN**

Tiêu chí

Điểm

Minh chứng

Đề xuất sửa

**1. Đúng thông tin (50%)**

**2,0/5,0**

**Lỗi 1 – Giá tour:** Trích nguyên văn: “Tour Sa Pa 2N1Đ bên em giá 2.200.000đ/người lớn”. Sai vì giá chuẩn là 2.400.000 đồng/người lớn, nhân viên báo thấp hơn 200.000 đồng. **Lỗi 2 – Chính sách hủy:** Trích nguyên văn: “Anh hủy trước 3 ngày thi được hoàn tiền đầy đủ nha anh.” Sai vì chính sách chuẩn quy định hủy trước ngày đi từ 7 ngày trở lên mới được hoàn 100%; từ 3–6 ngày hoàn 50%; dưới 3 ngày không hoàn tiền.

**Sửa lỗi 1:** “Tour Sa Pa 2N1Đ bên em có giá 2.400.000 đồng/người lớn ạ.” **Sửa lỗi 2:** “Về chính sách hủy tour, nếu anh hủy trước ngày đi từ 7 ngày trở lên, công ty hoàn 100% tiền tour; từ 3–6 ngày hoàn 50%; dưới 3 ngày sẽ không được hoàn tiền ạ.”

**2. Đầy đủ (30%)**

**1,5/3,0**

Nhân viên đã trả lời hai nội dung khách cần biết là giá tour và chính sách hủy. Tuy nhiên, chưa có lời mời khách cung cấp ngày đi và số lượng khách để hỗ trợ đặt tour.

Bổ sung: “Anh vui lòng cho em xin ngày dự kiến khởi hành và số lượng khách tham gia để em hỗ trợ kiểm tra lịch khởi hành và tư vấn đặt tour cho anh ạ.”

**3. Giọng điệu (20%)**

**1,5/2,0**

Trích nguyên văn: “đi rất vui luôn ạ”, “Anh cần gì cứ nhắn em nhé!”. Các cách diễn đạt này hơi suồng sã, thiếu tính chuyên nghiệp trong tư vấn dịch vụ.

Sửa thành: “Tour có lịch trình tham quan hấp dẫn, hứa hẹn mang đến cho anh trải nghiệm thú vị ạ. Nếu cần thêm thông tin, em luôn sẵn sàng hỗ trợ anh.”

**TỔNG ĐIỂM**

**5,0/10**

Nhân viên nắm được nội dung cần tư vấn nhưng mắc lỗi nghiêm trọng về giá tour và chính sách hoàn tiền.

Cần kiểm tra thông tin chuẩn trước khi tư vấn và sử dụng ngôn ngữ chuyên nghiệp hơn.

**Nhận xét của quản lý nhân sự:**

Nhân viên đã có thái độ chào hỏi và phản hồi khách hàng, tuy nhiên cần cải thiện độ chính xác của thông tin tư vấn. Đặc biệt, sai lệch về giá và chính sách hủy tour có thể gây thiệt hại tài chính và ảnh hưởng đến uy tín công ty. Cần ghi nhớ bảng giá, chính sách hủy và chủ động thu thập thông tin ngày đi, số lượng khách để hoàn thiện quy trình tư vấn.
```

**Link trò chuyện:** https://chatgpt.com/share/6afd043b-e5b4-83ec-a91c-7d7d3011a2fa

