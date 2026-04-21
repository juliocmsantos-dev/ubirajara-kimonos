# <img src="img/homer1.png" width="60" align="left" style="margin-right:16px;border-radius:50%;"> Ubirajara Kimonos

> *"Ubirajara - "Senhor da lança"* — E-commerce de Artes Marciais desenvolvido como projeto acadêmico

<br>

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

</div>

---

## 🪶 Sobre o Nome

**Ubirajara** vem do tupi-guarani ***Ybyrá-jara***: **"Senhor da Lança"** — o guerreiro que porta a lança, símbolo de força, honra e presença.

O nome é uma escolha pessoal e identitária: o desenvolvedor deste projeto pratica **retomada identitária indígena** e é **Guarani Mbya**. Nomear a loja com uma palavra tupi é um ato de afirmação cultural — um lembrete de que a luta, o respeito e a identidade caminham juntos, dentro e fora do tatame.

> *"A lança não é símbolo de guerra. É símbolo de quem sabe onde está e para onde vai."*

---

## 🥋 Sobre o Projeto

**Ubirajara Kimonos** é um e-commerce temático de artes marciais — desenvolvido como **Trabalho Avaliativo (T1)** da disciplina de Desenvolvimento Web, com foco nos esportes:

- 🥋 Jiu-Jitsu Brasileiro
- 🥊 Boxe e Muay Thai
- ⚔️ MMA
- 🤺 Judô

A loja oferece kimonos, luvas, caneleiras, faixas e acessórios para todos os níveis — do iniciante ao competidor.

---

## 🟡 O Mascote: Homer Simpson

<img src="img/homer1.png" width="180" align="right" style="border-radius:12px; margin-left:20px;">

O mascote da **Ubirajara Kimonos** é o **Homer Simpson de kimono** — e a escolha vai muito além do humor.

Homer representa um personagem muito especial nos centros de treinamento (CTs) de Jiu-Jitsu: **o aluno comum, trabalhador, pai de família, que só consegue treinar 3 vezes na semana.**

Ele não é atleta profissional. Não compete. Chega cansado do trabalho, às vezes pensa em faltar — mas vai. Treina a sua horinha, respeita os colegas, respeita o professor, paga a mensalidade em dia, e sai com aquele sorriso satisfeito de quem deu o seu melhor.

**O Homer é o coração do Jiu-Jitsu.** É ele que sustenta a academia. É ele que mantém o tatame vivo. Um dia já foi mais ativo, talvez tenha competido — hoje treina pela saúde, pela cabeça, e pelo prazer de apertar o kimono e estar presente.

> *"Você não precisa ser faixa preta para respeitar o tatame. Você só precisa aparecer."*

O Homer Simpson **carrega esse simbolismo**: o respeito, a humildade, a constância e a alegria de fazer parte de uma arte marcial — mesmo sendo, a seus próprios olhos, apenas um cara comum.

---

## 🗂️ Estrutura do Projeto

```
ubirajara-kimonos/
│
├── 📄 index.html          → Página inicial (hero, categorias, produtos)
├── 📄 catalogo.html       → Catálogo com filtros por categoria e marca
├── 📄 produto.html        → Página individual do produto com galeria
├── 📄 carrinho.html       → Carrinho de compras funcional
├── 📄 checkout.html       → Finalização de compra com formulário completo
├── 📄 clientes.html       → Lista de clientes cadastrados
├── 📄 ficha_cliente.html  → Painel do usuário (dados e endereços)
├── 📄 pedidos.html        → Histórico de pedidos do cliente
│
├── 🎨 style.css           → Folha de estilos global (CSS Grid, variáveis)
│
└── 📁 img/
    ├── homer.png          → Logo do site (Homer no kimono)
    ├── homer1.png         → Homer esquerda (hero banner)
    ├── homer2.png         → Homer direita (hero banner)
    ├── kimono.png         → Produto: Kimono Jiu-Jitsu
    ├── luva.jpg           → Produto: Luva MMA Venum
    ├── luvaboxe.png       → Produto: Luva de Boxe Pro Fighter
    └── luvapoatan.png     → Produto: Luva Edição Poatan
```

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Uso no projeto |
|---|---|
| **HTML5** | Estrutura semântica de todas as páginas |
| **CSS3 + CSS Grid** | Layout responsivo com `grid-template-areas` |
| **JavaScript (Vanilla)** | Carrinho via `localStorage`, troca de imagens, busca de CEP |
| **PHP** | Backend: processamento do pedido, validação, integração com banco |
| **MySQL** | Banco de dados hospedado no InfinityFree |
| **Font Awesome** | Biblioteca de ícones |
| **Google Fonts** | Tipografia: Barlow + Barlow Condensed |
| **API ViaCEP** | Preenchimento automático de endereço pelo CEP |

---

## 📐 CSS Grid — Obrigatório no Trabalho

O projeto utiliza **CSS Grid** como sistema de layout principal em todas as páginas, conforme exigido pelo professor. Exemplos de uso:

```css
/* Header — 4 colunas nomeadas */
.site-header {
  display: grid;
  grid-template-columns: 80px 1fr auto auto;
  grid-template-areas: "logo busca atendimento icones";
}

/* Checkout — formulário + resumo lateral */
.pagina-checkout {
  display: grid;
  grid-template-columns: 1fr 340px;
  grid-template-areas: "formularios resumo-checkout";
}

/* Catálogo — filtros + grade de produtos */
.pagina-catalogo {
  display: grid;
  grid-template-columns: 240px 1fr;
  grid-template-areas: "filtros area-produtos";
}

/* Painel do usuário — sidebar + conteúdo */
.painel-grid {
  display: grid;
  grid-template-columns: 220px 1fr;
  grid-template-areas: "sidebar main";
}
```

