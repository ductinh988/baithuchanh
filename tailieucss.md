# ***CSS Introduction***
- CSS là ngôn ngữ chúng ta sử dụng để tạo kiểu một trang web
- CSS là viết tắt của Cascading Style Sheets
- CSS mô tả cách các phần tử HTML được hiển thị trên màn hình, giấy hoặc trong các phương tiện khác
- CSS tiết kiệm rất nhiều công việc. Nó có thể kiểm soát bố cục của nhiều trang web cùng một lúc
- Các bảng định kiểu bên ngoài được lưu trữ trong các tệp CSS
# ***CSS Selectors***
- Bộ chọn phần tử CSS
- Bộ chọn id CSS
- Bộ chọn lớp CSS
- Bộ chọn chung CSS (dung dấu *)
- Công cụ chọn nhóm CSS
# ***Color***
## RBG
- Giá trị màu RGB đại diện cho các nguồn sáng ĐỎ, XANH LÁ và XANH LÁ.
- công thức: (red, green, blue)
- Giá trị màu RGB đại diện cho các nguồn sáng ĐỎ, XANH LÁ và XANH LÁ.
## RGBA
- Giá trị màu RGBA là phần mở rộng của các giá trị màu RGB với kênh alpha - chỉ định độ mờ cho một màu.
- Giá trị màu RGBA được chỉ định bằng
- rgba ( đỏ, lục , lam, alpha )
- rgba ( đỏ, lục , lam, alpha )
## HEX
- Trong CSS, một màu có thể được chỉ định bằng giá trị thập lục phân ở dạng:
- # rrggbb
- Trong đó rr (đỏ), gg (xanh lục) và bb (xanh lam) là các giá trị thập lục phân từ 00 đến ff (giống như số thập phân 0-255).
# HSL
- HSL là viết tắt của màu sắc, độ bão hòa và độ sáng.
- hsl ( màu sắc , độ bão hòa , độ sáng )
- Hue là một độ trên bánh xe màu từ 0 đến 360. 0 là màu đỏ, 120 là xanh lục và 240 là xanh lam.
- Độ bão hòa là giá trị phần trăm, 0% có nghĩa là màu xám và 100% là màu đầy đủ.
- Độ sáng cũng là một tỷ lệ phần trăm, 0% là màu đen, 50% là không sáng hoặc tối, 100% là màu trắng
#  HSLA 
- Giá trị màu HSLA là phần mở rộng của các giá trị màu HSL với kênh alpha - chỉ định độ mờ cho một màu.
- hsla ( màu sắc, độ bão hòa , độ đậm nhạt , alpha )
# ***CSS Backgrounds***
- Thuộc tính nền CSS được sử dụng để thêm hiệu ứng nền cho các phần tử.
# Opacity / Transparency (độ trong suốt)
- Thuộc opacitytính chỉ định độ mờ / trong suốt của một phần tử. Nó có thể nhận giá trị từ 0,0 - 1,0. Giá trị càng thấp, càng minh bạch:

- **`Lưu ý`**: Khi sử dụng thuộc opacity tính để thêm độ trong suốt vào nền của một phần tử, tất cả các phần tử con của nó sẽ kế thừa cùng một độ trong suốt. Điều này có thể làm cho văn bản bên trong một phần tử hoàn toàn trong suốt khó đọc.
- Độ trong suốt sử dụng RGBA
    - Nếu bạn không muốn áp dụng độ mờ cho các phần tử con, như trong ví dụ của chúng tôi ở trên, hãy sử dụng các giá trị màu RGBA . Ví dụ sau đặt độ mờ cho màu nền chứ không phải cho văn bản:
# CSS Background Image
- Thuộc `background-iage` tính chỉ định một hình ảnh để sử dụng làm nền của một phần tử.

                   background-image: url("bgdesert.jpg");
# Background Image Repeat (tính lặp của ảnh)
- Theo mặc định, thuộc background-image tính lặp lại một hình ảnh theo cả chiều ngang và chiều dọc.

               - background-repeat: repeat-x; (hình nền lập theo chiều ngang)
               - background-repeat: repeat-y; (hình nền lập theo chiều dọc)
               -  background-repeat: no-repeat; (bỏ thuộc tính lặp của ảnh)

- vị trí nền:

            - background-position: right top; (nền ở vị trí góc trên bên phải)

# Background Attachment (tệp đính kèm nền)
- Thuộc `background-attachment` tính chỉ định xem hình nền nên cuộn hay được sửa (sẽ không cuộn với phần còn lại của trang):
- các giá trị của `background-attachment`

    - `scroll`: 

        - Hình nền sẽ bị cuốn đi khi ta kéo thanh scroll(chỉ khi hình nền được thiết lập cho phần tử body)
        - Hình nền sẽ nằm ở một vị trí nhất đinh mặc cho ta có kéo thanh scroll(Hình nền sẽ nằm ở một vị trí nhất đinh mặc cho ta có kéo thanh scroll)
    - `local` :
             Hình nền sẽ bị cuốn đi khi ta kéo thanh scroll(khi hình nền được thiết lập cho bất kỳ một phần tử nào)
    - `fixed` :
        - Hình nền sẽ nằm ở một vị trí nhất đinh mặc cho ta có kéo thanh scroll
            - `lưu ý:` Đối với giá trị này, cho dù hình nền được thiết lập trong phần tử nào thì hình nền vẫn luôn được hiển thị ở vị trí "góc phía trên bên trái" của phần tử body. Nhưng bạn có thể sử dụng thuộc tính background-position để thiết lập lại vị trí cho nó.
        - Tuy nhiên, nếu hình nền được thiết lập cho phần tử nằm bên trong phần tử body thì khi hiển thị một số phần của nó có thể sẽ bị ẩn đi vì những phần tử khác đè lên.
    - `initial` : Sử dụng giá trị mặc định của nó.
        -  Lưu ý: Thuộc tính background-attachment của một phần tử sẽ có giá trị mặc định là scroll.
    - `inherit` : Kế thừa giá trị thuộc tính background-attachment từ phần tử cha của nó.
# Background Shorthand(cách viết gộp các giá trị của backgournd)
         background: #ffffff url("img_tree.png") no-repeat right top;
