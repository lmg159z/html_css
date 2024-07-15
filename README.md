# 1. HTML là gì ?

- HTML là viết tắt của Hyper Text Markup Language
- HTML là ngôn ngữ đánh dấu chuẩn để tạo ra các trang Web
- HTML mô tả cấu trúc của một trang Web
- HTML bao gồm một loạt các phần tử
- Các thành phần HTML cho trình duyệt biết cách hiển thị nội dung
- Các phần tử HTML gắn nhãn cho các phần nội dung như "đây là tiêu đề", "đây là đoạn văn", "đây là liên kết", v.v.

# 2. Cấu trúc HTML

###  Lý Thuyết:
  - Tuyên bố này `<!DOCTYPE html>`xác định rằng tài liệu này là tài liệu HTML5
  - Phần **`<html>`**tử là phần tử gốc của một trang HTML
  - Phần **`<head>`** tử chứa thông tin meta về trang HTML
  - Phần tử này **`<title>`** chỉ định tiêu đề cho trang HTML (được hiển thị trên thanh tiêu đề của trình duyệt hoặc trên tab của trang)
  - Phần tử này **`<body>`** xác định phần nội dung của tài liệu và là nơi chứa tất cả nội dung hiển thị, chẳng hạn như tiêu đề, đoạn văn, hình ảnh, siêu liên kết, bảng, danh sách, v.v.
  - Phần tử này **`<h1>`** xác định một tiêu đề lớn
  - Phần tử này **`<p>`** xác định một đoạn văn

### Cấu trúc

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trình bày đoạn văn bản</title>
</head>
<body>
  <!-- block elements-->
</body>
</html>

```

# 3. Định dạng văn bản

### Thuộc tính thẻ

 **`Lý thuyết thuộc tính thẻ (Attributes)`**
  
  - Tất cả các phần tử HTML **có thể** có các thuộc tính
  - Thuộc tính cung cấp thông tin bổ sung về các thành phần
  - Thuộc tính luôn được chỉ định trong thẻ bắt đầu
  - Thuộc tính thường có cặp tên/giá trị như: **name="value"**
  
  **Cấu trúc**

  ```html
  <img src="img_girl.jpg" width="500" height="600" /> 
  <p style="color:red;">This is a red paragraph.</p>
  ```
  
 **`1 số thuộc tính cơ bản`**
  
  1. **`class`**: Được sử dụng để chỉ định một hoặc nhiều lớp CSS cho phần tử.
     ```html
     <div class="container"></div>
     ```
  
  2. **`id`**: Được sử dụng để chỉ định một định danh duy nhất cho phần tử.
     ```html
     <div id="header"></div>
     ```
  
  3. **`style`**: Được sử dụng để áp dụng các kiểu CSS trực tiếp cho phần tử.
     ```html
     <p style="color: red;">`This is a paragraph.</p>
     ```
  
  4. **`src`**: Được sử dụng trong các thẻ như `<img>`, `<script>`, để chỉ định nguồn của tài nguyên bên ngoài.
     ```html
     <img src="image.jpg" alt="Description">
     ```
  
  5. **`href`**: Được sử dụng trong thẻ `<a>` để chỉ định liên kết đến tài nguyên khác.
     ```html
     <a href="https://example.com">`Visit Example</a>
     ```
  
  6. **`alt`**: Được sử dụng trong thẻ `<img>` để cung cấp văn bản thay thế nếu hình ảnh không hiển thị.
     ```html
     <img src="image.jpg" alt="Description">
     ```
  
  7. **`title`**: Cung cấp thông tin chú thích khi người dùng di chuột qua phần tử.
     ```html
     <button title="Submit">Submit</button>
     ```
  
  8. **`type`**: Được sử dụng trong các thẻ như `<input>`, `<button>`, để chỉ định loại của phần tử.
     ```html
     <input type="text" name="username">
     ```
  
  9. **`value`**: Được sử dụng trong các thẻ như `<input>`, `<option>`, để chỉ định giá trị của phần tử.
     ```html
     <input type="text" name="username" value="default">
     ```
  
  10. **`name`**: Được sử dụng trong các thẻ như `<input>`, `<form>`, để chỉ định tên của phần tử.
      ```html
      <input type="text" name="username">
      ```
  

### Các thẻ trình bày văn bản

  1. **Heading (Tiêu đề):**
     - `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`: Được sử dụng để tạo các tiêu đề với kích thước khác nhau, `<h1>` là lớn nhất và `<h6>` là nhỏ nhất.
       ```html
       <h1>Tiêu đề 1</h1>
       <h2>Tiêu đề 2</h2>
       ```
  
  2. **Paragraph (Đoạn văn):**
     - `<p>`: Được sử dụng để tạo đoạn văn.
       ```html
       <p>Đây là một đoạn văn bản.</p>
       ```
  
  3. **Bold (In đậm):**
     - `<b>` hoặc `<strong>`: Làm cho văn bản in đậm.
       ```html
       <b>Văn bản in đậm</b>
       <strong>Văn bản quan trọng</strong>
       ```
  
  4. **Italic (In nghiêng):**
     - `<i>` hoặc `<em>`: Làm cho văn bản in nghiêng.
       ```html
       <i>Văn bản in nghiêng</i>
       <em>Văn bản nhấn mạnh</em>
       ```
  
  5. **Underline (Gạch chân):**
     - `<u>`: Làm cho văn bản gạch chân.
       ```html
       <u>Văn bản gạch chân</u>
       ```
  
  6. **Break (Xuống dòng):**
     - `<br>`: Tạo một ngắt dòng.
       ```html
       Đây là dòng đầu tiên.<br>Đây là dòng thứ hai.
       ```
  
  7. **Horizontal Rule (Dòng ngang):**
     - `<hr>`: Tạo một dòng ngang phân cách nội dung.
       ```html
       <hr>
       ```
  
  8. **Blockquote (Trích dẫn khối):**
     - `<blockquote>`: Được sử dụng để trích dẫn một đoạn văn dài.
       ```html
       <blockquote>Đây là một đoạn trích dẫn.</blockquote>
       ```
  
  9. **Lists (Danh sách):**
     - **Ordered List (Danh sách có thứ tự):** `<ol>` và `<li>`
       ```html
       <ol>
         <li>Mục thứ nhất</li>
         <li>Mục thứ hai</li>
       </ol>
       ```
     - **Unordered List (Danh sách không thứ tự):** `<ul>` và `<li>`
       ```html
       <ul>
         <li>Mục thứ nhất</li>
         <li>Mục thứ hai</li>
       </ul>
       ```
  
  10. **Code (Mã nguồn):**
      - `<code>`: Được sử dụng để hiển thị đoạn mã nguồn.
        ```html
        <code>console.log('Hello, world!');</code>
        ```
  
  11. **Span (Phần văn bản):**
      - `<span>`: Được sử dụng để nhóm các phần tử trong một dòng.
        ```html
        <span style="color: red;">`Văn bản màu đỏ</span>
        ```
  
  12. **Div (Khối):**
      - `<div>`: Được sử dụng để nhóm các phần tử thành một khối.
        ```html
        <div style="background-color: lightgrey;">
          Đây là một khối.
        </div>
        ```

