
# 🧩 4.2.2 Reusable Profile Card Component (React)

🎯 Энэ хичээл нь FreeCodeCamp-ийн `Reusable Profile Card Component` төслийг даган хийж, React-ийн **props**, **component**, болон **JSX** ойлголтуудыг сурахад зориулагдсан.

📝 Хичээлийн дэлгэрэнгүй код болон тайлбарыг **PDF Material** хэсгээс дарж үзнэ үү.

🔗 FreeCodeCamp линк: [freeCodeCamp - Build a Reusable Profile Card Component](https://www.freecodecamp.org/learn/full-stack-developer/workshop-reusable-profile-card-component)

---

## 📚 Алхам алхмаар тайлбар

### ✅ Step 1: `Card` Component үүсгэх
```jsx
export default function Card({ name, title, bio }) {
  return ("");
}
export түлхүүр үгийг ашиглан Card функцийн компонент үүсгэнэ.

props-оос name, title, bio гэсэн утгуудыг destructure хийж авч байна.

✅ Step 2: div нэмэх
jsx
Copy
Edit
return (
  <div className="card"></div>
);
card гэдэг className-тай div үүсгэнэ.

Энэ нь бидний карт бүрийг хүрээлсэн layout болно.

✅ Step 3: Карт дотор props-уудаа харуулах
jsx
Copy
Edit
return (
  <div className="card">
    <h2>{name}</h2>
    <p className="card-title">{title}</p>
    <p>{bio}</p>
  </div>
);
name, title, bio props-уудыг JSX дотор {}-аар оруулан харуулна.

card-title нь онцгой class тул styles.css-д стилийг өөрөөр өгсөн.

✅ Step 4: App Component үүсгэх
jsx
Copy
Edit
export function App() {
  return ("");
}
App бол үндсэн component бөгөөд түүнээс Card-уудыг дуудаж харуулна.

✅ Step 5: Layout хийх
jsx
Copy
Edit
return (
  <div className="flex-container"></div>
);
flex-container нь бүх Card-уудыг нэг эгнээ болгон зэрэгцүүлж харуулна.

✅ Step 6: Эхний Card нэмэх
jsx
Copy
Edit
<Card
  name="Mark"
  title="Frontend developer"
  bio="I like to work with different frontend technologies and play video games."
/>
Card компонентыг нэг удаа ашиглаж, name, title, bio утгуудыг дамжуулсан.

✅ Step 7: Нэмэлт хоёр Card нэмэх
jsx
Copy
Edit
<Card
  name="Tiffany"
  title="Engineering manager"
  bio="I have worked in tech for 15 years and love to help people grow in this industry."
/>

<Card
  name="Doug"
  title="Backend developer"
  bio="I have been a software developer for over 20 years and I love working with Go and Rust."
/>
Хоёр шинэ хүн нэмэгдсэнээр component reuse буюу дахин ашиглах чадвар тодорхойлогдоно.
