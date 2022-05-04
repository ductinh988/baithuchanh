- **thẻ pre : định dạng giống bài thơ
- **thẻ hr : dòng kẻ ngang
- **thẻ br: xuống dòng
- **text-align : căn chỉnh van bản
## **Formatting: định dạng**
- thẻ b : là in đậm
- thẻ strong : văn bản quan trọng
- thẻ i : là chữ nghiêng 
- thẻ em :  xác định văn bản nhấn mạnh. Nội dung bên trong thường được hiển thị bằng italic.
- thẻ small : thẻ xác định văn bản nhỏ hơn
- thẻ mark :thẻ tô sáng
- thẻ del :thẻ gạch ngang chữ
- thẻ ins : thẻ gạch chân
- thẻ sub : thẻ làm văn bản thấp xuống vd: h2o
- thẻ sup : thẻ làm văn bản kéo lên trên giống x2(x mũ 2)
## **blockquote:Các yếu tố trích dẫn và trích dẫn**
- **blockquote** : xd đc trích dẫn. trình duyệt thg thụt lề.
- thẻ q : xác định 1 trích dẫn ngắn "như vd"
- thẻ abbr : xác định chữ viết tắt hoặc từ viết tắt
-  thẻ address: xác định thông tin liên hệ của tác giả
- thẻ cite : xác định tiêu đề của một tác phẩm sáng tạo vd: cuốn sách,..
- bdo: được sử dụng để ghi đè hướng văn bản hiện tại:
## **color**
   - rgb(red, green, blue) : red, green, blue: có giá trị từ 0-255
        - rgba(red, green, blue, alpha) : alpha là độ mờ có giá trị từ 0-1
   - hex : một màu có thể được chỉ định bằng giá trị thập lục phân ở dạng: vd: # rrggbb, #333, #fffff
   - hsl: hsl ( màu sắc , độ bão hòa , độ sáng ) //vd :hsl (0, 100%, 50%)

## **link**
- a

    - Một liên kết không được truy cập được gạch chân và có màu xanh lam
    - Một liên kết đã truy cập được gạch chân và có màu tím
    - Một liên kết đang hoạt động được gạch chân và có màu đỏ
- Thuộc target tính chỉ định nơi để mở tài liệu được liên kết.
Thuộc target tính có thể có một trong các giá trị sau:
    - _self- Mặc định. Mở tài liệu trong cùng một cửa sổ / tab khi nó được nhấp vào
    - _blank- Mở tài liệu trong một cửa sổ hoặc tab mới
    - _parent- Mở tài liệu trong khung chính

    - _top- Mở tài liệu trong toàn bộ phần thân của cửa sổ
  -  `:link dùng để chọn các liên kết mà đường dẫn của nó chưa được trình duyệt viếng thăm.`
    - `:visited dùng để chọn các liên kết mà đường dẫn của nó đã được trình duyệt viếng thăm.`
    -  `:active dùng để chọn phần tử đang được người dùng nhấp vào.`
- link bookmarks
 - Sử dụng idthuộc tính (id = " value ") để xác định dấu trang trong một trang
- Sử dụng hrefthuộc tính (href = "# value ") để liên kết với dấu trang
- Sử dụng mailto:lược đồ bên trong hrefthuộc tính để tạo liên kết mở chương trình email của người dùng

## **Images**
- img 
- thuộc tính src
- thẻ map: xác định bản đồ hình ảnh (trong map sẽ có thẻ area)
    - thẻ area: Để xác định các khu vực có thể nhấp trong bản đồ hình ảnh
    - Sử dụng thuộc tính HTML USEMAP của phần tử img để trỏ đến bản đồ hình ảnh
        <!-- <picture>
         <source media="(min-width: 650px)" srcset="img_food.jpg">
        <source media="(min-width: 465px)" srcset="img_car.jpg">
        <img src="img_girl.jpg">
         </picture> -->
- Bìa nền : 
    - `background-attachment: fixed;`  //Fixed nghĩa là hình ảnh nền được cố định vào khung nhìn và không di chuyển, ngay cả khi người dùng đang di chuyển dọc theo khung. Local là hình nền nên được cố định vào vị trí của nó trong phần tử.
    -  `background-size: cover;` để đảm bảo toàn bộ phần tử luôn được bao phủ,
- HTML picture Element: 
- thẻ picture :cho phép bạn hiển thị các hình ảnh khác nhau cho các thiết bị hoặc kích thước màn hình khác nhau.
    - thẻ source: mỗi phần tử đề cập đến các hình ảnh khác nhau thông qua srcset thuộc tính
## **table**
<!-- <table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>  -->
 - table :Định nghĩa một bảng
 - tr : xác định 1 hàng trong 1 bảng
 - th : Xác định một tiêu đề trong một bảng
 - td : xác định một ô trong một bảng
 - caption : xác định chú thích bảng
 ### **table borders**
 - để bỏ đưuòng viền kép thành 1 đường viền ta dùng:

             border-collapse: collapse;

  -  border-radius:
    **các giá trị của borders-style:**
        - dotted  : đường viền chấm 
        - dashed    :  đưuòng viền nét đứt
        solid    : nét liền 
        double  : đường viền kép   
        groove  : viền màu xám   
        ridge     
        inset     
        outset     
        none     
        hidden  
- border-color: 
- table size: viết thuộc tính style= height hoặc width vào ô cần chỉnh size  
- table Headers
    - `Align Table Headers`(căn chỉnh tiêu đề): text-align: 
    - `Header for Multiple Columns`(tiêu đề cho nhiều cột): Để làm điều này, hãy sử dụng thuộc tính colspan trên phần tử **th**:

    - `Table Caption`(bảng chú thích): caption