# 4.Định dạng danh sách 

1. **Danh sách HTML không có thứ tự**

- Danh sách không có thứ tự bắt đầu bằng `<ul>`thẻ. Mỗi mục danh sách bắt đầu bằng `<li>`thẻ.
- Theo mặc định, các mục trong danh sách sẽ được đánh dấu bằng dấu đầu dòng (vòng tròn đen nhỏ):

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

2. **Danh sách HTML có thứ tự**

- Danh sách có thứ tự bắt đầu bằng `<ol>`thẻ. Mỗi mục danh sách bắt đầu bằng `<li>`thẻ.
- Theo mặc định, các mục trong danh sách sẽ được đánh dấu bằng số:
- Có thể thay đổi các mục đánh dấu danh sách bằng thuộc tính type 

```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```


3. **Danh sách mô tả HTML**

- HTML cũng hỗ trợ danh sách mô tả.
- Danh sách mô tả là danh sách các thuật ngữ, kèm theo mô tả cho từng thuật ngữ.
- Thẻ `<dl>`xác định danh sách mô tả, `<dt>`thẻ xác định thuật ngữ (tên) và `<dd>` thẻ mô tả từng thuật ngữ:

```html
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```

# 5. Định dạng bản (table)

1. **Định nghĩa một bảng HTML**

- Một bảng trong HTML bao gồm các ô trong bảng bên trong các hàng và cột
- Tiêu đề bảng
  + Đôi khi bạn muốn các ô của mình là các ô tiêu đề bảng. Trong những trường hợp đó, hãy sử dụng thẻ `<th>` thay vì `<td>`thẻ:
  + **th** viết tắt của tiêu đề bảng.
- Các ô của bảng
  + Mỗi ô trong bảng được xác định bởi thẻ a `<td>`và a `</td>`.
  + td là viết tắt của dữ liệu bảng.
  + Mọi thứ nằm giữa `<td>`và `</td>`là nội dung của ô trong bảng.
- Hàng của bảng
  + Mỗi hàng của bảng bắt đầu bằng ký tự a `<tr>`và kết thúc bằng `</tr>`thẻ.
  + tr có nghĩa là hàng bàn.
- Theo mặc định, văn bản trong `<th>`các phần tử được in đậm và căn giữa, nhưng bạn có thể thay đổi điều này bằng CSS.

2. **Ví Dụ**

```html
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```

# 6. Liên kết

1. **Khái Niệm**

- Liên kết HTML là siêu liên kết.
- Bạn có thể nhấp vào liên kết và chuyển đến tài liệu khác.
- Khi bạn di chuyển chuột qua một liên kết, mũi tên chuột sẽ biến thành hình bàn tay nhỏ.

2. **Cú Pháp**
 
```html
<a href="url">link text</a>
```

- Thuộc tính quan trọng nhất của phần `<a>` tử là hrefthuộc tính cho biết đích đến của liên kết.
- Văn bản liên kết là phần mà người đọc sẽ nhìn thấy.
- Khi nhấp vào văn bản liên kết, người đọc sẽ được chuyển đến địa chỉ URL đã chỉ định.
- Theo mặc định, các liên kết sẽ hiển thị như sau trên mọi trình duyệt:
  + Một liên kết chưa được truy cập sẽ được gạch chân và màu xanh
  + Một liên kết đã truy cập được gạch chân và màu tím
  + Một liên kết đang hoạt động được gạch chân và màu đỏ

3. **Thuộc tính**

- Theo mặc định, trang được liên kết sẽ được hiển thị trong cửa sổ trình duyệt hiện tại. Để thay đổi điều này, bạn phải chỉ định một mục tiêu khác cho liên kết.
- Thuộc tính này targetchỉ định nơi mở tài liệu được liên kết.
- Thuộc targettính có thể có một trong các giá trị sau:
  
  + **_self**- Mặc định. Mở tài liệu trong cùng cửa sổ/tab khi nó được nhấp vào
  + **_blank**- Mở tài liệu trong một cửa sổ hoặc tab mới
  + **_parent**- Mở tài liệu trong khung cha
  + **_top**- Mở toàn bộ nội dung của cửa sổ tài liệu
 

```html
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```

4. **URL tương đối**

- Cả hai ví dụ trên đều sử dụng URL tuyệt đối (địa chỉ web đầy đủ) trong hrefthuộc tính.
- Liên kết cục bộ (liên kết đến một trang trong cùng một trang web) được chỉ định bằng URL tương đối (không có phần "https://www"):

```html
<h2>Relative URLs</h2>
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```

5. **các kiểu trong thuộc tính `herf`**

- **URL tuyệt đối**: Chỉ định địa chỉ đầy đủ từ gốc đến đích.
   ```html
   <a href="https://example.com">`Example</a>
   ```

-  **URL tương đối**: Địa chỉ URL dựa trên vị trí hiện tại của tài liệu HTML.
   ```html
   <a href="../path/to/page.html">`Example</a>
   ```

