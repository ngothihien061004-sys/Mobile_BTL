# MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419 <br>
## BÀI TẬP LỚN:<br>
I. Viết phần mềm trên công cụ Mit App inventor:<br>
   - Khởi tạo dự án:<br>
   <img width="1911" height="999" alt="image" src="https://github.com/user-attachments/assets/18a4802e-5bc3-4600-88d7-35ff845fb435" /><br>
- Thêm 2 Screen:<br>
  <img width="287" height="277" alt="image" src="https://github.com/user-attachments/assets/ef299620-000d-4e76-ad7a-b3caefe8629c" /><br>
- Cấu hình Screen1 bằng giao diện đồ họa: about về bản thân+nút gọi sang 2 screen còn lại<br>
  + Sử dụng các thanh công cụ trong User Interface để cấu hình giao diện:<br>
  + Kéo thanh label vào màn hình và sử đổi phần text trong cột Properties thành nôi dung muốn hiển thị, button để chuyển sang screen khác<br>
    <img width="1754" height="942" alt="image" src="https://github.com/user-attachments/assets/60476299-65b0-44bb-ae73-c5b6f8d8fa84" />
<br>

- Cấu hình Screen2 bằng giao diện đồ họa( giải bài toán đơn giản)<br>
  + Tiếp tục sử dụng các thanh label để hiển thị, button để thực hiện tính toán, textbox để nhập giá trị<br>
  <img width="1765" height="922" alt="image" src="https://github.com/user-attachments/assets/1a3cfa14-b8c9-42fc-8fd0-cd8f3dc26fee" />

- Cấu hình Screen3 bằng giao diện đồ họa( truy cập webview có sẵn)<br>
  + Thêm công cụ web view vào screen3<br>
  + Dán url trang web vào HomeUrl<br>
    <img width="1914" height="995" alt="image" src="https://github.com/user-attachments/assets/78ae8cbc-aaa8-42de-b0b7-d9739ec5b654" /><br>
    <img width="1907" height="937" alt="image" src="https://github.com/user-attachments/assets/d53e458b-a2af-4e41-bf07-6b57c7641b45" />
<br>


- Cấu hình Screen1 bằng block để xử lí logic:<br>
  + Chọn 2 khối điều kiện When button click do open another screen:<br>
    <img width="912" height="158" alt="image" src="https://github.com/user-attachments/assets/2b83eb9b-7a8b-4eab-a572-eb9ea7df21c5" />
<br>
- Cấu hình Screen2 bằng block:<br>
<img width="782" height="165" alt="image" src="https://github.com/user-attachments/assets/36e151b0-ce54-4a71-9db1-fa545c3292c5" />
<br>

  - Screen3 không cần cấu hình gì thêm vì đã thêm url rồi<br>
 
  - Kết nối tới Mitt App APK trêm điện thoại để test:<br>
    
   <img width="1290" height="2796" alt="image" src="https://github.com/user-attachments/assets/435873b4-ec85-48ea-858a-4abf5466d674" />
<br>
<img width="1290" height="2796" alt="image" src="https://github.com/user-attachments/assets/55e33e7a-670c-46a1-a435-480c8de86d0a" />
<br>
<img width="1290" height="2796" alt="image" src="https://github.com/user-attachments/assets/2821749d-3cc0-42d0-9575-d6fe868b55d6" />

<br>


  - Bản chất của việc kéo thả Block<br>

Trong MIT App Inventor, lập trình được thực hiện bằng cách kéo và ghép các khối lệnh (Blocks) thay vì viết mã nguồn bằng ngôn ngữ lập trình. Mỗi block đại diện cho một câu lệnh, điều kiện, phép toán hoặc sự kiện. Khi ghép các block lại với nhau, ta tạo thành logic hoạt động của chương trình.<br>

a. Ưu điểm so với viết code<br>
- Dễ học và dễ sử dụng cho người mới bắt đầu.<br>
- Hạn chế lỗi cú pháp vì các block chỉ ghép được theo cấu trúc hợp lệ.<br>
- Trực quan, dễ quan sát luồng xử lý của chương trình.<br>
- Tăng tốc độ phát triển các ứng dụng đơn giản.<br>
- Phù hợp cho việc học tư duy lập trình và phát triển ứng dụng nhanh.<br>
b. Nhược điểm<br>
- Khó xây dựng các ứng dụng lớn và phức tạp.<br>
- Khi chương trình nhiều chức năng, số lượng block lớn sẽ gây rối và khó quản lý.<br>
- Ít linh hoạt hơn so với các ngôn ngữ lập trình truyền thống như Java, Python, Kotlin.<br>
- Khả năng tối ưu và mở rộng bị hạn chế.<br>
- Khó tích hợp các thư viện hoặc chức năng nâng cao.<br>
                  