- Table Padding & Spacing(bảng đệm và khoảng cách): 
    - `border-spacing`: Để thay đổi khoảng cách giữa các ô trong bảng, 
-  Colspan & Rowspan: 
    - `colspan` : Để tạo một ô di động trên nhiều cột
    - `Rowspan` : Để tạo một nhịp di động trên nhiều hàng
    - HTML Table Styling (bảng kiểu dáng)
        - `tr:nth-child(even) {
        background-color: #D6EEEE;
        }` //: tạo kiểu vằn vằn
        - even : tạo kiểu vằn hàng 2,4,6,..
        - odd : tạo kiểu vằn hàng 1,3,5,..
- HTML Table - Vertical Zebra Stripes( sọc ngựa vằn dọc):
    - `td:nth-child(even), th:nth-child(even) {
        background-color: #D6EEEE;
        }`   //: tạo kiểu sọc vằng cột dọc
        - `Lưu ý: Đặt :nth-child()bộ chọn trên cả hai thvà td các phần tử nếu bạn muốn có kiểu trên cả tiêu đề và ô bảng thông thường.`
- Combine Vertical and Horizontal Zebra Stripes(tạo kiểu sọc cả ngang và dọc)
    - `tr:nth-child(even) {
         background-color: rgba(150, 212, 212, 0.4);
        }`

    - `th:nth-child(even),td:nth-child(even)
        {
         background-color: rgba(150, 212, 212, 0.4);
        }`
- Horizontal Dividers( bộ chia ngang): 
    - `tr {
         border-bottom: 1px solid #ddd;
        }`
- <u>Sử dụng</u> :hoverbộ chọn trên trđể đánh dấu các hàng trong bảng khi di chuột qua:
    - `so sánh thẻ p với span, b với strong, em với i?`
    - `alt : hỗ trợ cho ng mù khi họ lượt đến sẽ có máy hỗ trợ đọc đoạn text?`
    - `tìm hiểu viewport`
    - `chỉ số của thẻ body?`
- Table Colgroup: phần tử được sử dụng để tạo kiểu cho các cột cụ thể của bảng.
    - Colgroup : 
        - trong colgroup có phần tử col
            - trong col có span và style
            _`span"2": chọn số cột đổ màu là 2"
## **list :**
    - ul: xác định 1 danh sách k có thứ tự
    - ol: xác định danh sách theo thứ tự
    - li: xsc định một mục dah sách
    - dl: xác định một danh sách mô tả.
    - dt: Xác định một thuật ngữ trong một danh sách mô tả

    - dd:Mô tả thuật ngữ trong một danh sách mô tả
- Unordered HTML List - Choose List Item Marker
    - Thuộc tính `CSS list-style-type`được sử dụng để xác định kiểu của điểm đánh dấu mục danh sách. Nó có thể có một trong các giá trị sau:    
        - disc : Đĩa
        - circle :Set point đánh dấu danh sách mục thành một vòng tròn
        - square: Hình vuông
        - none : Không có
- Other Lists
## **HTML Block and Inline Elements**

- Block-level Elements
        - Phần tử cấp khối luôn bắt đầu trên một dòng mới và trình duyệt sẽ tự động thêm một số khoảng trắng (lề) trước và sau phần tử.
        - Một phần tử cấp khối luôn chiếm toàn bộ chiều rộng có sẵn (trải dài sang trái và phải hết mức có thể).
        - Hai phần tử khối thường được sử dụng là: p và div.

        - Phần p tử xác định một đoạn văn trong tài liệu HTML.

        - Phần div tử xác định một bộ phận hoặc một phần trong tài liệu HTML.
- Inline Elements
        - Một phần tử nội tuyến không bắt đầu trên một dòng mới.
        - Một phần tử nội tuyến chỉ chiếm nhiều chiều rộng khi cần thiết.
        - div: là cấp khối và thường được sử dụng làm vùng chứa cho các phần tử HTML khác
        - là một vùng chứa nội tuyến được sử dụng để đánh dấu một phần của văn bản hoặc một phần của tài liệu
## **HTML class Attribute**
        - JavaScript có thể truy cập các phần tử có tên lớp cụ thể bằng `getElementsByClassName()`phương thức
## **HTML Iframe:**
- HTML Iframe Syntax: 
    - iframe: Thẻ chỉ định một khung nội tuyến
    - Một khung nội tuyến được sử dụng để nhúng một tài liệu khác trong tài liệu HTML hiện tại.
    - Iframe - Đặt Chiều cao và Chiều rộng
    - Iframe - Xóa đường viền
    - Iframe - Nhắm mục tiêu cho một liên kết
        - Thẻ HTML iframe chỉ định khung nội tuyến
        - Thuộc src tính xác định URL của trang để nhúng
        - Luôn bao gồm một titlethuộc tính (dành cho trình đọc màn hình)
        - Thuộc tính heightvà widthchỉ định kích thước của iframe
        - Sử dụng border:none;để xóa đường viền xung quanh iframe
## **HTML JavaScript**
- Thẻ HTML script
    - script: được sử dụng để xác định một tập lệnh phía máy khách (JavaScript).
    - Phần script tử chứa các câu lệnh script hoặc nó trỏ đến một tệp script bên ngoài thông qua srcthuộc tính.
    - Các ứng dụng phổ biến cho JavaScript là thao tác hình ảnh, xác thực biểu mẫu và các thay đổi động của nội dung.
    - Để chọn một phần tử HTML, JavaScript thường sử dụng `document.getElementById()`phương pháp này nhất.
- thẻ noscript
    - xác định nội dung thay thế sẽ được hiển thị cho người dùng đã tắt tập lệnh trong trình duyệt của họ hoặc có trình duyệt không hỗ trợ tập lệnh:
## **HTML File Paths**
- Đường dẫn tệp HTML
    - Đường dẫn tệp mô tả vị trí của tệp trong cấu trúc thư mục của trang web.
    - Đường dẫn tệp được sử dụng khi liên kết với các tệp bên ngoài
        - Web pages
        - Images phần 
        - Style sheets
        - JavaScripts
## **HTML - The Head Element**
- Phần tử HTML head
    - là vùng chứa siêu dữ liệu (dữ liệu về dữ liệu) và được đặt giữa html thẻ và body thẻ.
    - Siêu dữ liệu HTML là dữ liệu về tài liệu HTML. Siêu dữ liệu không được hiển thị.
    - Siêu dữ liệu thường xác định tiêu đề tài liệu, bộ ký tự, kiểu, tập lệnh và các thông tin meta khác
- Phần tử HTML title
    - xác định tiêu đề của tài liệu. Tiêu đề phải ở dạng chỉ văn bản và nó được hiển thị trên thanh tiêu đề của trình duyệt hoặc trong tab của trang
    - bắt buộc trong các tài liệu HTML!
    - Nội dung của tiêu đề trang rất quan trọng đối với việc tối ưu hóa công cụ tìm kiếm (SEO)! Tiêu đề trang được sử dụng bởi các thuật toán của công cụ tìm kiếm để quyết định thứ tự khi liệt kê các trang trong kết quả tìm kiếm
        - xác định tiêu đề trong thanh công cụ của trình duyệt
        - cung cấp tiêu đề cho trang khi nó được thêm vào mục yêu thích
        - cung cấp tiêu đề cho trang khi nó được thêm vào mục yêu thích
- thể meta: `thường được sử dụng để chỉ định bộ ký tự, mô tả trang, từ khóa, tác giả của tài liệu và cài đặt chế độ xem`
    - thường được sử dụng để chỉ định bộ ký tự, mô tả trang, từ khóa, tác giả của tài liệu và cài đặt chế độ xem.
    - Siêu dữ liệu sẽ không được hiển thị trên trang, nhưng được sử dụng bởi các trình duyệt (cách hiển thị nội dung hoặc tải lại trang), bởi các công cụ tìm kiếm (từ khóa) và các dịch vụ web khác.
- Đặt chế độ xem để làm cho trang web của bạn trông đẹp trên tất cả các thiết bị:
 `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- Chế độ xem là vùng hiển thị của người dùng trên một trang web. Nó thay đổi theo thiết bị - nó sẽ nhỏ hơn trên điện thoại di động hơn là trên màn hình máy tính.

