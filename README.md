
<div dir="rtl">

#  تمرين - 5
## صفحة تسجيل الدخول Sign In Page
### خطوات 
1. قم بعمل Fork لهذا المجلد و clone وافتح المجلد من خلال Github Desktop 
2. قم بإنشاء صفحة تسجيل الدخول الموضحة أدناه
3. يجب أن يكون الباسورد على هذه الهيئة •••••. 

<details>
  <summary>
    <strong>Hint 👀</strong>
  </summary>
بدلاً من استخدام `TextField` استعمل `SecureField` 
</details>

4. عند كتابة اسم المستخدم وكلمة السر بشكل صحيح، يتم استبدال الصفحة بصفحة فارغة مكتوب فيها "You are signed in". استعمل `if else` بداخل الواجهة
5. إذا قام المستخدم بكتابة البيانات بشكل خاطئ، قم بعرض رسالة تنبيه له. لا تعرضها إلا إذا أخطأ
6. قم بحساب كل خطأ، واعرض عدد المحاولات الخاطئة التي أخطأها المستخدم من خلال `Text` لونه أحمر  
<img width="300" src="https://user-images.githubusercontent.com/8784343/102728034-957b9300-433a-11eb-8894-3a56c1458af7.gif" alt="sign in page gif"/>


<details>
  <summary>
    <strong>بونص 🎁</strong>
  </summary>
  <pre>
- قم بتعطيل التصليح التلقائي spell check للكيبورد 
- إذا أدخل المستخدم الـ username بهاتين الطريقتين "UserName" أو "username" يقبلهم 
- إذا أدخل المستخدم نفس البيانات مرتين متتاليتين، لا يحسب عليه محاولة خاطئة
</pre>
</details>


لجعل الزر يأخذ حجم الشاشة، استعمل هذا الكود 


## قليل من الهنتات 😎

<div dir="ltr">

```Swift
  Text("Sign in")
    .padding()
    .frame(minWidth: 0, idealWidth: 100, maxWidth: .infinity)
    .foregroundColor(.white)
    .background(Color.green)
    .clipShape(RoundedRectangle(cornerRadius: 6))

```


</div>


</div>