-  **Anchor Link (neo)**: Đường dẫn đến một vị trí cụ thể trong cùng một trang web.
   ```html
   <a href="#section-id">`Go to Section</a>
   ```

- **Email**: Địa chỉ email.
   ```html
   <a href="mailto:example@example.com">`Email Us</a>
   ```

-  **Đường dẫn đến số điện thoại**: Sử dụng để gọi điện thoại từ trình duyệt.
   ```html
   <a href="tel:+123456789">`Call Us`</a>
   ```

-  **Javascript**: Được sử dụng để thực thi mã Javascript khi người dùng nhấp vào liên kết.
   ```html
   <a href="javascript:void(0);" onclick="myFunction()">`Click Me</a>
   ```

6. **Các thuộc tính thẻ**

- **`href`**: Chỉ định URL của trang đích mà liên kết sẽ điều hướng đến.

-  **`target`**: Xác định cách mở liên kết (ví dụ: `_blank` để mở trong cửa sổ/tab mới).

-  **`rel`**: Xác định mối quan hệ giữa trang hiện tại và trang được liên kết.

-  **`title`**: Cung cấp thông tin bổ sung khi di chuột qua liên kết.

-  **`download`**: Chỉ định rằng liên kết là để tải xuống tệp thay vì điều hướng.

- **`type`**: Xác định loại MIME của tài nguyên được liên kết.

- **`class`** và **`id`**: Để áp dụng CSS hoặc JavaScript.

- **`accesskey`**: Chỉ định phím tắt để kích hoạt liên kết.

- **`tabindex`**: Xác định thứ tự tab của liên kết.

# 7. chèn hình

1. **Lý Thuyết**

- Thẻ HTML `<img>`được sử dụng để nhúng hình ảnh vào trang web.
- Về mặt kỹ thuật, hình ảnh không được chèn vào trang web; hình ảnh được liên kết đến các trang web. Thẻ `<img>`tạo ra không gian lưu trữ cho hình ảnh được tham chiếu.
- Thẻ này `<img>`trống, chỉ chứa các thuộc tính và không có thẻ đóng.
- Thẻ này `<img>`có hai thuộc tính bắt buộc:
  + `src` - Chỉ định đường dẫn đến hình ảnh
  + `alt` - Chỉ định một văn bản thay thế cho hình ảnh

2. **Các Thuộc tính**

- **src** tính bắt buộc chỉ định đường dẫn (URL) đến hình ảnh.
- **alt** (thuộc tính bắt buộc)cung cấp văn bản thay thế cho hình ảnh nếu vì lý do nào đó người dùng không thể xem được hình ảnh (do kết nối chậm, lỗi trong thuộc tính src hoặc nếu người dùng sử dụng trình đọc màn hình).
- **width** sét chiều dài
- **height** sét chiều cao 
- Ngoài ra còn các thuộc tính cơ bản khác

3. **Cấu trúc**

```html
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```

# 8. chèn audio và video

1. **Các thuộc tính**

- **`src`**: Chỉ định URL của tệp âm thanh để phát lại.
- **`controls`**: Hiển thị các điều khiển phát nhạc như play, pause, và volume trên trình duyệt.
- **`autoplay`**: Tự động phát lại âm thanh khi trang web được tải lên.
- **`loop`**: Lặp lại phát lại âm thanh khi đến cuối.
- **`preload`**: Xác định cách mà trình duyệt nên tải dữ liệu âm thanh khi trang được tải lên.
- **`muted`**: Tắt tiếng của âm thanh.
- **`volume`**: Đặt âm lượng ban đầu của âm thanh (giá trị từ 0.0 đến 1.0).
- **`class`** và **`id`**: Để áp dụng CSS hoặc JavaScrips

2. **Lưu ý**

- Trình duyệt Chromium không cho phép phát tự động trong hầu hết các trường hợp. Tuy nhiên, phát tự động tắt tiếng luôn được phép.
- Thêm mutedafter autoplayđể cho phép tệp âm thanh của bạn tự động phát (nhưng tắt tiếng)

3. **Ví dụ audio**

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
```

3. **Vú dụ video**

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

# 9. khung Ifriame 

1. **Lý Thuyết**

- Iframe HTML được sử dụng để hiển thị một trang web trong một trang web khác.
- Thẻ HTML `<iframe>`chỉ định một khung nội tuyến
- Thuộc tính này src xác định URL của trang cần nhúng
- Luôn bao gồm một titlethuộc tính (cho trình đọc màn hình)
- Các thuộc tính heightvà widthchỉ định kích thước của iframe
- Sử dụng border:none;để xóa đường viền xung quanh iframe

2. **Ví dụ**

```html
<iframe src="https://www.w3schools.com/html/html_iframe.asp" style="border:2px solid red;" title="Iframe Example"></iframe>
```

# 10. from , input

 *Biểu mẫu HTML được sử dụng để thu thập dữ liệu đầu vào của người dùng. Dữ liệu đầu vào của người dùng thường được gửi đến máy chủ để xử lý.*

1. **Biểu mẫu `from`**

- Phần tử này `<form>`là nơi chứa các loại phần tử đầu vào khác nhau, chẳng hạn như: trường văn bản, hộp kiểm, nút radio, nút gửi, v.v.

```html
<from>
  <!-- item-->
</from>
```

### Các phần tử

1. **Phần tử `<input>`**

- Một trong những phần tử biểu mẫu được sử dụng nhiều nhất là `<input>`phần tử.
- Phần `<input>`tử có thể được hiển thị theo nhiều cách, tùy thuộc vào type thuộc tính

```html
<input type="text" id="fname" name="fname">
```

 **Các thuộc tính**