II. Viết app sử dụng Android Studio<br>
   # 1. AndroidManifest.xml là gì?<br>

`AndroidManifest.xml` là file cấu hình trung tâm của ứng dụng Android.<br>

Nó dùng để mô tả:<br>

- Tên package của ứng dụng.<br>
- Các Activity, Service, Broadcast Receiver.<br>
- Các quyền (Permission) ứng dụng cần sử dụng.<br>
- Phiên bản Android hỗ trợ.<br>
- Icon, Theme, Launcher Activity,...<br>

## Khai báo quyền<br>

Ví dụ quyền Internet:<br>

```xml
<uses-permission android:name="android.permission.INTERNET"/>
```

Ví dụ quyền vị trí:<br>

```xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
```

## Mục đích<br>

Android sử dụng Manifest để:<br>

- Xác định cấu trúc ứng dụng.<br>
- Kiểm soát bảo mật.<br>
- Cấp phát quyền truy cập tài nguyên hệ thống.<br>


# 2. Vòng đời của Activity Android<br>

```text
onCreate()
↓
onStart()
↓
onResume()
↓
(Ứng dụng hoạt động)

↓
onPause()
↓
onStop()

↓
onRestart()
↓
onStart()
↓
onResume()

hoặc

onDestroy()
```

## Ý nghĩa các hàm<br>

### onCreate()<br>

Được gọi khi Activity được tạo lần đầu.<br>

Thường dùng để:<br>

- Nạp giao diện.<br>
- Khởi tạo biến.<br>
- Khởi tạo dữ liệu.<br>

### onStart()<br>

Activity bắt đầu hiển thị.<br>

### onResume()<br>

Activity ở trạng thái tương tác với người dùng.<br>

### onPause()<br>

Activity bị che một phần hoặc mất focus.<br>

### onStop()<br>

Activity không còn hiển thị.<br>

### onDestroy()<br>

Activity bị hủy hoàn toàn.<br>

# 3. Tại sao Android Studio sinh sẵn hàm onCreate()?<br>

Android Framework tự động gọi `onCreate()` khi Activity được tạo.<br>

Do hầu hết ứng dụng đều cần:<br>

- Nạp giao diện.<br>
- Khởi tạo dữ liệu.<br>

nên Android Studio tạo sẵn:<br>

```java
@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
```
# 4. Kiểm tra quyền trong Android<br>

Từ Android 6.0 trở lên phải kiểm tra Runtime Permission.<br>

Ví dụ kiểm tra quyền Camera:<br>

```java
if (ContextCompat.checkSelfPermission(
        this,
        Manifest.permission.CAMERA)
        != PackageManager.PERMISSION_GRANTED) {

    ActivityCompat.requestPermissions(
            this,
            new String[]{Manifest.permission.CAMERA},
            100);
}
```

## Ý nghĩa<br>

### checkSelfPermission()<br>

Kiểm tra ứng dụng đã được cấp quyền hay chưa.<br>

### requestPermissions()<br>

Hiển thị hộp thoại yêu cầu người dùng cấp quyền.<br>


# 5. Giao diện Android<br>

Giao diện được mô tả bằng file XML nằm trong:<br>

```text
res/layout
```

Ví dụ:<br>

```xml
<TextView
    android:id="@+id/txtName"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"/>
```

# 6. Tránh Hardcode Text<br>

Không nên:<br>

```xml
android:text="Xin chào"
```

Nên lưu trong:<br>

```text
res/values/strings.xml
```

Ví dụ:<br>

```xml
<string name="hello">Xin chào</string>
```

Sử dụng:<br>

```xml
android:text="@string/hello"
```

# 7. Cú pháp tham chiếu tài nguyên<br>

## String<br>

```xml
@string/hello
```

## Color<br>

```xml
@color/primary
```

## Drawable<br>

```xml
@drawable/logo
```

## Dimension<br>

```xml
@dimen/text_size
```

