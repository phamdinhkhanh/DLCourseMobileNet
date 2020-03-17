# Chạy project git:
* **Bước 1:** Clone git vào máy tính:

`git clone https://github.com/phamdinhkhanh/DLCourseMobileNet.git`

* **Bước 2:** Mở chrome dưới chế độ disable security.

`start chrome --user-data-dir="C:/Chrome dev session" --disable-web-security`


* **Bước 3:** Mở file index.html từ cửa sổ chrome ở bước 2.


# Các bước deploy model tensorflow js:

* **Bước 1**: Huấn luyện mô hình trên tensorflow và lưu vào local folder.

* **Bước 2**: Convert tensorflow model thành tensorflow js model.

`tensorflowjs_converter --input_format=keras /tmp/model.h5 /tmp/tfjs_model` 

* **Bước 3**:Upload folder model tensorflow js vừa train ở bước 2 lên một git project.

* **Bước 4**: Vào file `js/mobile-net.js` điều chỉnh lại đường link load folder dòng 11 trỏ tới file js.

* **Bước 5**: Disable security

`start chrome --user-data-dir="C:/Chrome dev session" --disable-web-security`

* **Bước 6**: Mở file index.html trên cửa số google chrome.