- **`type`**: Xác định kiểu đầu vào (ví dụ: text, password, email, number, checkbox, radio, submit, v.v.).

  + **`text`**: Trường đầu vào văn bản một dòng.
  + **`password`**: Trường đầu vào văn bản một dòng với các ký tự được che giấu.
  + **`email`**: Trường đầu vào cho địa chỉ email, kiểm tra định dạng email hợp lệ.
  + **`number`**: Trường đầu vào cho các giá trị số, có thể xác định các thuộc tính bổ sung như `min`, `max`, và `step`.
  + **`checkbox`**: Hộp kiểm cho phép người dùng chọn hoặc bỏ chọn một tùy chọn.
  + **`radio`**: Nút radio cho phép người dùng chọn một tùy chọn từ một nhóm.
  + **`file`**: Trường đầu vào cho phép người dùng chọn một hoặc nhiều tệp từ hệ thống tệp.
  + **`submit`**: Nút gửi biểu mẫu, kích hoạt sự kiện gửi biểu mẫu khi được nhấp.
  + **`reset`**: Nút đặt lại biểu mẫu, đặt lại tất cả các trường về giá trị mặc định của chúng.
  + **`button`**: Nút bấm chung, không có chức năng mặc định, thường được sử dụng với JavaScript để thực hiện hành động tùy chỉnh.
  
- **`name`**: Đặt tên cho trường đầu vào, được gửi cùng với biểu mẫu.
- **`value`**: Giá trị ban đầu của trường đầu vào.
- **`placeholder`**: Văn bản hiển thị mờ trong trường đầu vào cho đến khi người dùng nhập dữ liệu.
- **`required`**: Bắt buộc người dùng phải điền vào trường trước khi gửi biểu mẫu.
- **`readonly`**: Trường chỉ có thể đọc, không thể chỉnh sửa.
- **`disabled`**: Vô hiệu hóa trường đầu vào, không thể tương tác.
- **`maxlength`**: Giới hạn số ký tự tối đa có thể nhập vào trường.
- **`min`** và **`max`**: Xác định giá trị tối thiểu và tối đa cho các trường số hoặc ngày tháng.
- **`step`**: Xác định khoảng tăng cho các trường số hoặc ngày tháng.
- **`pattern`**: Biểu thức chính quy để kiểm tra giá trị đầu vào.
- **`autocomplete`**: Kích hoạt hoặc tắt tính năng tự động hoàn thành của trình duyệt.
- **`autofocus`**: Tự động đặt tiêu điểm vào trường đầu vào khi trang được tải.
- **`size`**: Đặt chiều rộng của trường đầu vào tính bằng số ký tự.
- **`list`**: Liên kết đến một thẻ `<datalist>` để cung cấp các tùy chọn tự động hoàn thành.
- **`minlength`**: Giới hạn số ký tự tối thiểu phải nhập vào trường.
- **`multiple`**: Cho phép chọn nhiều giá trị (dùng cho các kiểu file, email).
- **`form`**: Liên kết trường đầu vào với một biểu mẫu cụ thể.
- **`formaction`**: Ghi đè giá trị của thuộc tính `action` trong thẻ `<form>` khi sử dụng loại submit.
- **`formenctype`**: Xác định kiểu mã hóa của dữ liệu gửi đi (dùng cho loại submit).
- **`formmethod`**: Xác định phương thức gửi biểu mẫu (GET hoặc POST, dùng cho loại submit).
- **`formnovalidate`**: Tắt tính năng kiểm tra đầu vào trước khi gửi biểu mẫu (dùng cho loại submit).
- **`formtarget`**: Xác định nơi mở kết quả trả về (dùng cho loại submit).


2. **Phần tử** `<label>`

- Phần tử này `<label>`xác định nhãn cho một số phần tử biểu mẫu.

- Phần tử này `<label>`hữu ích cho người dùng trình đọc màn hình vì trình đọc màn hình sẽ đọc to nhãn khi người dùng tập trung vào phần tử đầu vào.

- Phần tử này `<label>`cũng giúp người dùng gặp khó khăn khi nhấp vào các vùng rất nhỏ (như nút radio hoặc hộp kiểm) - vì khi người dùng nhấp vào văn bản trong phần `<label>`tử, nút radio/hộp kiểm sẽ bật/tắt.

- Thuộc fortính của `<label>`thẻ phải bằng với thuộc idtính của `<input>` phần tử để liên kết chúng lại với nhau.

```html
<label for="cars">`Choose a car:</label>
```

3. **Phần tử** `<select>` 

- Phần tử này `<option>`xác định một tùy chọn có thể được chọn.
- Theo mặc định, mục đầu tiên trong danh sách thả xuống sẽ được chọn.
- Để xác định một tùy chọn được chọn trước, hãy thêm selectedthuộc tính vào tùy chọn

### Ví dụ

```html
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

# 11. CSS là gì?
```
- CSS là viết tắt của Cascading Style Sheets
- CSS mô tả cách các thành phần HTML được hiển thị trên màn hình, giấy hoặc trong các phương tiện truyền thông khác
- CSS tiết kiệm rất nhiều công sức. Nó có thể kiểm soát bố cục của nhiều trang web cùng một lúc
- Các bảng định kiểu bên ngoài được lưu trữ trong các tệp CSS
```

# 12. liên kết css với html

1. **CSS bên ngoài**

- Với bảng định dạng bên ngoài, bạn có thể thay đổi giao diện của toàn bộ trang web chỉ bằng cách thay đổi một tệp!
- Mỗi trang HTML phải bao gồm một tham chiếu đến tệp bảng định kiểu bên ngoài bên trong phần tử `<link>`, bên trong phần đầu.


**`index.html`**
```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

**`mystyle.css`**

```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

2. **CSS nội bộ**
 
- Có thể sử dụng bảng định kiểu nội bộ nếu một trang HTML duy nhất có một kiểu duy nhất.
- Kiểu nội bộ được định nghĩa bên trong phần tử `<style>`, bên trong phần đầu.

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
        body {
          background-color: linen;
        }
        
        h1 {
          color: maroon;
          margin-left: 40px;
        }
    </style>
  </head>
  <body>
  
      <h1>This is a heading</h1>
      <p>This is a paragraph.</p>
  
  </body>