---

## 🛒 Funcionalidades Implementadas

### Front-end
- [x] Página inicial com hero banner, categorias e produtos em destaque
- [x] Catálogo com filtros (categoria, marca, preço, tamanho)
- [x] Página de produto com galeria interativa (troca de imagem ao clicar)
- [x] Seleção de tamanho com destaque visual
- [x] **Carrinho 100% funcional** via `localStorage` (persiste entre páginas)
- [x] Badge do carrinho atualiza em tempo real
- [x] Checkout com formulário completo (dados pessoais + endereço + pagamento)
- [x] **Busca automática de CEP** pela API ViaCEP (preenche o endereço sozinho)
- [x] Tabs de pagamento: Cartão de Crédito, Boleto e PIX
- [x] Formatação automática do número do cartão (blocos de 4 dígitos)
- [x] Cupom de desconto funcional (`UBIRAJARA10` = 10% off)
- [x] Cálculo de parcelamento dinâmico (até 12x)
- [x] Lista de clientes com busca e paginação
- [x] Painel do usuário com sidebar e formulário de edição
- [x] Histórico de pedidos com expansão de detalhes

### Identidade Visual
- [x] Paleta: **vermelho `#cc0000`**, preto e branco
- [x] Mascote Homer Simpson em kimono com faixa preta
- [x] Tipografia: **Barlow Condensed** (títulos) + **Barlow** (texto)
- [x] Cards com hover animado (`transform: translateY`)
- [x] Header sticky (fixo no topo ao rolar a página)
- [x] Botão flutuante de carrinho (canto inferior direito)

---

## 📋 Páginas Obrigatórias (Requisitos)

| Requisito | Página | Status |
|---|---|---|
| Carrinho de compras | `carrinho.html` | ✅ |
| Checkout / Pagamento | `checkout.html` | ✅ |
| Lista de Clientes | `clientes.html` | ✅ |
| Ficha do Cliente | `ficha_cliente.html` | ✅ |
| Catálogo de Produtos | `catalogo.html` | ✅ |
| Lista de Pedidos | `pedidos.html` | ✅ |
| Wireframe das páginas | Estrutura HTML + comentários | ✅ |
| CSS Grid obrigatório | Todas as páginas | ✅ |
| Identidade visual | Logo, cores, imagens | ✅ |

---

## 🎨 Identidade Visual

| Elemento | Valor |
|---|---|
| Cor principal | `#cc0000` (vermelho) |
| Cor secundária | `#111111` (preto) |
| Cor de ação (comprar) | `#28a745` (verde) |
| Fonte dos títulos | Barlow Condensed 900 |
| Fonte do corpo | Barlow 400/600/700 |
| Border radius padrão | `6px` |
| Mascote | Homer Simpson 🥋 |

---

## 🚀 Como Rodar Localmente

### Pré-requisitos
- **XAMPP** ou **WAMP** instalado (para rodar PHP)
- Ou apenas abrir os `.html` no navegador (para ver o front-end)

### Front-end apenas (sem PHP)
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/ubirajara-kimonos.git

# Abra o index.html no navegador
# (duplo clique no arquivo ou arraste para o Chrome/Firefox)
```

### Com PHP e banco de dados
```bash
# 1. Clone dentro da pasta htdocs do XAMPP
git clone https://github.com/seu-usuario/ubirajara-kimonos.git C:/xampp/htdocs/ubirajara

# 2. Inicie o Apache e MySQL no XAMPP

# 3. Acesse no navegador
http://localhost/ubirajara/
```

> **Nota:** Os arquivos PHP de backend (processa_pedido.php, ver_pedidos.php) não estão incluídos neste repositório público por conterem credenciais do banco de dados.

---

## 📱 Capturas de Tela

### Página Inicial
> Hero banner com Homer Simpson, categorias em ícones circulares e grade de produtos com imagens reais.

### Carrinho de Compras
> Carrinho funcional com controle de quantidade, cálculo de frete e resumo lateral sempre visível.

### Checkout
> Formulário completo com preenchimento automático de CEP, tabs de pagamento e cálculo de parcelamento dinâmico.

---

## 👨‍💻 Desenvolvedor

**Julio** — Estudante de Desenvolvimento Web  
🪶 Guarani Mbya | Praticante de Retomada Identitária Indígena  
🥋 Jiu-Jitsu | Artes Marciais  

---

## 📚 Contexto Acadêmico

Projeto desenvolvido como **T1 — Primeiro Trabalho Avaliativo** da disciplina de **Desenvolvimento Web**.

**Critérios atendidos:**
- ✅ Wireframe de todas as páginas (2,0 pts)
- ✅ CSS Grid obrigatório em todas as páginas (3,0 pts)
- ✅ Organização e layout (2,0 pts)
- ✅ Imagens e identidade visual (1,0 pt)
- ✅ Integração com PHP/backend (2,0 pts)

---

## 📄 Licença

Este projeto foi desenvolvido para fins **acadêmicos**.  
O personagem Homer Simpson é propriedade da **Fox / Matt Groening**.  
As imagens de produtos são utilizadas apenas para fins educacionais.

---

<div align="center">

**Ubirajara Kimonos** — *"Senhor da Lança"* 🪶  

*Feito com ❤️ e muito treino*

`HTML` · `CSS Grid` · `JavaScript` · `PHP` · `MySQL`

</div>
