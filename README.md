# Detecting-facial-features-with-Python-language---opencv-and-numpy-library
Detecting facial features with Python language - opencv and numpy library
ارائه شده توسط محمد مهدی خدادوست - سید محمد حسین دهقان منشادی
با سلام و خسته نباشید
این فایل پروژه مربوط به تشخیص اجزای صورت با زبان پایتون می باشد
قبل از کار با این نرم افزارر باید چند نکته را در نظر داشته باشید.
1- ابتدا باید با دستور 
pip install opencv 
باید کتابخانه opencv را در cmd ویتدوز نصب کنید در صورتی که در نصب دچار خطا شدید باید ابتدا با دستور py -0 نسحه پایتون را خود را بررسی کرده و  فایل زیپ Dlib-library-Installation-main را استخراج کرده فایل مرتبط با نسخه پایتون خود را پیدا کنید مثلا برای پایتون با نسخه 3.9 باید از فایل dlib-19.22.1-cp39-cp39-win_amd64.whl استفاده کنید درباره نحوه استفاده از فایل به این صورت است که این فایل را در مکانی مثلا دستکتاپ قرار داده و وارد cmd ویندوز شده و باید وارد فولدر desktop بشویم برای نصب کتابخانه opencv مرتبط با نسخه پایتون دستور زیر را وارد می کنیم مثلا برای نصب نسخه 3.9 :
pip install dlib-19.22.1-cp39-cp39-win_amd64.whl
2- نصب کتابخانه numpy:
pip intall numpy
3- شناسایی فایل های مربوط به تشخیص چهره،چشم،لبخند:
برای تشخیص محل نصب پایتون دستور زیر را در cmd ویندوز وارد کنیم:
where python
وارد مسیر نصب پایتون شده و وارد مسیر زیر می شویم تا به محتویات کتابخانه opencv دسترسی پیدا کنیم:
\Python39\Lib\site-packages\cv2\data
و سه تا فایل  haarcascade_smile.xml  haarcascade_frontalface_default.xml   haarcascade_eye.xml در فایل پروژه قرار می دهیم با استفاده از کد های زیر
face_cascade = cv.CascadeClassifier('C:\\Users\\mohammad\\AppData\\Local\\Programs\\Python\\Python39\\Lib\\site-packages\\cv2\\data\\haarcascade_frontalface_default.xml')
eye_cascade = cv.CascadeClassifier('C:\\Users\\mohammad\\AppData\\Local\\Programs\\Python\\Python39\\Lib\\site-packages\\cv2\\data\\haarcascade_eye.xml')
smile_cascade = cv.CascadeClassifier('C:\\Users\\mohammad\\AppData\\Local\\Programs\\Python\\Python39\\Lib\\site-packages\\cv2\\data\\haarcascade_smile.xml'
4-اجرای فایل پروژه
موفق باشید