Bạn nên đưa meta phần tử sau vào tất cả các trang web của mình
- Điều này cung cấp cho trình duyệt hướng dẫn về cách kiểm soát kích thước và tỷ lệ của trang.
- Phần `width=device-width` ặt chiều rộng của trang tuân theo chiều rộng màn hình của thiết bị (sẽ thay đổi tùy theo thiết bị).
- Phần `initial-scale=1.0` đặt mức thu phóng ban đầu khi trang được tải lần đầu tiên bởi trình duyệt
- thẻ base : Phần tử chỉ định URL cơ sở và / hoặc mục tiêu cho tất cả các URL tương đối trong một trang
- Thẻ base phải có một href hoặc một thuộc tính đích hoặc cả hai.
- Chỉ có thể có một base phần tử duy nhất trong một tài liệu!
## **HTML Layout Elements and Techniques**
- Phần tử bố cục HTML
    - header: Xác định tiêu đề cho một tài liệu hoặc một phần
    - nav : Xác định một tập hợp các liên kết điều hướng
    - section : Xác định một phần trong tài liệu
    - article : Xác định một nội dung độc lập, khép kín
    - aside: Xác định nội dung bên cạnh nội dung (như một thanh bên)
    - footer : Xác định chân trang cho một tài liệu hoặc một phần
    - details :  Xác định các chi tiết bổ sung mà người dùng có thể mở và đóng theo yêu cầu
    - summary : Xác định tiêu đề cho details phần tử

    ![](https://user-images.githubusercontent.com/89244324/164264649-f02e3aa6-d077-4d6e-9c68-576dc7f98aef.png)

- Kỹ thuật bố cục HTML
- Có bốn kỹ thuật khác nhau để tạo bố cục nhiều cột. Mỗi kỹ thuật đều có ưu và nhược điểm của nó:


        - Khung CSS
        - Thuộc tính float CSS
        - CSS flexbox
        - Lưới CSS
## **HTML Responsive Web Design**
- Thiết kế web đáp ứng là tạo ra các trang web có giao diện đẹp trên tất cả các thiết bị!
- Viewport là kích thước cửa sổ trình duyệt. 1vw = 1% chiều rộng khung nhìn. Nếu khung nhìn rộng 50cm, 1vw là 0,5cm.

## **HTML Computer Code Elements**
- HTML kbd For Keyboard Input:  
    - Phần tử được sử dụng để xác định đầu vào bàn phím. Nội dung bên trong được hiển thị trong phông chữ monospace mặc định của trình duyệt.
    - kbd :  xác định đầu vào bàn phím
    - samp : xác định đầu ra mẫu từ một chương trình máy tính
    - code:  xác định một đoạn mã máy tính
    - var: xác định một biến trong lập trình hoặc trong một biểu thức toán học
    - pre: xác định văn bản được định dạng trước
## **HTML Semantic Elements: **
//- max-width :  chiều rộng tối đa//
- Các yếu tố ngữ nghĩa là gì?
- Ví dụ về các yếu tố phi ngữ nghĩa : div và span - Không cho biết gì về nội dung của nó.
- Ví dụ về các yếu tố ngữ nghĩa:,form và table- article Xác định rõ ràng nội dung của nó.
    - figure  :chỉ định nội dung độc lập, như hình minh họa, sơ đồ, ảnh, danh sách mã, v.v.
    - figcaption : xác định chú thích cho một figure phần tử. Phần figcaption tử có thể được đặt làm con đầu tiên hoặc con cuối cùng của một figure phần tử.
## **HTML Style Guide**
- Mã HTML nhất quán, sạch sẽ và gọn gàng giúp người khác đọc và hiểu mã của bạn dễ dàng hơn.
-  Dưới đây là một số hướng dẫn và mẹo để tạo mã HTML tốt.
- Sử dụng tên phần tử chữ thường
- Đóng tất cả các phần tử HTML
- Sử dụng tên thuộc tính viết thường
- Luôn trích dẫn các giá trị thuộc tính
- Luôn chỉ định alt, chiều rộng và chiều cao cho Hình ảnh
- Dấu cách và dấu bằng: HTML cho phép khoảng trắng xung quanh các dấu bằng. Nhưng không gian ít hơn sẽ dễ đọc hơn và nhóm các thực thể lại với nhau tốt hơn.
- Tránh các dòng mã dài: 
- Dòng trống và thụt đầu dòng:
- Để dễ đọc, hãy thêm hai khoảng cách thụt lề. Không sử dụng phím tab.
## **HTML Entities**
- Các ký tự dành riêng trong HTML phải được thay thế bằng các thực thể ký tự.
## **HTML Symbols**
- Các ký hiệu không có trên bàn phím của bạn cũng có thể được thêm vào bằng cách sử dụng các thực thể.
## **Using Emojis in HTMLUsing Emojis in HTML**
- Biểu tượng cảm xúc là các ký tự từ bộ ký tự UTF-8:
- Biểu tượng cảm xúc trông giống như hình ảnh hoặc biểu tượng, nhưng thực tế không phải vậy.
- Chúng là các chữ cái (ký tự) từ bộ ký tự UTF-8 (Unicode).
- UTF-8 bao gồm hầu hết tất cả các ký tự và biểu tượng trên thế giới.
- Nhiều ký tự UTF-8 không thể được nhập trên bàn phím, nhưng chúng luôn có thể được hiển thị bằng số (được gọi là số thực thể):
    - A là 65
    - B là 66
    - c là 67 
- `Để trình duyệt hiểu rằng bạn đang hiển thị một ký tự, bạn phải bắt đầu số thực thể bằng & # và kết thúc bằng; (dấu chấm phẩy).`
## **HTML Encoding (Character Sets)**
- Để hiển thị trang HTML một cách chính xác, trình duyệt web phải biết bộ ký tự nào sẽ sử dụng.
- Từ ASCII đến UTF-8
    - ASCII là tiêu chuẩn mã hóa ký tự đầu tiên. ASCII đã xác định 128 ký tự khác nhau có thể được sử dụng trên internet: số (0-9), chữ cái tiếng Anh (AZ) và một số ký tự đặc biệt như! $ + - () @ <>.
    - ISO-8859-1 là bộ ký tự mặc định cho HTML 4. Bộ ký tự này hỗ trợ 256 mã ký tự khác nhau. HTML 4 cũng được hỗ trợ UTF-8.
    - ANSI (Windows-1252) là bộ ký tự gốc của Windows. ANSI giống với ISO-8859-1, ngoại trừ ANSI có 32 ký tự phụ.
    - Đặc tả HTML5 khuyến khích các nhà phát triển web sử dụng bộ ký tự UTF-8, bao gồm hầu hết tất cả các ký tự và ký hiệu trên thế giới!
## **HTML Uniform Resource Locators**
- URL là một từ khác để chỉ địa chỉ web.
- URL có thể bao gồm các từ (ví dụ: w3schools.com) hoặc địa chỉ Giao thức Internet (IP) (ví dụ: 192.68.20.50).
- Hầu hết mọi người nhập tên khi lướt web, vì tên dễ nhớ hơn số.
**URL - Uniform Resource Locator**
- Trình duyệt web yêu cầu các trang từ máy chủ web bằng cách sử dụng một URL.
    - scheme :xác định loại dịch vụ Internet (phổ biến nhất là http hoặc https )
    - prefix: xác định tiền tố tên miền (mặc định cho http là www )
    - domain :xác định tên miền Internet (như w3schools.com)
    - port:xác định số cổng tại máy chủ (mặc định cho http là 80 )
    - path:xác định một đường dẫn tại máy chủ (Nếu bỏ qua: thư mục gốc của trang web)
    - filename:xác định tên của tài liệu hoặc tài nguyên 
    - http: Chung web các trang. Không được mã hóa
    - https: Trang web an toàn. Mã hóa
    - ftp: 
## **HTML so với XHTML**
- XHTML là một phiên bản HTML dựa trên XML chặt chẽ hơn.
**XHTML là gì?**
- XHTML stands for EXtensible HyperText Markup Language
- XHTML là một phiên bản HTML dựa trên XML chặt chẽ hơn

- XHTML là HTML được định nghĩa là một ứng dụng XML
- XHTML được hỗ trợ bởi tất cả các trình duyệt chính
- <! DOCTYPE> là bắt buộc
Thuộc tính xmlns trong html là bắt buộc
html, head, title và body là bắt buộc
Các phần tử phải luôn được lồng đúng cách
Các phần tử phải luôn được đóng
Các phần tử phải luôn ở dạng chữ thường
Tên thuộc tính phải luôn ở dạng chữ thường
Giá trị thuộc tính phải luôn được trích dẫn
Giảm thiểu thuộc tính bị cấm
- Các phần tử XHTML phải được lồng nhau đúng cách
- Các phần tử XHTML phải luôn được đóng
- Các phần tử trống XHTML Phải luôn được đóng
- Phần tử XHTML Phải ở dạng chữ thường
- Tên thuộc tính XHTML Phải ở dạng chữ thường
- Các Giá trị Thuộc tính XHTML Phải được Trích dẫn
## **HTML FORMS**
- Một biểu mẫu HTML được sử dụng để thu thập đầu vào của người dùng. Đầu vào của người dùng thường được gửi đến một máy chủ để xử lý.
- The form Element
-  Một input phần tử có thể được hiển thị theo nhiều cách, tùy thuộc vào type thuộc tính.
    - radio: Hiển thị một nút radio (để chọn một trong nhiều lựa chọn)

    - text: Hiển thị trường nhập văn bản một dòng
    - checkbox: Hiển thị hộp kiểm (để chọn không hoặc nhiều lựa chọn)
    - submit: Hiển thị nút gửi (để gửi biểu mẫu) 
    - button: 	Hiển thị một nút có thể nhấp
- input: nếu k có thuộc tính name thì sẽ biji bỏ qua,  giá trị của trường đầu vào sẽ hoàn toàn không được gửi.

**HTML Form Attributes**
- The Action Attribute
    -  Thuộc tính action xác định hành động được thực hiện khi biểu mẫu được gửi
    - Thông thường, dữ liệu biểu mẫu được gửi đến tệp trên máy chủ khi người dùng nhấp vào nút gửi.
    - 
- HTML Form Elements : 
    - Phần tử input:Phần input tử có thể được hiển thị theo một số cách, tùy thuộc vào type thuộc tính.
    - The label Element: dùng để định nghĩa nhãn cho các thẻ input trong HTML
        - Tác dụng của label là làm cho thao tác nhập liệu trở nên dễ dàng hơn.
         -Thuộc for tính của label thẻ phải bằng idthuộc tính của input phần tử để liên kết chúng lại với nhau.
    - The select Element: Phần tử xác định danh sách thả xuống
        - option : các yếu tố xác định một tùy chọn có thể được chọn

        - selected : Để xác định một tùy chọn đã chọn trước
    - Visible Values: (giá trị có thể nhìn thấy):
    - Thuộc tính để chỉ định số lượng giá trị hiển thị:
    - Allow Multiple Selections: cho phép nhiều lựa chọn
         - multiple: Thuộc tính cho phép người dùng chọn nhiều hơn một giá trị:
    - textarea:  element defines a multi-line input field
        - rows: Thuộc tính Chỉ định số lượng dòng hiển thị trong một vùng văn    bản.
        - cols: Thuộc tính Chỉ định chiều rộng hiển thị của một vùng văn bản.
- button 
    - The fieldset and legend Elements: 
       - fieldset : Phần tử được sử dụng để nhóm dữ liệu liên quan trong một biểu mẫu
       - legend: yếu tố xác định chú thích cho fieldset
    - datalist: Phần tử chỉ định một danh sách các tùy chọn được xác định trước cho một input
    - output: yếu tố đại diện cho kết quả của một tính toán
- Input Types: 
    - Giá trị mặc định của typethuộc tính là "văn bản".
    - các giá trị của thuộc tính text trong Input
        - text: trường nhập văn bản một dòng 
        - checkbox: xác định một hộp kiểm cho phép người dùng chọn tùy chọn KHÔNG hoặc NHIỀU tùy chọn trong một số lựa chọn giới hạn.
        - color: Loại đầu vào Màu sắc
        - date: Loại đầu vào Ngày
        - password: xác định một trường mật khẩu
        - submit:xác định một nút để gửi dữ liệu biểu mẫu đến trình xử lý biểu mẫu
        - reset: xác định nút đặt lại sẽ đặt lại tất cả các giá trị biểu mẫu về giá trị mặc định của chúng
        - radio: xác định một nút radio và chỉ đc chọn 1 trong các lựa chọn giới hạn
        - button: xác định một nút
        - datetime-local: Loại đầu vào Ngày giờ-cục bộ
        - email: Loại đầu vào Email
        - file: Tệp loại đầu vào
        - hidden: nghĩa một trường nhập ẩn (không hiển thị cho người dùng)
        - month: cho phép người dùng chọn tháng và năm
        - number: Số loại đầu vào
        - range: Phạm vi loại đầu vào là một thanh trượt
        - search: tìm kiếm (một trường tìm kiếm hoạt động giống như một trường văn bản thông thường).
        - tel : nhập phải chứa số điện thoại.
        - time: phép người dùng chọn thời gian (không có múi giờ).
        - url: vào phải chứa địa chỉ URL.
        - week: cho phép người dùng chọn một tuần và năm.
    - Input Restrictions: các thuộc tính hạn chế đầu vào:
        - checked: Chỉ định rằng trường đầu vào phải được chọn trước khi trang tải (đối với Type = "hộp kiểm" hoặc loại = "radio")
        - disabled: Chỉ định rằng một trường đầu vào sẽ được vô hiệu hóa
        - max: chỉ định giá trị tối đa cho một đầu vào
        - maxlength: Chỉ định số lượng ký tự tối đa cho trường đầu vào
        - min: chỉ định giá trị tối thiểu cho một đầu avfo
        - pattern: Chỉ định một biểu thức chính quy để kiểm tra giá trị đầu vào so với
        - readonly: Chỉ định rằng một trường đầu vào chỉ được đọc (không thể thay đổi)
        - required: Chỉ định rằng một trường đầu vào là bắt buộc (phải được điền)
        - value: Chỉ định các khoảng số hợp pháp cho một trường nhập
        - size: Chỉ định chiều rộng (tính bằng ký tự) của trường nhập
        - step: Chỉ định các khoảng số hợp pháp cho một trường nhập

    **HTML Input Attributes**
    - value: Thuộc tính giá trị
    - readonly : Thuộc tính chỉ đọc không nhập được, sẽ được gửi khi gửi biểu mẫu!
    - disabled: Thuộc tính bị vô hiệu hóa, k đc gửi khi gửi biểu mẫu
    - size: 
    - multiple
    - min
    - max
    - maxlength
    - multiple : chỉ định rằng người dùng được phép nhập nhiều giá trị vào một trường đầu vào, Thuộc multipletính hoạt động với các loại đầu vào sau: email và tệp.
    - pattern: chỉ định một biểu thức chính quy mà giá trị của trường đầu vào được kiểm tra, khi biểu mẫu được gửi., hoạt động với các loại đầu vào sau: văn bản, ngày tháng, tìm kiếm, url, số điện thoại, email và mật khẩu.
    - placeholder: chỉ định một gợi ý ngắn mô tả giá trị mong đợi của trường đầu vào (giá trị mẫu hoặc mô tả ngắn về định dạng mong đợi)., hoạt động với các loại đầu vào sau: văn bản, tìm kiếm, url, điện thoại, email và mật khẩu
    - required: 
    - step: định khoảng số hợp pháp cho một trường đầu vào. vd: step="3" thì gtri trả về sẽ là tăng giảm cho 3
    - autofocus: định rằng trường nhập sẽ tự động lấy tiêu điểm khi tải trang.
    - autocomplete: 
    - list: chỉ định xem biểu mẫu hoặc trường nhập liệu có nên bật hoặc tắt tính năng tự động hoàn thành hay không., Tự động điền cho phép trình duyệt dự đoán giá trị. Khi người dùng bắt đầu nhập vào một trường, trình duyệt sẽ hiển thị các tùy chọn để điền vào trường, dựa trên các giá trị đã nhập trước đó.
**HTML Input form* Attributes**
- HTML Input form* Attributes
    - Chương này mô tả các form*thuộc tính khác nhau cho phần tử HTML input.
    - Thuộc tính biểu mẫu()
        - form Thuộc tính đầu vào chỉ định hình thức mà input phần tử thuộc về.
        - Giá trị của thuộc tính này phải bằng thuộc tính id của phần tử form mà nó thuộc về.
    - Thuộc tính formaction 
        - Giá trị của thuộc tính này phải bằng thuộc tính id của phần tử form mà nó thuộc về.
        - Thuộc tính này ghi đè actionthuộc tính của form phần tử.
        - Thuộc formactiontính hoạt động với các loại đầu vào sau: gửi và hình ảnh.
    - Thuộc tính formenctype:
        - Thuộc tính đầu vào formenctype chỉ định cách mã hóa dữ liệu biểu mẫu khi gửi (chỉ dành cho biểu mẫu có method = "post").
        - Thuộc tính này ghi đè thuộc tính enctype của form phần tử.
        - Thuộc formenctypetính hoạt động với các loại đầu vào sau: gửi và hình ảnh
        - Thuộc formenctype tính hoạt động với các loại đầu vào sau: gửi và hình ảnh
        - Thuộc tính formmethod: Thuộc tính đầu vào formmethod xác định phương thức HTTP để gửi dữ liệu biểu mẫu đến URL hành động.
        - Thuộc tính formmethod: Thuộc tính đầu vào formmethod xác định phương thức HTTP để gửi dữ liệu biểu mẫu đến URL hành động.
        -  Thuộc tính này ghi đè thuộc tính phương thức của formphần tử.
        - Thuộc formmethodtính hoạt động với các loại đầu vào sau: gửi và hình ảnh.
       - Thuộc formmethodtính hoạt động với các loại đầu vào sau: gửi và hình ảnh.
        - Thuộc tính formmethod
             - Thuộc tính đầu vào formmethod xác định phương thức HTTP để gửi dữ liệu biểu mẫu đến URL hành động.
             - Thuộc tính đầu vào formmethod xác định phương thức HTTP để gửi dữ liệu biểu mẫu đến URL hành động.
    -  Dữ liệu biểu mẫu có thể được gửi dưới dạng biến URL (method = "get") hoặc dưới dạng giao dịch bài đăng HTTP (method = "post").
    - ` lưu ý`:Dữ liệu biểu mẫu có thể được gửi dưới dạng biến URL (method = "get") hoặc dưới dạng giao dịch bài đăng HTTP (method = "post").
    - *Notes on the "get" method:(lưu ý về phương thức get)*
        - Phương thức này nối dữ liệu biểu mẫu vào URL trong các cặp tên / giá trị
        - Phương pháp này hữu ích cho các lần gửi biểu mẫu mà người dùng muốn đánh dấu kết quả
        - Có giới hạn về số lượng dữ liệu bạn có thể đặt trong một URL (thay đổi giữa các trình duyệt), do đó, bạn không thể chắc chắn rằng tất cả dữ liệu biểu mẫu sẽ được chuyển một cách chính xác
        - Không bao giờ sử dụng phương pháp "lấy" để chuyển thông tin nhạy cảm! (mật khẩu hoặc thông tin nhạy cảm khác sẽ hiển thị trên thanh địa chỉ của trình duyệt)
    - *lưu ý về phương thức post*
        - Phương thức này gửi dữ liệu biểu mẫu dưới dạng giao dịch bài đăng HTTP
        - Không thể đánh dấu các bài gửi biểu mẫu bằng phương pháp "đăng"
        - Phương thức "post" mạnh mẽ và an toàn hơn "get" và "post" không có giới hạn về kích thước
- The formtarget Attribute

    - Thuộc tính đầu vào formtargetchỉ định tên hoặc từ khóa cho biết vị trí hiển thị phản hồi nhận được sau khi gửi biểu mẫu.
## **HTML Graphics**
- HTML Canvas Graphics
    - Phần tử HTML canvas được sử dụng để vẽ đồ họa trên trang web.
    - Hình bên trái được tạo bằng canvas. Nó hiển thị bốn yếu tố: một hình chữ nhật màu đỏ, một hình chữ nhật gradient, một hình chữ nhật nhiều màu và một văn bản nhiều màu.

    - HTML Canvas là gì?
      - Phần tử HTML canvas được sử dụng để vẽ đồ họa một cách nhanh chóng, thông qua JavaScript.
      - Phần canvas tử chỉ là một vùng chứa cho đồ họa. Bạn phải sử dụng JavaScript để thực sự vẽ đồ họa.
      -  Canvas có một số phương pháp để vẽ đường dẫn, hộp, hình tròn, văn bản và thêm hình ảnh.
    - Hỗ trợ trình duyệt
- Đồ họa HTML SVG
    - SVG định nghĩa đồ họa dựa trên vectơ ở định dạng XML.
- SVG là gì?
    - SVG là viết tắt của Scalable Vector Graphics
    - SVG được sử dụng để xác định đồ họa cho Web
    - SVG là một khuyến nghị của W3C
- Phần tử svg HTML
    - Phần tử HTML svg là vùng chứa đồ họa SVG.
    - Phần tử HTML svg là vùng chứa đồ họa SVG.
## **HTML Media**
- ### HTML Multimedia
- Đa phương tiện trên web là âm thanh, âm nhạc, video, phim và hình động.
- Đa phương tiện là gì?
    - Đa phương tiện có nhiều định dạng khác nhau. Đó có thể là hầu hết mọi thứ bạn có thể nghe hoặc nhìn thấy, như hình ảnh, nhạc, âm thanh, video, bản ghi, phim, hoạt ảnh và hơn thế nữa.
    - Các trang web thường chứa các phần tử đa phương tiện với nhiều kiểu và định dạng khác nhau.
- Hỗ trợ trình duyệt
    - Các trình duyệt web đầu tiên chỉ hỗ trợ cho văn bản, giới hạn ở một phông chữ duy nhất với một màu duy nhất.
    - Sau đó là các trình duyệt hỗ trợ màu sắc, phông chữ, hình ảnh và đa phương tiện!
- Định dạng đa phương tiện
    - Các phần tử đa phương tiện (như âm thanh hoặc video) được lưu trữ trong các tệp phương tiện.
    - Cách phổ biến nhất để phát hiện loại tệp là xem phần mở rộng tệp.
    - Các tệp đa phương tiện có các định dạng và phần mở rộng khác nhau như: .wav, .mp3, .mp4, .mpg, .wmv và .avi.
    - Các định dạng video phổ biến: 
        - 	Có rất nhiều định dạng video trên mạng.

        - Các định dạng MP4, WebM và Ogg được hỗ trợ bởi HTML.

        - Định dạng MP4 được YouTube khuyến nghị.
## **HTML Video**
- The HTML video element is used to show a video on a web page.
- The HTML video Element:
    - Làm thế nào nó hoạt động: 
        - controls:  thêm các điều khiển video, như phát, tạm dừng và âm lượng
        - Bạn nên luôn bao gồm widthvà heightcác thuộc tính. Nếu chiều cao và chiều rộng không được đặt, trang có thể nhấp nháy trong khi tải video.
        - source: cho phép bạn chỉ định các tệp video thay thế mà trình duyệt có thể chọn. Trình duyệt sẽ sử dụng định dạng được nhận dạng đầu tiên.
        - Văn bản giữa các thẻ video và /video sẽ chỉ được hiển thị trong các trình duyệt không hỗ trợ video phần tử.
        - Để tự động bắt đầu một video, hãy sử dụng autoplaythuộc tính:
        -  `Lưu ý:` Trong hầu hết các trường hợp, trình duyệt Chromium không cho phép tự động phát. Tuy nhiên, luôn cho phép tự động phát bị tắt tiếng.
        - Thêm mutedsau autoplayđể video của bạn bắt đầu tự động phát (nhưng bị tắt tiếng):
    - DOM HTML xác định các phương thức, thuộc tính và sự kiện cho video phần tử.
    - Điều này cho phép bạn tải, phát và tạm dừng video cũng như đặt thời lượng và âm lượng.
    - Ngoài ra còn có các sự kiện DOM có thể thông báo cho bạn khi video bắt đầu phát, bị tạm dừng, v.v.
## **HTML Audio**
- Phần tử Audio HTML được sử dụng để phát tệp âm thanh trên trang web.
- The HTML audio Element: Để phát tệp âm thanh trong HTML, hãy sử dụng audio phần tử:
- Âm thanh HTML - Cách hoạt động
    - controls: thêm các điều khiển âm thanh, như phát, tạm dừng và âm lượng.
    - source:  cho phép bạn chỉ định các tệp âm thanh thay thế mà trình duyệt có thể chọn. Trình duyệt sẽ sử dụng định dạng được nhận dạng đầu tiên.
    -  cho phép bạn chỉ định các tệp âm thanh thay thế mà trình duyệt có thể chọn. Trình duyệt sẽ sử dụng định dạng được nhận dạng đầu tiên.
    - HTML audio Tự động phát: Để tự động khởi động tệp âm thanh, hãy sử dụng autoplaythuộc tính:

- HTML Plug-ins: Plug-in là các chương trình máy tính mở rộng chức năng tiêu chuẩn của trình duyệt.
- Plug-ins: được thiết kế để sử dụng cho nhiều mục đích khác nhau:
    - Để chạy các applet java
    - Để chạy Microsoft ActiveX Controls
    - Để hiển thị phim Flash
    - Để hiển thị bản đồ
    - Để quét vi-rút
    - Để xác minh ID ngân hàng
- Phần tử object: được hỗ trợ bởi tất cả các trình duyệt
    - Phần tử được hỗ trợ bởi tất cả các trình duyệt
- Nó được thiết kế để nhúng các trình cắm thêm (như các applet java, đầu đọc PDF và trình phát flash) trong các trang web, nhưng cũng có thể được sử dụng để bao gồm HTML trong HTML:
- phần tử embed: được hỗ trợ trong tất cả các trình duyệt chính
    - cũng định nghĩa một đối tượng nhúng trong tài liệu HTML.
    - Các trình duyệt web đã hỗ trợ phần tử embed trong một thời gian dài. Tuy nhiên, nó không phải là một phần của đặc tả HTML trước HTML5.
    - Lưu ý rằng phần tử embed không có thẻ đóng. Nó không thể chứa văn bản thay thế.
    - Phần embed tử này cũng có thể được sử dụng để đưa HTML vào HTML:


## HTML **YouTube Videos**
- Cách dễ nhất để phát video trong HTML, là sử dụng YouTube.
- Bạn đang gặp khó khăn với các định dạng video?
    - Chuyển đổi video sang các định dạng khác nhau có thể khó khăn và tốn thời gian.
    - Một giải pháp dễ dàng hơn là cho phép YouTube phát video trên trang web của bạn.
- Id Video YouTube
    - Phát video YouTube bằng HTML
- Tự động phát trên YouTube + Tắt tiếng
    - Thêm mute=1sau autoplay=1để video của bạn bắt đầu phát tự động (nhưng bị tắt tiếng).
- Danh sách phát trên YouTube
    - Danh sách video để phát được phân tách bằng dấu phẩy (ngoài URL gốc).
- Vòng lặp YouTube
    - Thêm loop=1để video của bạn lặp lại mãi mãi.(gtri mặc định =0, phát 1 lần, =1 phát mãi mãi)
- Kiểm soát YouTube
- Thêm controls=0để không hiển thị các điều khiển trong trình phát video.Giá trị 

        0: Các điều khiển trình phát không hiển thị.

        Giá trị 1 (mặc định): Màn hình điều khiển trình phát.

## **HTML Geolocation API**
- API định vị địa lý HTML được sử dụng để xác định vị trí của người dùng.
- Xác định vị trí của người dùng
- Vì điều này có thể ảnh hưởng đến quyền riêng tư, vị trí sẽ không có sẵn trừ khi người dùng chấp thuận.
- Hỗ trợ trình duyệt
- Các số trong bảng chỉ định phiên bản trình duyệt đầu tiên hỗ trợ đầy đủ Vị trí địa lý.
- Lưu ý: Kể từ Chrome 50, API vị trí địa lý sẽ chỉ hoạt động trên các ngữ cảnh an toàn như HTTPS. Nếu trang web của bạn được lưu trữ trên nguồn gốc không an toàn (chẳng hạn như HTTP), các yêu cầu lấy vị trí của người dùng sẽ không còn hoạt động.
- Sử dụng định vị địa lý HTML
- Phương `getCurrentPosition()`thức được sử dụng để trả về vị trí của người dùng.
- *Đối tượng Geolocation cũng có các phương thức thú vị khác:*
    - watchPosition(): Trả lại vị trí hiện tại của người dùng và tiếp tục trả lại vị trí đã cập nhật khi người dùng di chuyển (giống như GPS trên ô tô).
    - clearWatch() : Dừng watchPosition()phương thức.
### *HTML Drag and Drop API*
    : Trong HTML, bất kỳ yếu tố nào có thể được kéo và giảm
- Drag and Drop
    - Kéo và thả là một tính năng rất phổ biến. Đó là khi bạn "lấy" một đối tượng và kéo nó đến một vị trí khác.    
- Tạo một phần tử có thể kéo được
- Trước hết: Để làm cho một phần tử có thể kéo được, hãy đặt draggablethuộc tính thành true:
- Kéo gì - ondragstart và setData ()
### HTML Web Storage API: Lưu trữ web HTML; tốt hơn cookie
- Lưu trữ Web HTML là gì? 
Với tính năng lưu trữ web, các ứng dụng web có thể lưu trữ dữ liệu cục bộ trong trình duyệt của người dùng.
- Đối tượng lưu trữ web HTML: Lưu trữ web HTML cung cấp hai đối tượng để lưu trữ dữ liệu trên máy khách:
     - window.localStorage:lưu trữ dữ liệu không có ngày hết hạn
     - window.sessionStorage: lưu trữ dữ liệu cho một phiên (dữ liệu bị mất khi đóng tab trình duyệt)
- API HTML SSE: Sự kiện do máy chủ gửi (SSE) cho phép một trang web nhận các bản cập nhật từ máy chủ.













    