# 8. Ưu điểm của việc tham chiếu tài nguyên<br>

- Dễ bảo trì.<br>
- Tránh lặp dữ liệu.<br>
- Hỗ trợ đa ngôn ngữ.<br>
- Hỗ trợ nhiều giao diện.<br>
- Dễ thay đổi nội dung tập trung.<br>

# 9. Android tự động chọn tài nguyên theo Language, Location, Theme<br>

Ví dụ:<br>

```text
values/
values-vi/
values-en/
```

Android sẽ tự động chọn:<br>

- values-vi → khi máy dùng tiếng Việt.<br>
- values-en → khi máy dùng tiếng Anh.<br>

Ví dụ Dark Mode:<br>

```text
values/
values-night/
```

Android sẽ tự động chọn giao diện phù hợp.<br>


# 10. Lợi ích của việc tự động chọn tài nguyên<br>

Ứng dụng có thể:<br>

- Tự đổi ngôn ngữ.<br>
- Tự đổi giao diện sáng/tối.<br>
- Tự thay đổi tài nguyên theo cấu hình thiết bị.<br>
- Hỗ trợ quốc tế hóa (Internationalization).<br>

# 11. Đối tượng chứa (Layout Container)<br>

Layout là đối tượng dùng để chứa và sắp xếp các View con.<br>

Ví dụ:<br>

- LinearLayout<br>
- RelativeLayout<br>
- ConstraintLayout<br>
- FrameLayout<br>

# 12. LinearLayout<br>

## Sắp xếp theo chiều dọc<br>

```xml
android:orientation="vertical"
```

Ví dụ:<br>

```text
Button
TextView
EditText
```

## Sắp xếp theo chiều ngang<br>

```xml
android:orientation="horizontal"
```

Ví dụ:<br>

```text
Button Button Button
```

# 13. Gravity<br>

Gravity quy định vị trí hiển thị của các View bên trong Layout.<br>

Ví dụ:<br>

```xml
android:gravity="center"
```

Các giá trị phổ biến:<br>

```text
center
left
right
top
bottom
center_horizontal
center_vertical
```

# 14. Code tương tác với Layout<br>

Ví dụ lấy TextView:<br>

```java
TextView txt = findViewById(R.id.txtName);
```

Hiển thị nội dung:<br>

```java
txt.setText(R.string.hello);
```

# 15. Tại sao dùng R.string thay vì Hardcode?<br>

Không nên:<br>

```java
txt.setText("Xin chào");
```

Nên:<br>

```java
txt.setText(R.string.hello);
```

Vì Android sẽ tự động lấy:<br>

- Ngôn ngữ phù hợp.<br>
- Theme phù hợp.<br>
- Tài nguyên phù hợp với thiết bị.<br>


# 16. Event là gì?<br>

Event là các sự kiện do người dùng tác động vào ứng dụng.<br>

Ví dụ:<br>

- Click Button.<br>
- Click TextView.<br>
- Chạm màn hình.<br>
- Nhập dữ liệu.<br>
- Vuốt màn hình.<br>


# 17. Layout cần làm gì để xử lý Event?<br>

Cần khai báo ID cho View:<br>

```xml
<Button
    android:id="@+id/btnSubmit"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"/>
```

Sau đó code Java có thể truy cập View bằng:<br>

```java
findViewById(R.id.btnSubmit);
```

# 18. Xử lý Event - Cách 1: Listener trong Java<br>

```java
Button btn = findViewById(R.id.btnSubmit);

btn.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        // xử lý sự kiện
    }
});
```

## Ưu điểm<br>

- Phổ biến nhất.<br>
- Dễ quản lý.<br>
- Phù hợp dự án lớn.<br>

# 19. Xử lý Event - Cách 2: Khai báo trực tiếp trong XML<br>

## XML<br>

```xml
<Button
    android:onClick="submitData"/>
```

## Java<br>

```java
public void submitData(View view) {
    // xử lý sự kiện
}
```

## Ưu điểm<br>

- Viết nhanh.<br>
- Phù hợp ứng dụng nhỏ.<br>

## Nhược điểm<br>