</html>
```

3. **CSS nội tuyến**

- Có thể sử dụng kiểu nội tuyến để áp dụng kiểu duy nhất cho một phần tử duy nhất.

- Để sử dụng kiểu nội tuyến, hãy thêm thuộc tính style vào phần tử có liên quan. Thuộc tính style có thể chứa bất kỳ thuộc tính CSS nào.

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

4. **Thứ tự xếp tầng**

- Kiểu nào sẽ được sử dụng khi có nhiều hơn một kiểu được chỉ định cho một phần tử HTML?
- Tất cả các kiểu trong một trang sẽ "xếp tầng" thành một bảng kiểu "ảo" mới theo các quy tắc sau, trong đó quy tắc số một có mức độ ưu tiên cao nhất:
  + Kiểu nội tuyến (bên trong một phần tử HTML)
  + Các bảng định kiểu bên ngoài và bên trong (ở phần đầu)
  + Trình duyệt mặc định
- Vì vậy, kiểu nội tuyến có mức độ ưu tiên cao nhất và sẽ ghi đè lên các kiểu bên ngoài, bên trong và mặc định của trình duyệt.

# 13. Đơn vị trong css 

1. **Đơn vị tuyệt đối**:
   - **`px` (pixel)**: Đơn vị điểm ảnh, thường được sử dụng cho các kích thước cố định.
   - **`in` (inch)**: Đơn vị inch.
   - **`cm` (centimeter)**: Đơn vị centimet.
   - **`mm` (millimeter)**: Đơn vị milimet.
   - **`pt` (point)**: Đơn vị điểm, thường được sử dụng trong in ấn (1 pt = 1/72 inch).
   - **`pc` (pica)**: Đơn vị pica (1 pc = 12 pt).

2. **Đơn vị tương đối**:
   - **`%` (percent)**: Phần trăm, thường được sử dụng tương đối với kích thước phần tử chứa.
   - **`em`**: Đơn vị tương đối so với kích thước font của phần tử cha trực tiếp.
   - **`rem` (root em)**: Đơn vị tương đối so với kích thước font của phần tử gốc (thường là `<html>`).
   - **`vw` (viewport width)**: Phần trăm chiều rộng của viewport.
   - **`vh` (viewport height)**: Phần trăm chiều cao của viewport.
   - **`vmin`**: Phần trăm của kích thước nhỏ hơn giữa chiều rộng và chiều cao của viewport.
   - **`vmax`**: Phần trăm của kích thước lớn hơn giữa chiều rộng và chiều cao của viewport.

3. **Đơn vị thời gian**:
   - **`s` (second)**: Đơn vị giây.
   - **`ms` (millisecond)**: Đơn vị mili giây.

4. **Đơn vị góc**:
   - **`deg` (degree)**: Đơn vị độ (1 vòng tròn = 360 độ).
   - **`rad` (radian)**: Đơn vị radian (1 vòng tròn = 2π radian).
   - **`grad` (gradian)**: Đơn vị gradian (1 vòng tròn = 400 gradian).
   - **`turn`**: Đơn vị vòng (1 vòng tròn = 1 turn).

5. **Đơn vị độ dài không phải pixel**:
   - **`ch`**: Độ rộng của ký tự "0" trong font hiện tại.
   - **`ex`**: Chiều cao của ký tự "x" trong font hiện tại.
   - **`cap`**: Chiều cao của chữ in hoa trong font hiện tại.
   - **`ic`**: Độ rộng của chữ Hán trong font hiện tại (thường dùng cho chữ tượng hình).

# 14. Định dạng văn bản

1. **`color`**: Đặt màu chữ.
   ```css
   color: #333333;
   ```

2. **`font-size`**: Đặt kích thước chữ.
   ```css
   font-size: 16px;
   ```

3. **`font-family`**: Đặt kiểu chữ.
   ```css
   font-family: Arial, sans-serif;
   ```

4. **`font-weight`**: Đặt độ đậm của chữ.
   ```css
   font-weight: bold;
   ```

5. **`font-style`**: Đặt kiểu chữ in nghiêng hoặc thường.
   ```css
   font-style: italic;
   ```

6. **`text-align`**: Canh lề văn bản.
   ```css
   text-align: center;
   ```

7. **`text-decoration`**: Đặt các hiệu ứng trang trí cho văn bản như gạch chân, gạch ngang, v.v.
   ```css
   text-decoration: underline;
   ```

8. **`line-height`**: Đặt khoảng cách giữa các dòng.
   ```css
   line-height: 1.5;
   ```

9. **`letter-spacing`**: Đặt khoảng cách giữa các ký tự.
   ```css
   letter-spacing: 2px;
   ```

10. **`text-transform`**: Chuyển đổi kiểu chữ (viết hoa, viết thường, viết hoa chữ cái đầu).
    ```css
    text-transform: uppercase;
    ```

11. **`text-indent`**: Đặt khoảng cách thụt đầu dòng cho đoạn văn bản.
    ```css
    text-indent: 30px;
    ```

12. **`word-spacing`**: Đặt khoảng cách giữa các từ.
    ```css
    word-spacing: 5px;
    ```

13. **`white-space`**: Điều khiển cách xử lý khoảng trắng trong văn bản.
    ```css
    white-space: nowrap;
    ```

14. **`text-shadow`**: Thêm bóng đổ cho văn bản.
    ```css
    text-shadow: 2px 2px 5px rgba(0,0,0,0.3);
    ```

# 15. css selector ( bộ chọn )

1. **Bộ chọn phần tử (Element Selector)**:
   - Chọn tất cả các phần tử của một loại cụ thể.
   ```css
   p {
     color: blue;
   }
   ```

2. **Bộ chọn lớp (Class Selector)**:
   - Chọn tất cả các phần tử có thuộc tính `class` cụ thể.
   ```css
   .class-name {
     color: green;
   }
   ```

3. **Bộ chọn ID (ID Selector)**:
   - Chọn phần tử có thuộc tính `id` cụ thể.
   ```css
   #id-name {
     color: red;
   }
   ```

4. **Bộ chọn toàn bộ (Universal Selector)**:
   - Chọn tất cả các phần tử.
   ```css
   * {
     color: black;
   }
   ```

5. **Bộ chọn thuộc tính (Attribute Selector)**:
   - Chọn các phần tử dựa trên giá trị của thuộc tính.
   ```css
   a[href] {
     color: orange;
   }
   ```

6. **Bộ chọn nhóm (Group Selector)**:
   - Áp dụng cùng một kiểu cho nhiều bộ chọn.
   ```css
   h1, h2, h3 {
     color: purple;
   }
   ```

7. **Bộ chọn con (Child Selector)**:
   - Chọn các phần tử là con trực tiếp của một phần tử khác.
   ```css
   div >` p {
     color: pink;
   }
   ```

