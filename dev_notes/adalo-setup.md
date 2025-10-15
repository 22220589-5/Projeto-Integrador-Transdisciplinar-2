# Configuração do Projeto no Adalo (Low-Code)

## 🧩 Estrutura de Dados (Collections)

### 1. Users
Campos:
- `name` (text)
- `email` (email)
- `password` (password - campo interno do Adalo)
- `role` (text - valores possíveis: "cliente" ou "admin")

### 2. Products
Campos:
- `name` (text)
- `description` (text)
- `price` (decimal)
- `stock` (number)
- `image` (image - opcional)
- `active` (true/false)
- `createdBy` (relationship → User)
- `orderItems` (relationship → OrderItem)

Relação:
- Um **User (admin)** pode criar vários **Products**.
- Um **Product** pertence a um único **User (admin)**.

### 3. Orders
Campos:
- `date` (date/time)
- `status` (text - valores: "pendente", "enviado", "entregue")
- `total` (decimal)
- `user` (relationship → User)
- `payment` (relationship → Payment)
- `orderItems` (relationship → OrderItem)

Relação:
- Um **User** pode ter vários **Orders**.
- Cada **Order** pode conter vários **OrderItems**.

### 4. OrderItems
Campos:
- `quantity` (number)
- `subtotal` (decimal)
- `product` (relationship → Product)
- `order` (relationship → Order)

Relação:
- Um **Order** pode ter vários **OrderItems**.
- Um **OrderItem** pertence a um único **Product**.

### 5. Payments
Campos:
- `method` (text)
- `value` (decimal)
- `status` (text - ex: "pago", "pendente")
- `order` (relationship → Order)

Relação:
- Um **Payment** pertence a um **Order**.

---

## 👤 Conta Administrador de Teste
- **E-mail:** admin@cupcakesgourmet.com  
*(A senha é configurada dentro do Adalo, não deve ser incluída no repositório.)*

---

## 🔗 Link do App Hospedado
[https://joao-paulos-team-46.adalo.com/cupcakes-gourmet-app](https://joao-paulos-team-46.adalo.com/cupcakes-gourmet-app)

---

## 📄 Observações
- Todas as collections foram criadas dentro do editor **Adalo Database**.  
- Relacionamentos seguem o mesmo modelo dos diagramas do diretório `/docs`.  
- Campos opcionais (como `image`) foram deixados vazios para simplificação inicial.  
- O campo `active` controla a exibição dos produtos no catálogo.
