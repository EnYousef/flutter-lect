
# ملاحظات هامة:
- *setter*
  ```class Rectangle {
  
  double left, top, width, height; // هذا السطر تعريف لمجموعة متغيرات بما انها من نفس النوع فخلي التعريف بسطر واحد

  Rectangle(this.left, this.top, this.width, this.height);

  // Define two calculated properties: right and bottom.
  double get right => left + width;
  set right(double value) => left = value - width; // طريقة كتابة ال setter .
  double get bottom => top + height;
  set bottom(double value) => top = value - height;
  }```
- *Extension methods*
  من خلال Extension methods نقدر انه نضيف دالة جديدة لنوع موجود سابقا مثل int او String وغيره هذا الشي يساعد انه نربط الدالة بالنوع المستهدف المثال التالي يوضح طريقة انشاء دالة مرتبطه بالنوع String وظيفتها تتحقق ما اذا كان النص فارغ اي مجرد مسافة او لا:
  ```
  extension on String {
  bool isBlank() {
    return this.trim().isEmpty;
  }
  }
  ```
  يمكن استخدام الدالة بالشكل التالي:
  ```
  String text = " ";
  print(text.isBlank());
  ```
  # التكليف:
  1. انشاء كلاس abstract باسم User يحوي الخصائص التالية (username - password) ودالة login التي تاخذ username و password كمامعلات
  2. انشاء كلاس Employee ويكون وارث من User وداخل هذا الكلاس يحوي الخصائص التالية (name - dob - phone - address - salary) ايضا يتم اضافة الوظيفة الخاصة بدالة login المعرفة سابقا واضافة دالة جديدة باسم printAllInformation() تقوم بطباعة كل بيانات الموظف ملاحظة يجب ان يتم اسناد بيانات الموظف عند انشاء كائن جديد من خلال constructors الخاص بكلاس Employee .
  3. توضيح للكلاسات المطلوبة: ![image](https://github.com/user-attachments/assets/80dc8b1a-26f2-447b-b756-e2985fc2e9e2)
  4. استخدم Extension methods لاضافة دالة جديدة تقوم بتحويل السلسة النصية الى رقم وفي حال لم تكون السلسة النصية تحوي على رقم قم بارجاع صفر.
