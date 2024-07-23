# - اعداد المتطلبات المطلوبة مسبقا (اي طالب اخذ الملفات مني ما يحتاج يحمل اي ملف من المذكورة.):
  1. تحميل JDK من الرابط : https://www.oracle.com/java/technologies/downloads/#jdk22-windows
  2. تحميل Git من الرابط : https://git-scm.com/download/win
  3. تحميل Flutter من الرابط: https://storage.googleapis.com/flutter_infra_release/releases/stable/windows/flutter_windows_3.22.3-stable.zip
  4. تحميل Android Studio من الرابط: https://developer.android.com/studio?hl=ar
# - خطوات التثبيت:
  1. تثبيت JDK
  2. تثبيت Git
  3. فك ضغط ملف flutter داخل حساب المستخدم C:\Users\{username} في حالتي كان اسم حساب المستخدم ComputerWorld.
  4. ![image](https://github.com/user-attachments/assets/1e596446-17ca-4947-bb20-425c5608e8ea)

  5. اضافة ملفات مسار فلاتر الى داخل متغيرات بيئئة النظام
       1. اضغط على شعار ويندوز واكتب **متغيرات** في حال كانت لغة جهازك عربي وفي حال كانت انجليزية اكتب **variable**
       2. ![image](https://github.com/user-attachments/assets/82dfe54a-f0ad-4717-a1c3-b0defdc3f79e)
       3. ![image](https://github.com/user-attachments/assets/76eb1ad8-8df7-4362-bf65-5e0e7a83b55d)
       4. ![image](https://github.com/user-attachments/assets/f4ad76bb-6310-4120-b663-f5628a8c3a74)
       5. ![image](https://github.com/user-attachments/assets/bb5a3e44-e66c-4caf-b3dc-cd646c8f8868)
       6. بعد الضغط على New (جديد) قم بلصق المسار الذي قمت بلصق فلاتر اليه الرابط يكون هكذا: C:\Users\{username}\flutter
       7. قم بفتح Cmd او Powershell واكتب الامر هذا الامر ``flutter doctor`` 
       8. ![image](https://github.com/user-attachments/assets/d91ef25f-7a05-48d4-b91f-d75109d323ca)
       9. في هذه المرحلة من المهم ان تكون Flutter عليها صح.
          
  6. هذه الخطوة **اختيارية** لمن لدية ملفات SDK
       1. ندخل المسار التالي: C:\Users\ComputerWorld\AppData\Local ونتحقق اذا كان يتوفر مجلد باسم Android
       2. اذا كان الملف موجودا نقوم بفك ضغط ملفات SDK فيه وان لم يكن موجودا نقوم بانشاء هذا المجلد وفك ضغط الملفات الى داخله.
7. تثبيت Android Studio (في حال عدم وجود ملفات SDK او وجود نقص بها سوف تظهر واجهة تطلب الموافقة على تثبيت اداوات SDK قم بالموافقة على ذلك وقد ياخذ التحميل وقت بسبب حجم الملفات)
8. افتح Cmd واكتب هذا الامر ``flutter doctor --android-licenses``
9. تثبيت Plugin الخاصة بفلاتر داخل Android Studio من **ملف > الاعدادات > Plugins** ثم نقوم بالبحث عن Flutter ونثبت الخيار الاول.
10. بعد تحميل Plugins الخاصة بفلاتر نقوم بانشاء مشروع فلاتر من **ملف > جديد > مشروع Fluttr جديد** او ** File > New < New Flutter Project** .
11. من داخل Android Studio نقوم بانشاء محاكي جديد لتنفيذ المشروع الجديد
    1. ![image](https://github.com/user-attachments/assets/2d39ac33-4876-4ca9-8588-1c973a7d2597)
    2. ![image](https://github.com/user-attachments/assets/cbf33f7b-fcf5-4666-8c2f-1c53812e1704)
    3. ![image](https://github.com/user-attachments/assets/9fac0f61-3c08-41d4-99df-aa5181fc5053)
    4. ![image](https://github.com/user-attachments/assets/2174dab4-5338-4768-8de7-733b1a1dc290)
    5. بعد الانتهاء من انشاء المحاكي يظهر المحاكي داخل الواجهة السابقة كما هو موضح بالصورة ونقوم بتشغيله من خلال الزر المحدد عليه.
    6. ![image](https://github.com/user-attachments/assets/67a7afee-b0af-444f-b3d9-3ba9d6134a00)
    7. بعد تشغيلة يظهر كما في الصورة التالية وفي حال عدم ظهور المحاكي اضغط على الزر المحدد
    8. ![image](https://github.com/user-attachments/assets/a3cfba1c-9af0-467f-bc2f-a4ff18af6649)
  12. بعد عملية انشاء المحاكي وتشغيلة قم بتنفيذ المشروع *هذه العملية تاخذ وقتا طويل نوعا ما وهذه المدة تكون تزيد او تنقص حسب مواصفات الجهاز وحسب سرعة الانترنت لديك* خلال مدة التنفيذ يتم تحميل ملفات Gradle بالاضافة الى اي Tools ناقصة .
- *في مصادر كثير بالنت تشرح كيفية التثبيت عادي شف اي مصدر وامشي معه من البداية لنهاية اذا كان واضح لك بس المهم تشيك على Git و JDK يمكن البعض ينسى يذكرهم. ايضا ممكن يكون يكون في اختلافات بين النقاط الي ذكرتها هنا وبين النقاط الي ببعض المصادر مثل المسار الي تفك فلاتر فيه لكن عادي المهم المسار ينضاف.*










  
