Akhunkhail Mega Mart - POS (MVP)

Structure:
- backend/  (Node.js + Express + SQLite)
- frontend/ (React)

Backend:
1. cd backend
2. npm install
3. node server.js
   - Default admin created: username=admin, password=admin123
4. API: http://localhost:4000/api
   - GET /products
   - POST /products  (body: {name, price, stock, category})
   - POST /sales (body: { items: [{productId, qty}], payment_method })

Frontend:
1. cd frontend
2. npm install
3. npm start
4. Open http://localhost:3000

To add sample products quickly (after backend is running), use:
curl -X POST http://localhost:4000/api/products -H "Content-Type:application/json" -d '{"name":"Apple","price":0.5,"stock":100,"category":"Fruits"}'

Notes:
- This is a starter MVP. For production, change JWT secret, enable HTTPS, and use a production DB.
- If you want, I can create additional admin frontend pages, login flow, and export features.
admin
admin123