- background-color (#ffffff)
- background-image (url("img_tree.png"))
- background-repeat (no-repeat)
- background-attachment
- background-position (right top)

`Không quan trọng nếu một trong các giá trị thuộc tính bị thiếu, miễn là các giá trị khác theo thứ tự này. Lưu ý rằng chúng tôi không sử dụng thuộc tính tệp đính kèm nền trong các ví dụ trên, vì nó không có giá trị.`
# ***CSS Borders*** (đường viền css)
- Thuộc tính đường viền CSS cho phép bạn chỉ định kiểu, chiều rộng và màu sắc của đường viền của một phần tử.
- CSS Border Style (kiểu viền)

                border-style

`các giá trị`
 - `dotted ` : đường viền chấm
 - `dashed` :  đường viền đứt nét
 - `solid` : đường viền chắc chắn(nét liền)
 - `double` : đường viền kép
 - `groove` : đường viền có rãnh 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
 - `ridge` : đường viền 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
 - `inset` : đường viền in 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
 - `outset` : đường viền ban đầu 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
 - `none` : Xác định không có đường viền
 - `hidden` : một đường viền ẩn

 `border-style`: có thể có từ một đến bốn giá trị (đối với đường viền trên cùng, đường viền bên phải, đường viền dưới cùng và đường viền bên trái).
# CSS Border Width (chiều rộng viền)
- border-width: chỉ định chiều rộng của bốn đường viền.
- giá trị: `px, pt, cm, em, v.v.` hoặc `thin (mỏng), medium(trung bình), or thick(dày)`
# CSS Border Color
- `border-color`: được sử dụng để đặt màu của bốn đường viền.
- giá trị : `tên, HEX , RGB, HSL`
# CSS Border Sides(các mặt biên giới)
- `border-top-style: solid;`
- `border-right-style:`
- `border-bottom-style:`
- `border-left-style:`
# CSS Shorthand Border Property(viết gộp các thuộc tính của border)
             border: 5px solid red;
- viết gộp 3 thuộc tính sau:
    - `border-width`
    - `border-style`: (k đc để trống)
    - `border-color`
# CSS Rounded Borders(bo viền tròn)
            border-radius: 5px;
# ***CSS Margins***(lề css)
- `lưu ý`: margin không làm tăng kishc thước của phần tử
- `margin` : được sử dụng để tạo không gian xung quanh các phần tử, bên ngoài bất kỳ đường viền xác định nào.
- Có các thuộc tính để đặt lề cho mỗi bên của một phần tử (trên cùng, bên phải, dưới cùng và bên trái).
    - `margin-top`
    - `margin-right`
    - `margin-bottom`
    - `margin-left`
- các giá trị thuộc tính:
    - `auto`: trình duyệt tính toán lợi nhuận
    -  `length`: chỉ định lề bằng px, pt, cm, v.v.
    - ` %` : chỉ định lề tính bằng% chiều rộng của phần tử chứa
    - `inherit` : Chỉ định rằng lề phải được kế thừa từ phần tử cha


             margin: 25px 50px 75px 100px; (trên, phải, dưới, trái)

             margin: 25px 50px 75px; (top= 25px, left,right = 50px, bottom=75px)
# CSS Margin Collapse(Thu gọn lề)
- Đôi khi hai lề thu gọn lại thành một lề duy nhất.
- Đôi khi hai lề thu gọn lại thành một lề duy nhất.
- Đôi khi hai lề thu gọn lại thành một lề duy nhất.

            margin: 0 0 50px 0;(lề trên)
            margin: 20px 0 0 0;(lề dưới)
# ***CSS Padding***(đệm css)
- `padding` : được sử dụng để tạo không gian xung quanh nội dung của phần tử, bên trong bất kỳ đường viền xác định nào.
- Với CSS, bạn có toàn quyền kiểm soát phần đệm. Có các thuộc tính để thiết lập phần đệm cho mỗi bên của một phần tử (trên cùng, bên phải, dưới cùng và bên trái).
    - `padding-top` : 
    - `padding-right`: 
    - `padding-bottom`: 
    - `padding-left`: 
- Tất cả các thuộc tính padding có thể có các giá trị sau:
    - `length` - chỉ định một khoảng đệm bằng px, pt, cm, v.v.
    - `%` - chỉ định một khoảng đệm tính bằng% chiều rộng của phần tử chứa
    - `inherit` - chỉ định rằng phần đệm phải được kế thừa từ phần tử mẹ

- `lưu ý`: padding làm tăng kích thước của phần tử

        - box-sizing: border-box; (thuộc tính này sẽ làm kishc thước phần tử không tăng lên khi padding hay border mà nó sẽ tự co kích thước của content lại sao cho phù hợp)
# ***CSS Height, Width and Max-width***(chiều cao, chiều rộng, chiều rộng tối đa của phần tử)
- `height và width` : thuộc tính được sử dụng để đặt chiều cao và chiều rộng của một phần tử.
- `max-width` : được sử dụng để đặt chiều rộng tối đa của một phần tử.
- Các thuộc tính chiều cao và chiều rộng không bao gồm phần đệm, đường viền hoặc lề. Nó đặt chiều cao / chiều rộng của vùng bên trong phần đệm, đường viền và lề của phần tử.
- Các thuộc tính heightvà widthcó thể có các giá trị sau:
    - `auto `- Đây là mặc định. Trình duyệt tính toán chiều cao và chiều rộng
    - `length `- Xác định chiều cao / chiều rộng bằng px, cm, v.v.
    - `% `- Xác định chiều cao / chiều rộng theo phần trăm của khối chứa
    - `initial `- Đặt chiều cao / chiều rộng thành giá trị mặc định của nó
    - `inherit `- Chiều cao / chiều rộng sẽ được kế thừa từ giá trị mẹ của nó
- `max-width`: như px, cm, v.v., hoặc phần trăm (%) của khối chứa hoặc đặt thành không (đây là mặc định. Có nghĩa là không có chiều rộng tối đa).
# ***CSS Box Model***(mô hình hộp)
- Tất cả các phần tử HTML có thể được coi là hộp.
- trong css, thuật ngữ `box model` được sử dụng khi nói về thiết kế và bố cục.
- Mô hình hộp CSS về cơ bản là một hộp bao bọc xung quanh mọi phần tử HTML. Nó bao gồm: lề, đường viền, phần đệm và nội dung thực tế. Hình ảnh dưới đây minh họa mô hình hộp:

- các thành phần
    - `margin : ` Nội dung của hộp, nơi văn bản và hình ảnh xuất hiện
    - `padding:` Xóa một khu vực xung quanh nội dung. Lớp đệm trong suốt
    - `border:` Đường viền bao quanh phần đệm và nội dung
    - `content` Xóa một khu vực bên ngoài biên giới. Lợi nhuận là minh bạch
- Mô hình hộp cho phép chúng ta thêm đường viền xung quanh các phần tử và xác định không gian giữa các phần tử. 
- `Quan trọng`: Khi bạn đặt thuộc tính chiều rộng và chiều cao của một phần tử bằng CSS, bạn chỉ cần đặt chiều rộng và chiều cao của vùng nội dung . Để tính toán kích thước đầy đủ của một phần tử, bạn cũng phải thêm phần đệm, đường viền và lề.
# ***CSS Outline***(đề cương css)
- Đường viền là một đường được vẽ xung quanh các phần tử, BÊN NGOÀI các đường viền, để làm cho phần tử "nổi bật"
- CSS có các thuộc tính phác thảo sau:
    - `outline-style`: kiểu dáng cho đường đường viền
    - `outline-color`: được sử dụng để đặt màu của đường viền.
    - `outline-width`: chiều rộng cho đường viền
    - `outline-offset`: 
    - `outline`:  viết gộp của (outline-width, outline-style,outline-color)
- `Lưu ý:` outline khác với border ! Không giống như border,outline được vẽ bên ngoài border của phần tử và có thể chồng lên nội dung khác. Ngoài ra, đường viền KHÔNG phải là một phần của các kích thước của phần tử; tổng chiều rộng và chiều cao của phần tử không bị ảnh hưởng bởi chiều rộng của outline.
# outline-style
- các giá trị của `outline-style` : 
    - `dotted ` : đường viền chấm
    - `dashed` :  đường viền đứt nét
    - `solid` : đường viền chắc chắn(nét liền)
    - `double` : đường viền kép
    - `groove` : đường viền có rãnh 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
    - `ridge` : đường viền 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
    - `inset` : đường viền in 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
    - `outset` : đường viền ban đầu 3D. Hiệu ứng phụ thuộc vào giá trị màu viền
    - `none` : Xác định không có đường viền
    - `hidden` : một đường viền ẩn
# outline-width
- `outline-width` : chỉ định chiều rộng của đường viền và có thể có một trong các giá trị sau:
    - `thin` : (mỏng)thường 1px
    - `medium`(bình thường)thường 3px
    - `thick` : (dày)thường 5px
    - `A specific size` : (1 giá trị cụ thể) (in px, pt, cm, em, etc)
# CSS Outline Offset 
- `Outline Offset` : thêm khoảng cách giữa outline và cạnh / border của một phần tử. Khoảng cách giữa một phần tử và đường viền của nó là trong suốt.
# ***CSS Text***
- CSS có rất nhiều thuộc tính để định dạng văn bản.
# text color
- `color` : sử dụng để đặ màu cho văn bản
- `background-color` : sử dụng để đặt màu nền cho văn bảng
- `Quan trọng:` Độ tương phản cao rất quan trọng đối với những người có vấn đề về thị lực. Vì vậy, hãy luôn đảm bảo rằng độ tương phản giữa màu văn bản và màu nền (hoặc ảnh nền) là tốt!
# CSS Text Alignment (căn chỉnh văn bản)
- `text-align` : được sử dụng để đặt căn lề ngang của văn bản.`(left, right, center)`

    - `text-align: justify;` : Sắp xếp nội dung cho các dòng có chiều rộng bằng nhau, điều này có nghĩa là trình duyệt sẽ tự động canh đều các dòng nội dung sao cho tất cả các dòng nội dung đều có cùng chiều rộng.

- `text-align-last` : chỉ định cách căn chỉnh dòng cuối cùng của văn bản.
    - các giá trị : `left, right, center, justify`
- `direction` :  được sử dụng để thay đổi hướng văn bản của một phần tử: 
    - các giá trị: 
        - `ltr` : Hướng văn bản từ trái sang phải, đây là mặc định của direction
        - `rtl` : Hướng văn bản từ phải sang trái.
        - `inherit` : Xác định thừa hưởng thuộc tính từ thành phần cha (thành phần bao ngoài).
- `unicode-bidi` :  được sử dụng để thay đổi hướng văn bản của một phần tử: ngược lại với `direction`
- `vertical-align` :  thiết lập căn chỉnh theo chiều dọc của một phần tử.
# CSS Text Decoration (đường Trang trí văn bản CSS)
- `text-decoration-line` : được sử dụng để thêm dòng trang trí vào văn bản.
    - các giá trị: 
        - `overline` : gạch trên
        - `line-through` : gạch ngang
        - `underline` : gạch dưới
- `Mẹo`: Bạn có thể kết hợp nhiều giá trị, như gạch ngang và gạch dưới để hiển thị cả dòng trên và dưới văn bản.

         text-decoration-line: overline underline line-through;

- `Lưu ý`: Không nên gạch dưới văn bản không phải là liên kết, vì điều này thường gây nhầm lẫn cho người đọc.
- `text-decoration-color` :  được sử dụng để thiết lập màu sắc của đường trang trí.
- `text-decoration-style` : được sử dụng để thiết lập phong cách của đường trang trí.
- `text-decoration-thickness` : được sử dụng để thiết lập độ dày của đường trang trí.
- `text-decoration` : viết tắt cho 
    - `text-decoration-line`(cần thiết)
    - `text-decoration-color`(không bắt buộc)
    - `text-decoration-style`(không bắt buộc)
    - `text-decoration-thickness`(không bắt buộc)
- `text-decoration: none;` : bỏ dấu gạch dấu gạch dưới cho đg link
# CSS Text Transformation 
- được sử dụng để chỉ định chữ hoa và chữ thường trong văn bản.
- `text-transform: uppercase;` : viết chữ hoa
- `text-transform: lowercase;` : viết chữ thường
- `text-transform: capitalize;` :  viết hoa chữ đầu tiên
# CSS Text Spacing (Khoảng cách văn bản CSS) 
- `text-indent:50px;` : được sử dụng để chỉ định thụt lề của dòng đầu tiên của văn bản:
- `letter-spacing: 5px;` : được sử dụng để chỉ định khoảng cách giữa các ký tự trong văn bản.
- `line-height: 0.8;` : được sử dụng để chỉ định khoảng cách giữa các dòng:
- `word-spacing: 10px;` : được sử dụng để chỉ định khoảng cách giữa các dòng:
- `white-space: nowrap;` :  chỉ định cách xử lý khoảng trắng bên trong một phần tử. ![](https://user-images.githubusercontent.com/89244324/164417879-98fb3f98-3cd1-4ea4-883c-606e8b3183cd.png)
# CSS Text Shadow (hiệu ứng bóng chữ)
- `text-shadow`: thêm bóng vào văn bản.

        text-shadow: 2px 2px 5px red;
          (2px bóng ngang, bóng dọc 2px, hiệu ứng mờ vào bóng 5px)
# ***CSS Fonts***
- Việc chọn đúng phông chữ có tác động rất lớn đến cách người đọc trải nghiệm trang web.
- Phông chữ phù hợp có thể tạo ra một bản sắc mạnh mẽ cho thương hiệu của bạn.
- Sử dụng phông chữ dễ đọc là điều quan trọng. Phông chữ làm tăng giá trị cho văn bản của bạn. Điều quan trọng nữa là chọn màu và kích thước văn bản chính xác cho phông chữ.

    - `Phông chữ Serif` có một nét nhỏ ở các cạnh của mỗi chữ cái. Chúng tạo ra một cảm giác trang trọng và sang trọng.
    - `Phông chữ Sans-serif` có đường nét rõ ràng (không kèm theo các nét nhỏ).Chúng tạo ra một cái nhìn hiện đại và tối giản.
    - `Phông chữ Monospace` - ở đây tất cả các chữ cái có cùng chiều rộng cố định. Chúng tạo ra một cái nhìn máy móc. 
    - `Cursive` chữ viết tay bắt chước chữ viết tay của con người.
    - `Fantasy` là phông chữ trang trí / vui tươi.
- `Lưu ý:` Trên màn hình máy tính, phông chữ sans-serif được coi là dễ đọc hơn phông chữ serif.
![](https://user-images.githubusercontent.com/89244324/164427650-a784fe0b-0853-491d-ae11-994f6c185789.png)
- `font-family:` để chỉ định phông chữ của văn bản.

      - font-family: "Times New Roman", Times, serif; 
        (phông chữ dự phòng, khi trang web k hỗ trợ, Luôn kết thúc danh sách bằng họ phông chữ chung. )
- `Lưu ý `: Nếu tên phông chữ có nhiều hơn một từ, nó phải nằm trong dấu ngoặc kép, như: "Times New Roman".
# CSS Web Safe Fonts
- Phông chữ an toàn Web CSS
![](https://user-images.githubusercontent.com/89244324/164430237-57437e40-c31b-440e-9fa2-3e30d235223a.png)
- `Arial (sans-serif):` 
    - Arial là phông chữ được sử dụng rộng rãi nhất cho cả phương tiện truyền thông trực tuyến và in ấn. Arial cũng là phông chữ mặc định trong Google Tài liệu.
    - Arial là một trong những phông chữ web an toàn nhất và nó có sẵn trên tất cả các hệ điều hành chính.
- `Verdana (sans-serif)`: Verdana là một phông chữ rất phổ biến. Verdana có thể dễ dàng đọc được ngay cả đối với kích thước phông chữ nhỏ.
- `Helvetica (sans-serif)`: Phông chữ Helvetica được các nhà thiết kế yêu thích. Nó phù hợp với nhiều loại hình kinh doanh.
# CSS Font Style
- `font-style` : chủ yếu được sử dụng để chỉ định văn bản in nghiêng.
    - `normal` - Văn bản được hiển thị bình thường
    - `italic` - Văn bản được in nghiêng
    - `oblique` -  Văn bản là "nghiêng" (xiên rất giống với in nghiêng, nhưng ít được hỗ trợ hơn)
- `font-weight` - Độ đậm phông chữ
    - `normal` : giá trị mặc định, tương đương với khi xác định là 400.
    - `lighter`: các chữ cái trong phần tử cha sẽ đậm hơn các chữ cái trong phần tử này
    - `bold`: giá trị tương đương với khi xác định là 700.
- `font-variant: small-caps`: tất cả các chữ cái thường được chuyển đổi thành chữ hoa. Tuy nhiên, các chữ hoa đã chuyển đổi sẽ xuất hiện ở kích thước phông chữ nhỏ hơn các chữ hoa gốc trong văn bản.
    - chỉ định xem một văn bản có nên được hiển thị bằng phông chữ in hoa nhỏ hay không.
# CSS Font Size
- `font-size` : Đặt kích thước của văn bản
- Giá trị kích thước phông chữ có thể là kích thước tuyệt đối hoặc tương đối.
    ![](https://user-images.githubusercontent.com/89244324/164618138-65a8d591-4a78-4120-b67f-4794c7a25c90.png)
- Đặt kích thước phông chữ với điểm ảnh
- Đặt kích thước phông chữ bằng Em
    - 1em =16px
- Sử dụng kết hợp Phần trăm và Em
- Kích thước phông chữ đáp ứng (vw)
    - 1vw = 1% chiều rộng khung hình
# CSS Google Fonts
- Nếu bạn không muốn sử dụng bất kỳ phông chữ tiêu chuẩn nào trong HTML, bạn có thể sử dụng Google Fonts.
- Google Fonts được sử dụng miễn phí và có hơn 1000 phông chữ để bạn lựa chọn.
- Cách sử dụng Phông chữ của Google

    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
- `Lưu ý`: Khi chỉ định một phông chữ trong CSS, hãy luôn liệt kê ít nhất một phông chữ dự phòng (để tránh các hành vi không mong muốn). Vì vậy, cũng ở đây, bạn nên thêm một họ phông chữ chung (như serif hoặc sans-serif) vào cuối danh sách.

    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">

- `Lưu ý`: Yêu cầu nhiều phông chữ có thể làm chậm các trang web của bạn! Vì vậy, hãy cẩn thận về điều đó.
# CSS Great Font Pairings
![](https://user-images.githubusercontent.com/89244324/164621932-619149d5-d760-4dd7-9ec3-626994459b48.png)
- một số cặp phông chữ phổ biến sẽ phù hợp với nhiều thương hiệu và ngữ cảnh.
    - Georgia và Verdana
    - Helvetica và Garamond
- Các cặp phông chữ phổ biến của Google
    - Merriweather và Open Sans
    - Ubuntu và Lora
    - Abril Fatface và Poppins
    - Cinzel và Fauna One
# CSS Font Property
- Để rút ngắn mã, cũng có thể chỉ định tất cả các thuộc tính phông chữ riêng lẻ trong một thuộc tính.
![](https://user-images.githubusercontent.com/89244324/164623204-d6a27ea5-c9d0-499f-9787-e9174d67c0ba.png)
# ***CSS Icons***
- Các biểu tượng có thể dễ dàng được thêm vào trang HTML của bạn bằng cách sử dụng thư viện biểu tượng.
- Các biểu tượng của Google
# ***CSS Links***
- Với CSS, các liên kết có thể được tạo kiểu theo nhiều cách khác nhau.
# Styling Links
- ![](https://user-images.githubusercontent.com/89244324/164628257-6d8c749c-908b-475c-b746-da8c2147e0f2.png)
- Khi đặt kiểu cho một số trạng thái liên kết, có một số quy tắc đặt hàng:
    - a:hover cần phải đến sau a:link and a:visited
    - a:active cần phải đến sau a:hover
- `Text Decoration`:  chủ yếu được sử dụng để xóa gạch chân khỏi các liên kết:
- Màu nền
- Các nút liên kết
# ***CSS Lists***
# Different List Item Markers (Các điểm đánh dấu mục trong danh sách khác nhau)
- `list-style-type` :  chỉ định loại điểm đánh dấu mục danh sách
- 1 số giá trị: 
    - `circle` : hình tròn
    - `square` hình vuông
    - `upper-roman` : số la mã
    - `lower-alpha` : chữ thường;
- `list-style-image` : chỉ định một hình ảnh làm điểm đánh dấu mục danh sách:
- `list-style-position`: chỉ định vị trí của các điểm đánh dấu mục danh sách (dấu đầu dòng).
- `list-style-position: external;` : các dấu đầu dòng sẽ nằm ngoài mục danh sách. Đầu mỗi dòng của một mục danh sách sẽ được căn chỉnh theo chiều dọc. Đây là mặc định:
- `list-style-position: inside;` : các dấu đầu dòng sẽ nằm bên trong mục danh sách. Vì nó là một phần của mục danh sách, nó sẽ là một phần của văn bản và đẩy văn bản vào đầu:
- Xóa cài đặt mặc định: 
    - `list-style-type:none` :  này cũng có thể được sử dụng để loại bỏ các điểm đánh dấu / dấu đầu dòng.
    - `Lưu ý` rằng danh sách cũng có lề và phần đệm mặc định. Để xóa phần này, hãy thêm margin:0và padding:0vào ul hoặc ol: 
- `list-style`:   list-style: square inside url("sqpurple.gif");

 ![](https://user-images.githubusercontent.com/89244324/164649953-61aad507-178f-4110-a07c-ec8068a05ea0.png)
 # ***CSS Tables***
- Giao diện của một bảng HTML có thể được cải thiện đáng kể với CSS:
- Đường viền bảng
- Bảng toàn chiều rộng: `width: 100%;`
- Đường viền đôi
Lưu ý rằng bảng trong các ví dụ trên có hai đường viền. Điều này là do cả bảng và các phần tử th và td đều có đường viền riêng biệt.
- Thu gọn đường viền bảng:  `border-collapse: collapse;`
# CSS Table Size
- `width` : chiều rộng bảng
- `height` : chiều cao bảng
# CSS Table Alignment (liên kết bảng)
- Căn chỉnh theo chiều dọc
    - `vertical-align` :  đặt căn chỉnh theo chiều dọc (như trên cùng, dưới cùng hoặc giữa) của nội dung trong th hoặc td.
# CSS Table Style
- `Table Padding` (bảng đệm): padding
- `Horizontal Dividers`:  (bộ chia ngang) : border-bottom: 1px solid
- `Hoverable Table`: (Bảng lưu trữ): dùng `hover` cho `tr`
- `Striped Tables`: (bảng sọc) : `nth-child()`
- `Table Color` : (màu bảng)
# CSS Responsive Table
- Bảng đáp ứng sẽ hiển thị thanh cuộn ngang nếu màn hình quá nhỏ để hiển thị toàn bộ nội dung:
- Thêm một phần tử vùng chứa (như `div`) với `overflow-x:autoxung` quanh phần tử `table` để làm cho nó đáp ứng:
- `Lưu ý:` Trong OS X Lion (trên Mac), thanh cuộn được ẩn theo mặc định và chỉ hiển thị khi được sử dụng (ngay cả khi "tràn: cuộn" được đặt).
# ***CSS Layout - The display Property***CSS
- `display`: là thuộc tính CSS quan trọng nhất để kiểm soát bố cục.
# The display Property
- `display` : chỉ định nếu / cách một phần tử được hiển thị
- Mọi phần tử HTML đều có giá trị hiển thị mặc định tùy thuộc vào loại phần tử đó. Giá trị hiển thị mặc định cho hầu hết các phần tử là blockhoặc inline.
- `Block-level Elements`(phần tử cấp khối): 
    - div
    - h1 - h6
    - p
    - form
    - header
    - footersection...v.v
- `Inline Elements`(phần tử nội tuyến)
    - span
    - a
    - img
- `Display: none;` thường được sử dụng với JavaScript để ẩn và hiển thị các phần tử mà không cần xóa và tạo lại chúng
    -  `script` : dùng `display: none` làm mặc định
- `Override The Default Display Value` Ghi đè Giá trị Hiển thị Mặc định
    - Như đã đề cập, mọi phần tử đều có giá trị hiển thị mặc định. Tuy nhiên, bạn có thể ghi đè điều này.
    - Thay đổi phần tử nội tuyến thành phần tử khối hoặc ngược lại

- `Lưu ý`: Việc đặt thuộc tính hiển thị của một phần tử chỉ thay đổi cách phần tử được hiển thị , KHÔNG phải loại phần tử đó là gì. Vì vậy, một phần tử nội tuyến với display: block;không được phép có các phần tử khối khác bên trong nó.
- `Hide an Element(ẩn 1 phần tử)` - `display:none` hoặc `visibility:hidden`?
    - Việc ẩn một phần tử có thể được thực hiện bằng cách đặt thuộc `display`tính thành `none`. Phần tử sẽ bị ẩn và trang sẽ được hiển thị như thể phần tử không có ở đó:
    - `visibility:hidden`: cũng ẩn 1 ptu, Tuy nhiên, phần tử sẽ vẫn chiếm dung lượng như trước. Phần tử sẽ bị ẩn, nhưng vẫn ảnh hưởng đến bố cục
# ***CSS Layout - width and max-width***
# ***CSS Layout - The position Property***(thuộc tính vị trí)
- `position` : chỉ định loại phương pháp định vị được sử dụng cho một phần tử (tĩnh, tương đối, cố định, tuyệt đối hoặc cố định).
- có 5 giá trị:
    - `static` : 
    - `relative` : 
    - `fixed` : 
    - `absolute` : 
    - `sticky` : 
- Sau đó, các phần tử được định vị bằng cách sử dụng các thuộc tính trên cùng, dưới cùng, trái và phải. Tuy nhiên, các thuộc tính này sẽ không hoạt động trừ khi thuộc position tính được đặt trước. Chúng cũng hoạt động khác nhau tùy thuộc vào giá trị vị trí.
- `position: static;`: được định vị theo bất kỳ cách đặc biệt nào; nó luôn được định vị theo dòng bình thường của trang
- `position: relative;`(liên quan đến): vị trí tương đối, k bị phụ thuộc vào thg nào. lấy chính nó làm gốc tọa độ. 
    - có thể di chuyển 4 hướng. và đè lên các phần tử khác.
- `position: absolute`: vị trí tuyệt đối. lấy thẻ cha gần nhất có thuộc tính position làm gốc tạo độ,
- `position: fixed` : được định vị so với chế độ xem, có nghĩa là nó luôn ở cùng một vị trí ngay cả khi trang được cuộn. Các thuộc tính trên cùng, phải, dưới cùng và bên trái được sử dụng để định vị phần tử.
- `position: sticky;` : được định vị dựa trên vị trí cuộn của người dùng. bám dính
# ***CSS Layout - The z-index Property***
- `z-index`:thiết lập thứ tự xếp chồng nhau của một thành phần vị trí.
- Thứ tự chồng nhau được sắp xếp dựa theo giá trị số, thành phần HTML nào có chỉ số z-index cao hơn sẽ nằm trên, ngược lại sẽ nằm dưới, giá trị mặc định là 0..
- Một phần tử có thể có thứ tự ngăn xếp dương hoặc âm:
![](https://user-images.githubusercontent.com/89244324/165020061-1362270a-8b4a-43be-a5e7-bc71fa0f3d7d.png
)
# ***CSS Layout - Overflow***
- `overflow`: kiểm soát những gì xảy ra với nội dung quá lớn để vừa với một khu vực.
# CSS Overflow
-  `overflow`: chỉ định cắt nội dung hoặc thêm thanh cuộn khi nội dung của một phần tử quá lớn để vừa với khu vực được c(hỉ định
![](https://user-images.githubusercontent.com/89244324/165021395-7d4de7c4-47f6-4118-84d1-696626977502.png)

# ***CSS Layout - float and clear***
- `float` :sử dụng để chuyển một phần tử sang góc trái hoặc phải của không gian bao quanh nó, rất cần thiết trong việc định dạng bố cục trang.
![](https://user-images.githubusercontent.com/89244324/165021872-78ff7112-7e78-4e86-ae97-c825771f6ea1.png)
- `clear` : gần như là ngược lại với float. Thuộc tính Clear ngăn chặn thành phần A chiếm vùng không gian của thành phần B (với thành phần B là thành phần sử dụng float). Đôi khi không muốn float ở một số tình huống nào đó ta sẽ dùng clear để khắc chế.
![](https://user-images.githubusercontent.com/89244324/165022201-36e2bdfd-5f7e-4a15-ae1b-4f15973cfc3d.png)
- `The clearfix Hack`: 
# ***CSS Layout - display: inline-block***
- So với `display: inline`, sự khác biệt chính là `display: inline-block`cho phép thiết lập chiều rộng và chiều cao trên phần tử.
- Ngoài ra, với display: `inline-block`, lề / đệm trên cùng và dưới cùng được tôn trọng, nhưng với `display: inline`chúng thì không.
- So với `display: block`, sự khác biệt chính là `display: inline-block`không thêm dấu ngắt dòng sau phần tử, vì vậy phần tử có thể nằm cạnh các phần tử khác.
# ***CSS Layout - Horizontal & Vertical Align***
# Các yếu tố căn giữa
- Các yếu tố căn giữa: Để căn giữa theo chiều ngang một phần tử khối (như div), hãy sử dụng `margin: auto;`
- `Lưu ý`: Căn giữa không có hiệu lực nếu thuộc `width` tính không được đặt (hoặc được đặt thành 100%).
# Căn giữa Văn bản
- `text-align: center`
# Căn giữa một hình ảnh
- Để căn giữa một hình ảnh, hãy đặt lề trái và phải `auto`và biến nó thành một `block` phần tử:
# Căn trái và Phải - Sử dụng vị trí
- Một phương pháp để căn chỉnh các phần tử là sử dụng `position: absolute;`: 
- `Lưu ý`: Các phần tử có vị trí tuyệt đối bị xóa khỏi luồng thông thường và có thể chồng chéo các phần tử.
# Căn trái và Phải - Sử dụng float
- Một phương pháp khác để căn chỉnh các phần tử là sử dụng thuộc `float` tính:
# Bản hack clearfix
# Căn giữa theo chiều dọc - Sử dụng đệm
- Có nhiều cách để căn giữa một phần tử theo chiều dọc trong CSS. Một giải pháp đơn giản là sử dụng `top` và `bottom padding`:
# Căn giữa theo chiều dọc - Sử dụng đệm
- Để căn giữa theo cả chiều dọc và chiều ngang, hãy sử dụng `padding` và `text-align: center`:
# Căn giữa theo chiều dọc - Sử dụng chiều cao dòng
# Căn giữa theo chiều dọc - Sử dụng vị trí và chuyển đổi
- Nếu `padding`và `line-height` không phải là các tùy chọn, một giải pháp khác là sử dụng định vị và thuộc `transform` tính:
# Căn giữa theo chiều dọc - Sử dụng Flexbox
# ***CSS Combinators***
- Bộ tổ hợp là thứ giải thích mối quan hệ giữa các bộ chọn
![](https://user-images.githubusercontent.com/89244324/165050826-45c011f9-c239-4d90-80b0-1a443694ad1b.png)
- Descendant Selector: Bộ chọn hậu duệ khớp với tất cả các phần tử là con của một phần tử được chỉ định.
- Bộ chọn con (>): Bộ chọn con chọn tất cả các phần tử là con của một phần tử được chỉ định.
- Bộ chọn Anh chị em kế cận (+): Bộ chọn anh chị em kế cận được sử dụng để chọn một phần tử nằm ngay sau một phần tử cụ thể khác.
    - Các phần tử anh chị em phải có cùng một phần tử mẹ và "liền kề" có nghĩa là "ngay sau đó".
- Bộ chọn anh chị em chung (~): Bộ chọn anh chị em chung chọn tất cả các phần tử là anh chị em tiếp theo của một phần tử được chỉ định.
# ***CSS Pseudo-classes***
- Một lớp giả được sử dụng để xác định trạng thái đặc biệt của một phần tử.
![](https://user-images.githubusercontent.com/89244324/165055056-319975ad-a8c5-427e-87b8-1e1b914ddc1e.png)
- `:link` : Hiển thị hiệu ứng khác biệt để người đọc biết đây là đường liên kết
- `:visited` :Đường link đã từng được click vào
- `:hover` : khi di chuyển chuột qua sẽ có hiệu ưng chuyển màu
- `:active` : Đường link đang được nhấp chuột vào
- `:first-child` :  khớp với một phần tử được chỉ định là phần tử con đầu tiên của phần tử khác.
- `:last-child` : lấy đứa con cuối cùng
- `:lang` : cho phép bạn xác định các quy tắc đặc biệt cho các ngôn ngữ khác nhau.
# ***CSS Pseudo-elements***(phần tử giả)
- `::before` :thường được sử dụng để thêm text, hình ảnh hay bất kỳ nội dung gì phía trước nội dung của phần tử được chọn.
- `::after`:cũng được sử dụng để thêm nội dung nhưng là vào phía sau phần tử được chọn.
- `::fist-letter`:được sử dụng để thêmstyle đặc biệt vào chữ cái đầu tiên của văn bản.
- `::fist-line`:dùng để style cho dòng đầu tiên của phần tử được chọn
- `::selection`::dùng để style cho dòng đầu tiên của phần tử được chọn
- `::marker`: họn các điểm đánh dấu của các mục danh sách.
# ***CSS Opacity / Transparency***(độ mờ, dộ trong suốt của css)
- `opacity`: chỉ định độ mờ / trong suốt của một phần tử. có thể nhận giá trị từ 0,0 - 1,0. Giá trị càng thấp, càng minh bạch:

# Hiệu ứng Di chuột trong suốt
- Thuộc `opacity` tính thường được sử dụng cùng với `:hover` bộ chọn để thay đổi độ mờ khi di chuột qua:
# Hộp trong suốt
- Khi sử dụng thuộc opacitytính để thêm độ trong suốt vào nền của một phần tử, tất cả các phần tử con của nó sẽ kế thừa cùng một độ trong suốt. Điều này có thể làm cho văn bản bên trong một phần tử hoàn toàn trong suốt khó đọc:
# Độ trong suốt sử dụng RGBA
- Nếu bạn không muốn áp dụng độ mờ cho các phần tử con, như trong ví dụ của chúng tôi ở trên, hãy sử dụng các giá trị màu RGBA
# ***CSS Navigation Bar***
- Thanh điều hướng
- Thanh điều hướng = Danh sách các liên kết
- CSS Vertical Navigation Bar
# ***CSS Dropdowns***(Trình đơn thả xuống)
# ***Hình ảnh CSS Sprites***
# ***CSS Attribute Selectors*** 
- Có thể tạo kiểu cho các phần tử HTML có các thuộc tính hoặc giá trị thuộc tính cụ thể.
- Bộ chọn [thuộc tính] CSS
- Bộ chọn CSS [thuộc tính = "value"]
- Bộ chọn CSS [thuộc tính ~ = "value"] : được sử dụng để chọn các phần tử có giá trị thuộc tính chứa một từ được chỉ định.***
- Bộ chọn CSS [thuộc tính | = "value"]
- Bộ chọn CSS [thuộc tính ^ = "value"]
- Bộ chọn CSS [thuộc tính $ = "value"] 
- Bộ chọn CSS [thuộc tính * = "value"]
# ***CSS Forms***
# ***CSS Counters***
- Bộ đếm CSS là "biến" được duy trì bởi CSS mà giá trị của nó có thể được tăng lên bởi các quy tắc CSS (để theo dõi số lần chúng được sử dụng). Bộ đếm cho phép bạn điều chỉnh hình thức của nội dung dựa
![](https://user-images.githubusercontent.com/89244324/165280751-a3c19877-b672-4648-964d-0059d2ae7a4f.png)
# ***CSS Units***
- CSS có một số đơn vị khác nhau để thể hiện độ dài.
- Lưu ý: Khoảng trắng không được xuất hiện giữa số và đơn vị. Tuy nhiên, nếu giá trị là 0, đơn vị có thể được bỏ qua.
- Có hai loại đơn vị độ dài: tuyệt đối và tương đối .
- tuyệt đối
![](https://user-images.githubusercontent.com/89244324/165497899-86fc91c3-9f7e-4614-934a-3fdba945e0be.png)
- tương đối
![](https://user-images.githubusercontent.com/89244324/165498392-7a5c6614-8156-4fc7-80c5-7f833f06302c.png)
# ***Đặc tính CSS***
- `Kiểu nội tuyến - Ví dụ: <h1 style = "color: pink;">`
- `ID - Ví dụ: #navbar`
- `Lớp, lớp giả, bộ chọn thuộc tính - Ví dụ: .test,: hover, [href]`
- `Phần tử và phần tử giả - Ví dụ: h1,: before`
- Lưu ý: Kiểu nội tuyến nhận giá trị đặc trưng là 1000 và luôn được ưu tiên cao nhất!
- `Lưu ý 2`: Có một ngoại lệ đối với quy tắc này: nếu bạn sử dụng `!important` quy tắc, nó thậm chí sẽ ghi đè các kiểu nội tuyến!
- Bộ chọn có giá trị độ đặc hiệu cao nhất sẽ thắng và có hiệu lực!
- `Tính cụ thể ngang nhau: quy tắc mới nhất thắng - Nếu cùng một quy tắc được viết hai lần vào biểu định kiểu bên ngoài, thì quy tắc mới nhất sẽ thắng:`
- Bộ chọn ID có độ đặc hiệu cao hơn bộ chọn thuộc tính
- Bộ chọn theo ngữ cảnh cụ thể hơn bộ chọn phần tử đơn lẻ - Biểu định kiểu được nhúng gần với phần tử cần tạo kiểu hơn
- Bộ chọn theo ngữ cảnh cụ thể hơn bộ chọn phần tử đơn lẻ - Biểu định kiểu được nhúng gần với phần tử cần tạo kiểu hơn
- Một bộ chọn lớp đánh bại bất kỳ số lượng bộ chọn phần tử nào
- Một bộ chọn lớp đánh bại bất kỳ số lượng bộ chọn phần tử nào
# ****CSS Advanced***
# **CSS Rounded Corners**
- Với thuộc tính CSS border-radius, bạn có thể đặt bất kỳ phần tử nào là "các góc được làm tròn".
# ***CSS Border Images***            
- `border-image`: cho phép bạn chỉ định một hình ảnh sẽ được sử dụng thay vì đường viền bình thường xung quanh một phần tử.
![](https://user-images.githubusercontent.com/89244324/165668431-5326e9bf-e027-4868-abc8-5603e43cebf4.png)
- Thuộc border-imagetính sẽ lấy hình ảnh và cắt nó thành chín phần, giống như một bảng tic-tac-toe. Sau đó, nó đặt các góc ở các góc, và các phần ở giữa được lặp lại hoặc kéo dài như bạn chỉ định.
- Lưu ý: Để `border-image` hoạt động, phần tử cũng cần có thuộc `border`tính!
![](https://user-images.githubusercontent.com/89244324/165670027-4ea8a137-a7b2-486a-b6a7-dfd1cea835ae.png)
- Lúc này ta chú ý các phần 1, 3, 7, 9 là bốn góc và nó cố định, phần 5 là vị trí trung tâm và những phần còn lại sẽ bị ảnh hưởng bởi các giá trị như round, repeat hoặc stretch bạn chỉ định.
# **CSS Multiple Backgrounds**
- `background-size` : 
- `background-origin` : 
- `background-clip` : 
- Hai giá trị có thể có khác `background-size`là `contain` và `cover`.
- Từ `containkhóa` chia tỷ lệ hình nền càng lớn càng tốt (nhưng cả chiều rộng và chiều cao của hình ảnh phải vừa với vùng nội dung). Như vậy, tùy thuộc vào tỷ lệ của ảnh nền và khu vực định vị nền, có thể có một số vùng nền không bị ảnh nền che phủ.
- Xác định kích thước của nhiều hình nền
    - Thuộc `background-size`tính cũng chấp nhận nhiều giá trị cho kích thước nền (sử dụng danh sách được phân tách bằng dấu phẩy), khi làm việc với nhiều nền.
- Thuộc tính `background-origin` CSS
![](https://user-images.githubusercontent.com/89244324/165673994-7e50830f-6078-4209-af0b-978d60b831b5.png)
- Thuộc tính nền-clip CSS
![](https://user-images.githubusercontent.com/89244324/165674095-88e856a4-631e-4374-a6bd-881c71ccaf58.png)
# ***Màu CSS***
- CSS hỗ trợ hơn 140 tên màu, giá trị HEX, giá trị RGB , giá trị RGBA, giá trị HSL, giá trị HSLA và độ mờ.
- Màu HSL 
![](https://user-images.githubusercontent.com/89244324/165674617-974306bd-7685-4392-8361-cf4ad526cc8f.png)
- Màu HSLA
![](https://user-images.githubusercontent.com/89244324/165674879-2531eb82-7954-480e-812b-a167ff4613ca.png)
# ***CSS Color Keywords***
- Trang này sẽ giải thích `transparent, currentcolorvà inherit`từ khóa.
- `transparent` : được sử dụng để làm cho màu trong suốt. Điều này thường được sử dụng để tạo màu nền trong suốt cho một phần tử.
- Lưu ý: Từ `transparent` khóa tương đương với `rgba (0,0,0,0)`. Giá trị màu RGBA là phần mở rộng của các giá trị màu RGB với kênh alpha - chỉ định độ mờ cho một màu. Đọc thêm trong chương CSS RGB của chúng tôi và trong chương Màu sắc CSS của chúng tôi 
- `currentcolor`: giống như một biến giữ giá trị hiện tại của thuộc tính màu của một phần tử.
    - Từ khóa này có thể hữu ích nếu bạn muốn một màu cụ thể nhất quán trong một phần tử hoặc một trang.
- `inherit`: chỉ định rằng một thuộc tính sẽ kế thừa giá trị của nó từ phần tử mẹ của nó.
    - chỉ định rằng một thuộc tính sẽ kế thừa giá trị của nó từ phần tử mẹ của nó.
# ***CSS Gradients***
- CSS gradient cho phép bạn hiển thị các chuyển đổi mượt mà giữa hai hoặc nhiều màu được chỉ định.
    - Sử dụng Angles :Nếu bạn muốn kiểm soát nhiều hơn hướng của gradient, bạn có thể xác định một góc, thay vì các hướng được xác định trước (xuống dưới, lên trên, sang phải, sang trái, dưới cùng bên phải, v.v.). Giá trị 0deg tương đương với "to top". Giá trị 90deg tương đương với "to right". Giá trị 180deg tương đương với "to bottom".
- `CSS Radial Gradients`: 
- Một gradient xuyên tâm được xác định bởi tâm của nó.
- Tham số kích thước xác định kích thước của gradient. Nó có thể nhận bốn giá trị:
    - closest-side: gần nhất
    - farthest-side: xa nhất
    - closest-corner: góc gần nhất
    - farthest-corner : góc xa nhất
- `CSS Conic Gradients`: Gradient conic là một gradient với các chuyển đổi màu được quay xung quanh một điểm trung tâm
![](https://user-images.githubusercontent.com/89244324/165699933-3a7733a6-839e-4812-82a4-3d1dda2906dc.png)
# ***CSS Shadow Effects***
-  `text-shadow: 2px 2px 5px red;`: (bóng ngang, bóng dọc, hiệu ưng mờ , màu)
- `box-shadow:`: 