8. **Bộ chọn liền kề (Adjacent Sibling Selector)**:
   - Chọn phần tử ngay sau một phần tử khác.
   ```css
   h1 + p {
     color: brown;
   }
   ```

9. **Bộ chọn anh chị em (General Sibling Selector)**:
   - Chọn tất cả các phần tử là anh chị em của một phần tử khác.
   ```css
   h1 ~ p {
     color: yellow;
   }
   ```

10. **Bộ chọn con cháu (Descendant Selector)**:
    - Chọn tất cả các phần tử là con cháu của một phần tử khác.
    ```css
    div p {
      color: gray;
    }
    ```

# 16. khối trong css 

1. **Block elements (Phần tử khối)**:

   - **Chiếm toàn bộ chiều rộng có sẵn**: Phần tử khối chiếm toàn bộ chiều rộng của phần tử chứa nó.
   - **Bắt đầu trên một dòng mới**: Mỗi phần tử khối bắt đầu trên một dòng mới.
   - **Có thể chứa các phần tử block và inline**: Phần tử khối có thể chứa cả các phần tử khối và phần tử inline.
   - **Ví dụ**: `<div>`, `<p>`, `<h1>` đến `<h6>`, `<ul>`, `<ol>`, `<li>`, `<form>`, `<header>`, `<footer>`

2. **Inline elements (Phần tử nội tuyến)**:

   - **Chỉ chiếm không gian cần thiết**: Phần tử nội tuyến chỉ chiếm không gian cần thiết cho nội dung của nó.
   - **Không bắt đầu trên một dòng mới**: Các phần tử nội tuyến không bắt đầu trên một dòng mới mà hiển thị trên cùng một dòng với nội dung trước và sau nó.
   - **Chỉ chứa các phần tử inline khác và nội dung văn bản**: Phần tử nội tuyến không thể chứa các phần tử khối.
   - **Ví dụ**: `<span>`, `<a>`, `<img>`, `<strong>`, `<em>`, `<b>`, `<i>`, `<u>`

# 17. Css cho khối

### Giá trị chiều cao và chiều rộng của CSS
```
Trong CSS, bạn có thể đặt chiều cao (height) và chiều rộng (width) của các phần tử HTML bằng nhiều cách khác nhau, bao gồm sử dụng các giá trị tuyệt đối, tương đối, hoặc tự động. Dưới đây là các phương pháp và ví dụ minh họa:
```

1. **Giá trị tuyệt đối:**
   - Đặt chiều cao và chiều rộng cụ thể bằng các đơn vị như `px` (pixel), `em`, `rem`, `cm`, v.v.
   ```css
   .element {
     width: 300px;
     height: 200px;
   }
   ```

2. **Giá trị phần trăm:**
   - Đặt chiều cao và chiều rộng dựa trên phần trăm của kích thước của phần tử cha.
   ```css
   .element {
     width: 50%;
     height: 50%;
   }
   ```

3. **Giá trị tự động (auto):**
   - Cho phép trình duyệt tự động tính toán kích thước dựa trên nội dung hoặc phụ thuộc vào bố cục.
   ```css
   .element {
     width: auto;
     height: auto;
   }
   ```

4. **Giá trị tối đa và tối thiểu:**
   - Sử dụng `max-width`, `min-width`, `max-height`, và `min-height` để giới hạn các giá trị chiều rộng và chiều cao.
   ```css
   .element {
     max-width: 100%;
     min-height: 50px;
   }
   ```

5. **Giá trị inherit và initial:**
   - `inherit`: Kế thừa giá trị từ phần tử cha.
   - `initial`: Đặt giá trị về mặc định.
   ```css
   .element {
     width: inherit;
     height: initial;
   }
   ```

6. **Định dạng linh hoạt (flexible formatting):**
   - Sử dụng các thuộc tính của Flexbox (`display: flex`) hoặc Grid (`display: grid`) để quản lý các phần tử trong layout một cách linh hoạt hơn.
   ```css
   .container {
     display: flex;
     justify-content: space-between;
   }
   .element {
     flex: 1;
   }
   ```


### Background 

  1. **`background-color`**: Đặt màu nền cho phần tử.
     ```css
     .block {
       background-color: #f0f0f0; /* Màu xám nhạt */
     }
     ```
  
  2. **`background-image`**: Đặt hình ảnh nền cho phần tử.
     ```css
     .block {
       background-image: url('background.jpg');
     }
     ```
  
  3. **`background-repeat`**: Xác định cách lặp lại hình ảnh nền.
     - `repeat`: Lặp lại cả ngang và dọc.
     - `repeat-x`: Chỉ lặp lại ngang.
     - `repeat-y`: Chỉ lặp lại dọc.
     - `no-repeat`: Không lặp lại.
     ```css
     .block {
       background-image: url('background.jpg');
       background-repeat: repeat-x;
     }
     ```
  
  4. **`background-position`**: Đặt vị trí ban đầu của hình ảnh nền.
     - Các giá trị: `left top`, `center center`, `right bottom`, v.v.
     ```css
     .block {
       background-image: url('background.jpg');
       background-position: center center;
     }
     ```
  
  5. **`background-size`**: Đặt kích thước của hình ảnh nền.
     - `auto`: Kích thước mặc định.
     - `cover`: Phù hợp với phần lớn.
     - `contain`: Phù hợp với toàn bộ.
     - Các giá trị cụ thể như `100% auto`, `cover`, `contain`, v.v.
     ```css
     .block {
       background-image: url('background.jpg');
       background-size: cover;
     }
     ```
  
  6. **`background-attachment`**: Xác định liệu hình ảnh nền có cuộn cùng nội dung hay không.
     - `scroll`: Cuộn cùng nội dung.
     - `fixed`: Không cuộn.
     ```css
     .block {
       background-image: url('background.jpg');
       background-attachment: fixed;
     }
     ```
  
  7. **`background-clip`**: Xác định phạm vi sử dụng của hình ảnh nền và màu nền.
     - `border-box`: Màu nền và hình ảnh nền sẽ được hiển thị đầy đủ dưới đường viền của phần tử.
     - `padding-box`: Màu nền và hình ảnh nền chỉ được hiển thị trong vùng padding.
     - `content-box`: Màu nền và hình ảnh nền chỉ được hiển thị trong vùng nội dung.
     ```css
     .block {
       background-color: #f0f0f0;
       background-clip: padding-box;
     }
     ```
  8. **`viết tắt`**
  
     ```
     background: #ffffff url("img_tree.png") no-repeat right top;
     ```

