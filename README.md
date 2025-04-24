# tp5_BigData
قواعد البيانات NoSQL - MongoDB

هذا المشروع يهدف إلى التعرف على أساسيات التعامل مع قواعد البيانات NoSQL باستخدام **MongoDB**، من خلال تنصيب البرنامج، ثم تنفيذ عمليات CRUD (إنشاء، قراءة، تحديث، حذف) على مجموعة بيانات بسيطة.

---
## خطوات العمل 
1/إنشاء قاعدة بيانات ومجموعة بيانات
![DB](https://github.com/user-attachments/assets/9aa717d6-cb8f-4747-8957-e13c53f5f716)

2/إنشاء مجموعة produits وإضافة مستندات
![produits](https://github.com/user-attachments/assets/5bd89e0f-a008-4c28-9390-1e2889bf4f1a)

3/الأوامر 
{} //كل المنتجات 
![all](https://github.com/user-attachments/assets/eae38f12-9ee6-41d7-87f8-ca0f29f95a4d)
//اول منتج { "nom": 1 }

![1](https://github.com/user-attachments/assets/f23dee17-05c6-4dc3-a240-55b52b05208f)
//البحث عن منتج باستخدام الـ ID (مثلاً للـ Thinkpad) { "_id": ObjectId("6803e387956fd7c4d6c4ad1b") }
![think](https://github.com/user-attachments/assets/b2c48ef1-cf9d-451e-9c56-c690b6e66e8c)
// جلب المنتجات التي سعرها أكبر من 13723 DA  { "prix": { "$gt": 13723 } }
![prix](https://github.com/user-attachments/assets/bcf3636e-f73a-453f-a847-923768c90e1e)
//أول منتج يحتوي على الحقل ultrabook: true 
![prod](https://github.com/user-attachments/assets/fe520c68-c070-4367-b854-8ce41e748c54)
// أول منتج اسمه يحتوي على كلمة "Macbook"   { "nom": { "$regex": "Macbook", "$options": "i" } }
![prod2](https://github.com/user-attachments/assets/1e7206c0-80c0-4c6a-a669-06b74e170c47)
// جلب كل المنتجات التي يبدأ اسمها بـ "Macbook" { "nom": { "$regex": "^Macbook", "$options": "i" } }
![Capture d’écran 2025-04-24 231008](https://github.com/user-attachments/assets/5dfccd45-fe51-474d-9207-6546c15bfae4)
//حذف كل المنتجات المصنعة من Apple { "fabriquant": "Apple" }
![delet](https://github.com/user-attachments/assets/e5856295-32e2-4198-822b-8affecbf6a02)
//حذف منتج محدد بالـ ID (مثل Lenovo X230) { "_id": ObjectId("6803e387956fd7c4d6c4ad1b") }
![delet2](https://github.com/user-attachments/assets/702e5be3-d9cd-4564-acef-8c7d47184e9e)











