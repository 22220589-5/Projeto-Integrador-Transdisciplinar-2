# Cupcakes Gourmet App

## 📌 Visão Geral
Aplicativo mobile desenvolvido no modo Low-Code utilizando a plataforma Adalo, como parte do Projeto Integrador Transdisciplinar II.
O sistema representa uma loja de cupcakes gourmet, permitindo visualizar produtos, adicionar ao carrinho, finalizar pedidos e acompanhar o status de entrega.
O foco do projeto é demonstrar o ciclo completo de desenvolvimento de software com base em documentação, modelagem de dados, prototipação e entrega funcional.

---

## 🎯 Objetivos
- Disponibilizar catálogo de cupcakes gourmet.  
- Permitir adicionar itens ao carrinho e finalizar pedidos.  
- Oferecer opções de pagamento e rastreamento de pedidos.  
- Melhorar a imagem da loja através de um app estável e intuitivo.  

---

## 🛠️ Arquitetura e Abordagem
Este projeto foi implementado com ferramentas Low-Code, eliminando a necessidade de codificação manual extensa.
A estrutura segue a lógica do padrão MVC (conceitualmente), mas com componentes visuais configurados no Adalo:
- Model (Dados) → Collections do Adalo: Users, Products, Orders, OrderItems e Payments.
- View (Interface) → Telas construídas via drag-and-drop no editor visual do Adalo.
- Controller (Fluxos e Regras) → Ações automáticas do Adalo configuradas com condições e relacionamentos entre collections.

---

## ⚙️ Tecnologias Utilizadas
- Plataforma: Adalo
- Banco de Dados: Collections internas do Adalo
- Hospedagem: Própria da plataforma
- Prototipação: Figma e Draw.io (modelos visuais complementares)
- Controle de Versão: Git + GitHub

## 🌐 Link da Solução em Funcionamento
https://joao-paulos-team-46.adalo.com/cupcakes-gourmet-app

(Abra no navegador ou no celular para visualizar a versão mobile do aplicativo.)


## 📂 Estrutura de Pastas
```
/docs
   ├── casos_de_uso.md
   ├── diagrama_classes.png
   ├── der.png
   ├── dicionario_dados.xlsx
   └── prototipos/
       ├── tela_catalogo.png
       ├── tela_carrinho_de_compras.png
       ├── tela_login.png
       ├── tela_rastreamento.png
       └── tela_administracao_de_produtos.png
/dev_notes
   ├── README.md
   └── adalo-setup.md
```
---

## ✅ Critérios de Aceite
- O cliente pode navegar no catálogo e ver os cupcakes disponíveis.  
- É possível adicionar/remover itens do carrinho.  
- O sistema registra o status do pedido.
- O administrador pode cadastrar, editar ou remover produtos.
- A aplicação está hospedada e acessível via link público.

---

## 👥 Equipe
- **Aluno:** João Paulo da Silva Freitas  
- **RGM:** 42246342  