### Border
  
1. **`border-width`**: Đặt độ dày của đường viền.
   - Giá trị: `thin`, `medium`, `thick`, hoặc số pixel (`px`).
   ```css
   .block {
     border-width: 2px;
   }
   ```

2. **`border-style`**: Đặt kiểu của đường viền.
   - Giá trị: `solid`, `dashed`, `dotted`, `double`, `groove`, `ridge`, `inset`, `outset`, `none`.
   ```css
   .block {
     border-style: dashed;
   }
   ```

3. **`border-color`**: Đặt màu sắc của đường viền.
   - Giá trị: Tên màu, mã màu, `transparent`.
   ```css
   .block {
     border-color: #ccc;
   }
   ```

4. **`border`**: Đặt đồng thời `border-width`, `border-style`, và `border-color`.
   - Các giá trị có thể được chỉ định theo thứ tự: `border-width`, `border-style`, `border-color`.
   ```css
   .block {
     border: 2px dashed #999;
   }
   ```

5. **`border-radius`**: Đặt độ cong của góc của đường viền.
   - Giá trị: Số pixel (`px`), hoặc `%` (tùy chọn).
   ```css
   .block {
     border-radius: 10px;
   }
   ```

6. **`border-collapse`**: Xác định cách viền của bảng được xử lý.
   - Giá trị: `separate` (mặc định) hoặc `collapse`.
   ```css
   table {
     border-collapse: collapse;
   }
   ```

7. **`border-spacing`**: Đặt khoảng cách giữa các ô trong bảng khi `border-collapse` là `separate`.
   - Giá trị: Số pixel (`px`).
   ```css
   table {
     border-spacing: 5px;
   }
   ```

8. **`border-image`**: Sử dụng hình ảnh làm đường viền thay vì đơn giản là màu sắc.
   - Cần sử dụng cú pháp phức tạp hơn, bao gồm URL hình ảnh và các giá trị khác như `slice`, `width`, `repeat`, v.v.
   ```css
   .block {
     border-image: url(border-image.png) 30 round;
   }
   ```
9. **`Viết tắt`** 
  ```
  .element {
  border: [border-width] [border-style] [border-color];
    }
  ```

### Margin

- Thuộc tính CSS marginđược sử dụng để tạo khoảng trống xung quanh các thành phần, bên ngoài bất kỳ đường viền nào được xác định.

- Với CSS, bạn có toàn quyền kiểm soát lề. Có các thuộc tính để thiết lập lề cho mỗi bên của một phần tử (trên, phải, dưới và trái).

1. **`margin-top`, `margin-right`, `margin-bottom`, `margin-left`**: Đặt khoảng cách từng cạnh của phần tử.
   - Các giá trị có thể là số pixel (`px`), phần trăm (`%`), `em`, `rem`, `auto`, v.v.
   ```css
   .element {
     margin-top: 10px;
     margin-right: 20px;
     margin-bottom: 15px;
     margin-left: 5px;
   }
   ```

2. **Viết tắt với một giá trị:**
   - Nếu bạn chỉ định một giá trị, nó sẽ áp dụng cho cả bốn cạnh theo thứ tự: `top`, `right`, `bottom`, `left`.
   ```css
   .element {
     margin: 10px; /* Áp dụng 10px cho cả bốn cạnh */
   }
   ```

3. **Viết tắt với hai giá trị:**
   - Nếu bạn chỉ định hai giá trị, chúng sẽ áp dụng cho các cạnh ngang (`top`, `bottom`) và các cạnh dọc (`left`, `right`) theo thứ tự.
   ```css
   .element {
     margin: 10px 20px; /* 10px cho top và bottom, 20px cho left và right */
   }
   ```

4. **Viết tắt với ba giá trị:**
   - Ba giá trị sẽ áp dụng lần lượt cho `top`, `right/left` và `bottom`.
   ```css
   .element {
     margin: 10px 20px 15px; /* 10px cho top, 20px cho left và right, 15px cho bottom */
   }
   ```

5. **Viết tắt với bốn giá trị:**
   - Chỉ định cụ thể từng cạnh theo thứ tự: `top`, `right`, `bottom`, `left`.
   ```css
   .element {
     margin: 10px 20px 15px 5px; /* 10px cho top, 20px cho right, 15px cho bottom, 5px cho left */
   }
   ```

6. **Giá trị `auto`**: 
   - Các giá trị `margin` có thể được đặt thành `auto` để tự động điều chỉnh khoảng cách, chẳng hạn như canh giữa một phần tử trong container.
   ```css
   .element {
     margin-left: auto;
     margin-right: auto;
   }
   ```

### Padding

- Thuộc tính CSS paddingđược sử dụng để tạo khoảng trống xung quanh nội dung của phần tử, bên trong bất kỳ đường viền nào được xác định.

- Với CSS, bạn có toàn quyền kiểm soát phần đệm. Có các thuộc tính để thiết lập phần đệm cho mỗi bên của phần tử (trên, phải, dưới và trái).

1. **`padding-top`, `padding-right`, `padding-bottom`, `padding-left`**: Đặt khoảng đệm từng cạnh của phần tử.
   - Các giá trị có thể là số pixel (`px`), phần trăm (`%`), `em`, `rem`, v.v.
   ```css
   .element {
     padding-top: 10px;
     padding-right: 20px;
     padding-bottom: 15px;
     padding-left: 5px;
   }
   ```