- Khó quản lý khi dự án lớn.<br>
- Không linh hoạt bằng Listener.<br>
     trong app có các thư mục đặc biệt: Assets<br>
     khi sử dụng Window Explorer để copy các files + folder vào trong Assets<br>
     thì khi compiler: mọi file này đều đi theo app, nằm trong app<br>
     trong app có thể truy cập được đến các file này<br>
     cú pháp truy cập vào là gì?<br>
     lợi ích của việc app có sẵn các files (offline cũng có)?<br>
     ứng dụng: app hướng dẫn việc X<br>


III. Cài đặt app:<br>
A. App1:<br>
ĐẶT VẤN ĐỀ & ĐỀ XUẤT GIẢI QUYẾT<br>
1. Vấn đề đặt ra<br>
Khi xây dựng một ứng dụng cung cấp thông tin tiểu sử và bảng xếp hạng ca sĩ, nếu phụ thuộc hoàn toàn vào API/Internet, ứng dụng sẽ có độ trễ khi tải và không thể hoạt động offline. Tuy nhiên, nếu lưu toàn bộ thông tin thô (như tiểu sử dài hàng nghìn từ) trực tiếp vào cơ sở dữ liệu SQLite hoặc mã cứng (hardcode) trong Java, file cài đặt sẽ rất nặng và khó quản lý cấu trúc văn bản.<br>

2. Giải pháp giải quyết<br>
Lưu trữ: Sử dụng một file singers.json đặt trong thư mục assets đóng vai trò là một "Local Database" tĩnh, lưu giữ thông tin cốt lõi (Tên, Thể loại, Số cúp, Đường dẫn file tiểu sử chi tiết). Các file tiểu sử dài được tách riêng thành các file .txt hoặc .html độc lập nằm trong cụm thư mục assets/bios/.<br>

Xử lý (Thuật toán): Đọc luồng dữ liệu (InputStream), phân tích chuỗi JSON (JSON Parsing). Triển khai thêm Thuật toán sắp xếp nhanh (Quick Sort) hoặc sử dụng Collections.sort() để tự động sắp xếp thứ hạng ca sĩ theo Số lượng cúp/giải thưởng giảm dần ngay khi ứng dụng vừa khởi chạy, đảm bảo tính động thay vì sắp xếp thủ công bằng tay trong file JSON.<br>

Hiển thị: Sử dụng RecyclerView kết hợp CardView ở màn hình chính để tối ưu hiệu năng cuộn danh sách lớn. Khi ấn vào một ca sĩ, ứng dụng mở màn hình chi tiết và dùng NestedScrollView kết hợp TextView (hoặc WebView) để nạp file tiểu sử offline tương ứng từ assets.<br>
- Các bước thực hiện:<br>
Bước 1: Khởi tạo cấu trúc thư mục Assets tĩnhMặc định khi tạo dự án mới, Android Studio không sinh sẵn thư mục assets. Bạn cần khởi tạo thủ công:<br>
Click chuột phải vào thư mục app (hoặc main) ---> New ---> Folder ---> Assets Folder ---> Nhấn Finish.<br>
Tại thư mục assets vừa xuất hiện, click chuột phải ---> New ---> Directory ---> Đặt tên là bios.<br>
Tạo file cấu hình chính: Click chuột phải vào assets ---> New ---> File ---> Đặt tên là singers.json và dán nội dung định dạng JSON (gồm id, tên, thể loại, số cúp, đường dẫn file).<br>
<img width="496" height="585" alt="image" src="https://github.com/user-attachments/assets/740f7423-5a09-4f4b-8c59-211c769f79bc" /><br>

Tạo các file nội dung: Click chuột phải vào thư mục bios ---> New ---> File ---> Tạo các file văn bản thô như son_tung.txt, den_vau.txt chứa nội dung tiểu sử chi tiết.<br>
<img width="430" height="224" alt="image" src="https://github.com/user-attachments/assets/d42d468d-57ee-4d3d-983f-ce68ff760145" /><br>
Bước 2: Định nghĩa lớp dữ liệu và thiết kế giao diện (UI):<br>
1. Tạo Java Class Singer.java<br>
   <img width="954" height="762" alt="image" src="https://github.com/user-attachments/assets/c5021b45-e494-4a8b-915b-5c24210ab84a" /><br>

2. Thiết kế giao diện dòng đơn item_singer.xml<br>
   <img width="960" height="760" alt="image" src="https://github.com/user-attachments/assets/37b65389-b73a-4a24-b9d0-265ac2a339a1" /><br>
