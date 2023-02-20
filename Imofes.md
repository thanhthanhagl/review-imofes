# **Review Imofes**
> [Link web demo Imofes](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/)
***
## **Hình ảnh**
- Tất cả hình xuất 1x.
- Background: 
    + Set background color cho body.
    + Những section có trang trí củ khoai 2 bên thì xuất ra dưới dạng png, chỉ lấy màu các củ khoai không cần lấy màu nền. (Như hình dưới).<br>
    [background-icon](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/images/index/bg-feature.png)

***
## **Cấu trúc web**
### Header + Mainvisual
- Mainvisual nằm trong header.
- Background header không cắt phần màu vàng.<br>
    - [background-header](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/images/common/mv.png)
- Gộp tất cả hình dưới thành 1 group, đặt nó làm h1.<br>
    - [mv](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/images/index/top.png)
- Phần lượn sóng thì cắt hình ra vfa cho z-index thấp hơn.
    - [before mv](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/images/common/mv_before.png)
### **Section info**
- [section info](https://prnt.sc/osTYIziO-a5C)
- Đặt margin là âm (ở đây khách để -20%) để nó đè lên phần bachground dư của header bên trên.
### **Section feature**
- Cách chia bố cục các box:
    - Row 1:chia 2 cột và cắt thành 2 hình riêng, gắn link cho instagram.
    - Row 2: chia 2 cột, 1 cột text, 1 cột hình (group 2 hình 2 lại với nhau).
    - Row 3: 1 hình (group 3 hình lại và export).
*Note 1: Thay vì đặt class phụ *c-feature__row c-feature__title*" thì hãy đặt thành "*c-feature__row --title*"
    c-feature__row c-feature__title -> c-feature__row --title
    => css
    .c-feature {
        &__row {
            &.--title {
            }
        }
    }
*Note 2: Những row chia 2 cột thì khi xuống sp cho nó thành 2 hàng.
**Box cuối**
- Vẫn dùng before và after để chèn ảnh cho box.
- Cắt hình ở trên thành 2 phần. Hình có củ khoai thì cho nó là before của box text.
    - [decor text box](http://aglstaff.allgrow-labo.jp/trandiepthanhthanh/test/images/index/kanta_title.png)

***
## **Chú ý quan trong**
- Không chỉ xóa những hình không dùng đến mà phải xóa tất cả các file không dùng đến như folder cms, page template.
- Khi nộp source code thì nộp luôn folder dist.