2. **Viết tắt với một giá trị:**
   - Nếu bạn chỉ định một giá trị, nó sẽ áp dụng cho cả bốn cạnh theo thứ tự: `top`, `right`, `bottom`, `left`.
   ```css
   .element {
     padding: 10px; /* Áp dụng 10px cho cả bốn cạnh */
   }
   ```

3. **Viết tắt với hai giá trị:**
   - Nếu bạn chỉ định hai giá trị, chúng sẽ áp dụng cho các cạnh ngang (`top`, `bottom`) và các cạnh dọc (`left`, `right`) theo thứ tự.
   ```css
   .element {
     padding: 10px 20px; /* 10px cho top và bottom, 20px cho left và right */
   }
   ```

4. **Viết tắt với ba giá trị:**
   - Ba giá trị sẽ áp dụng lần lượt cho `top`, `right/left` và `bottom`.
   ```css
   .element {
     padding: 10px 20px 15px; /* 10px cho top, 20px cho left và right, 15px cho bottom */
   }
   ```

5. **Viết tắt với bốn giá trị:**
   - Chỉ định cụ thể từng cạnh theo thứ tự: `top`, `right`, `bottom`, `left`.
   ```css
   .element {
     padding: 10px 20px 15px 5px; /* 10px cho top, 20px cho right, 15px cho bottom, 5px cho left */
   }
   ```

# 18. Pseudo-classes

**Lớp giả là gì?**

- Lớp giả được sử dụng để xác định trạng thái đặc biệt của một phần tử.
- Ví dụ, nó có thể được sử dụng để:
  + Tạo kiểu cho một phần tử khi người dùng di chuột qua nó
  + Kiểu liên kết đã truy cập và chưa truy cập khác nhau
  + Tạo kiểu cho một phần tử khi nó được chú ý

1. **`:hover`**: Áp dụng kiểu khi phần tử được "hover" bởi con trỏ chuột.
   ```css
   a:hover {
     color: red;
   }
   ```

2. **`:active`**: Áp dụng kiểu khi phần tử đang được kích hoạt (ví dụ nhấp chuột lên nút).
   ```css
   button:active {
     background-color: #ccc;
   }
   ```

3. **`:focus`**: Áp dụng kiểu khi phần tử đang được trọng tâm hoặc tập trung vào (thường sử dụng cho các phần tử có thể tương tác bằng bàn phím như input).
   ```css
   input:focus {
     border: 2px solid blue;
   }
   ```

4. **`:first-child`**: Áp dụng kiểu cho phần tử là con đầu tiên của phần tử cha.
   ```css
   li:first-child {
     font-weight: bold;
   }
   ```

5. **`:last-child`**: Áp dụng kiểu cho phần tử là con cuối cùng của phần tử cha.
   ```css
   li:last-child {
     margin-bottom: 0;
   }
   ```

6. **`:nth-child()`**: Áp dụng kiểu cho các phần tử là con thứ n trong phần tử cha, với một số lượng các cách sử dụng khác nhau, ví dụ như `nth-child(odd)`, `nth-child(even)`, `nth-child(3n+1)`.
   ```css
   tr:nth-child(even) {
     background-color: #f2f2f2;
   }
   ```

7. **`:nth-of-type()`**: Áp dụng kiểu cho các phần tử là con thứ n của một loại phần tử cụ thể trong phần tử cha.
   ```css
   div:nth-of-type(2n) {
     background-color: lightblue;
   }
   ```

8. **`:nth-last-child()`**: Tương tự như `nth-child()`, nhưng tính từ cuối danh sách con.
   ```css
   li:nth-last-child(2) {
     color: red;
   }
   ```

9. **`:nth-last-of-type()`**: Tương tự như `nth-of-type()`, nhưng tính từ cuối danh sách con.
   ```css
   p:nth-last-of-type(2) {
     font-style: italic;
   }
   ```

10. **`:not()`**: Loại trừ các phần tử khỏi lựa chọn.
    ```css
    p:not(.special) {
      color: gray;
    }
    ```

# 19. Pseudo-Elements

**Phần tử giả là gì?**

- Phần tử giả CSS được sử dụng để định kiểu cho các phần được chỉ định của một phần tử.
- Ví dụ, nó có thể được sử dụng để:
  + Định dạng chữ cái đầu tiên hoặc dòng đầu tiên của một phần tử
  + Chèn nội dung trước hoặc sau nội dung của một phần tử

1. **`::before`**: Tạo một phần tử ảo trước nội dung của phần tử được chọn.
   ```css
   .element::before {
     content: "Trước nội dung: ";
     font-weight: bold;
   }
   ```

2. **`::after`**: Tạo một phần tử ảo sau nội dung của phần tử được chọn.
   ```css
   .element::after {
     content: " - Sau nội dung";
     color: #999;
   }
   ```

3. **`::first-line`**: Chọn và tùy chỉnh dòng đầu tiên của phần tử văn bản.
   ```css
   p::first-line {
     font-weight: bold;
     font-size: 120%;
   }
   ```

4. **`::first-letter`**: Chọn và tùy chỉnh ký tự đầu tiên của phần tử văn bản.
   ```css
     font-size: 150%;
     color: #cc0000;
   }
   ```

5. **`::selection`**: Tùy chỉnh phần được chọn bởi người dùng trên trang.
   ```css
   ::selection {
     background-color: yellow;
     color: black;
   }
   ```

6. **`::placeholder`**: Tùy chỉnh phong cách của placeholder trong các trường nhập liệu.
   ```css
   input::placeholder {
     color: #999;
     font-style: italic;
   }
   ```

7. **`::marker`**: Tùy chỉnh các đánh dấu (marker) của các mục danh sách.
   ```css
   ul::marker {
     color: blue;
     font-weight: bold;
   }
   ```

8. **`::backdrop`**: Được sử dụng để tạo các hiệu ứng mờ nền khi sử dụng các lớp backdrop-filter CSS3.
   ```css
   .backdrop-example::backdrop {
     backdrop-filter: blur(5px);
   }
   ```