3. Thiết kế giao diện chính activity_main.xml<br>
  <img width="947" height="659" alt="image" src="https://github.com/user-attachments/assets/b4559c39-d380-4926-b4fa-b8bec8e0136f" /><br>
4. Thiết kế giao diện chi tiết activity_detail.xml<br>
   <img width="949" height="841" alt="image" src="https://github.com/user-attachments/assets/6c6b4eaf-d78e-4970-828d-f59c547601cc" /><br>

BƯỚC 3: Cài đặt app và kiểm thử:<br>
<img width="558" height="812" alt="image" src="https://github.com/user-attachments/assets/6c4a728b-2e16-4388-9e02-95294545539b" /><br>
<img width="552" height="956" alt="image" src="https://github.com/user-attachments/assets/d86dfc30-c1ab-471a-aa89-aa7d9c7c330b" /><br>
<img width="552" height="941" alt="image" src="https://github.com/user-attachments/assets/c04f4670-f8ae-4642-8e9f-c8c1d1cb0c0f" /><br>


B. App2:<br>
- Bước 1: Khởi tạo dự án mới:<br>
  <img width="982" height="797" alt="image" src="https://github.com/user-attachments/assets/749dd4e7-beb2-4e19-bc8a-39cafe0e4848" /><br>

- Bước 2: Cấp quyền Internet (AndroidManifest.xml)<br>
   <img width="895" height="687" alt="image" src="https://github.com/user-attachments/assets/93e7d885-d1a5-4d2a-883f-f59f93f6362a" /><br>

- Bước 3: Thiết kế Giao diện (XML):<br>
  1. Activity 1: Giới thiệu bản thân (activity_main.xml)<br>
     Giao diện gồm thông tin cá nhân và 2 nút để chuyển sang Activity 2 và Activity 3.<br>
  <img width="810" height="579" alt="image" src="https://github.com/user-attachments/assets/9869d76a-35f0-4c3d-9cd6-4d017b93db7a" />
<br>

   2. Activity 2: Giải toán + Gọi API (activity_math.xml)<br>
      Click chuột phải vào thư mục layout --> New --> Layout Resource File--> Đặt tên là activity_math.<br>
<img width="412" height="284" alt="image" src="https://github.com/user-attachments/assets/6c18aef4-5f7f-46f2-a36b-affb35b24190" /><br>
<img width="888" height="763" alt="image" src="https://github.com/user-attachments/assets/f4d30634-b7cd-47ae-b440-16328b3ac64f" /><br>
   3. Activity 3: WebView hiển thị trang web (activity_web.xml):<br>
      <img width="827" height="451" alt="image" src="https://github.com/user-attachments/assets/6ec97fa6-b2ba-4d01-a886-51acb157e7eb" /><br>

- Bước 4: Viết Logic xử lý (Java):<br>
  1. MainActivity.java (Điều hướng):<br>
     <img width="860" height="594" alt="image" src="https://github.com/user-attachments/assets/7c97cfd6-b411-4d73-bf76-41c2ce32321a" /><br>
2. MathActivity.java:<br>
   <img width="864" height="598" alt="image" src="https://github.com/user-attachments/assets/a11d2ea9-e924-47f1-93ac-ed9575e24953" /><br>
3. WebActivity.java (WebView truy cập URL định danh mã sinh viên)<br>
   <img width="849" height="586" alt="image" src="https://github.com/user-attachments/assets/dad8205f-5c49-431a-b261-6121cb9b4d54" />
<br>

- Bước 5: Khai báo Activity mới trong AndroidManifest.xml<br>
<img width="854" height="801" alt="image" src="https://github.com/user-attachments/assets/df3105d3-80b0-4203-a7ca-40ea9f9f764c" /><br>

- Bước 6: Tiến hành build và kiểm thử<br>
  
+ Acivity1:<br>
 <img width="555" height="880" alt="image" src="https://github.com/user-attachments/assets/faf7dc94-5f5d-4589-9e61-dfb4643fd035" />
<br>
+ Activity2:<br>
  <img width="554" height="691" alt="image" src="https://github.com/user-attachments/assets/51eaf90a-671b-4ea7-926b-55b33d6b2a9f" />
<br>
+ Activity3:<br>
  <img width="557" height="287" alt="image" src="https://github.com/user-attachments/assets/948c90a3-b703-4991-bec5-d2e6e57537a4" />
<br>

