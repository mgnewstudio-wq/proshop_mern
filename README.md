ҮНДСЭН ФУНКЦҮҮД (FEATURES)
Дэлгүүрийн сагсны бүрэн ажиллагаа
Бүтээгдэхүүний үнэлгээ, сэтгэгдэл
Шилдэг бүтээгдэхүүний карусель (слайдер)
Бүтээгдэхүүний хуудаслалт (Pagination)
Бүтээгдэхүүн хайх функц
Хэрэглэгчийн захиалгын түүхтэй профайл
Админ: Бүтээгдэхүүн удирдах
Админ: Хэрэглэгч удирдах
Админ: Захиалгын дэлгэрэнгүй хуудас
Захиалгыг "Хүргэгдсэн" гэж тэмдэглэх
Төлбөрийн үйл явц (хүргэлт, төлбөрийн хэлбэр гэх мэт)
PayPal / кредит картны интеграцчилалӨгөгдлийн санг бэлэн мэдээллээр дүүргэгч (бүтээгдэхүүн ба хэрэглэгчид)
АШИГЛАЛТ (USAGE)

MongoDB өгөгдлийн сан үүсгэж, MongoDB URI-г авах - MongoDB AtlasPayPal бүртгэл үүсгэж,Client ID-г авах - PayPal DeveloperEnv (Орчны) Хувьсагчид.env.example файлыг .env болгон нэрийг нь өөрчилж, дотор нь дараах утгуудыг оруулна уу:NODE_ENV = development

PORT = 5000
MONGO_URI = your mongodb uri
JWT_SECRET = 'abc123'
PAYPAL_CLIENT_ID = your paypal client id
PAGINATION_LIMIT = 8
JWT_SECRET болон PAGINATION_LIMIT-г хүссэнээрээ өөрчилнө үү.Шаардлагатай Багцууды Суулгах (frontend & backend)npm install
cd frontend
npm install
АЖИЛЛУУЛАХ (RUN)# Frontend (:3000) ба Backend (:5000) серверийг хамт ажиллуулах
npm run dev

# Зөвхөн Backend серверийг ажиллуулах
npm run server
BUILD & DEPLOY (БҮТЭЭХ БА НИЙТЛЭХ)# Frontend-ийн production build үүсгэх
cd frontend
npm run build
ӨГӨГДЛИЙН САНГ ДҮҮРГЭХ (SEED DATABASE)Та дараах тушаалууды ашиглан өгөгдлийн санг жишиг хэрэглэгчид болон бүтээгдэхүүнээр дүүргэх, эсвэл бүх өгөгдлийг устгах боломжтой.# Мэдээлэл оруулах (Import)
npm run data:import

# Мэдээлэл устгах (Destroy)
npm run data:destroy
Жишиг хэрэглэгчийн нэвтрэх мэдээлэл

admin@email.com (Админ)
123456

john@email.com (Хэрэглэгч)
123456

jane@email.com (Хэрэглэгч)
123456
