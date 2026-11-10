# 🐾 PetCode | Planos de Saúde Veterinários Inteligentes

> O plano de saúde com o **código genético** do cuidado.

**PetCode** é um site institucional e de contratação de planos de saúde para pets, desenvolvido como **Single Page Application** em um único arquivo HTML, usando **Tailwind CSS**, **JavaScript puro** e **localStorage** para simular um sistema completo (cadastro, login, área do cliente e painel administrativo) sem precisar de back-end.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Font Awesome](https://img.shields.io/badge/Font_Awesome-528DD7?style=flat&logo=fontawesome&logoColor=white)

---

## 📸 Preview

> Adicione aqui capturas de tela do projeto (ex.: `docs/home.png`, `docs/admin.png`).

---

## ✨ Funcionalidades

### 🌐 Área pública (Home)
- **Hero** com apresentação do serviço e carteirinha digital de exemplo.
- **Simulador de Plano Ideal**: quiz com espécie, porte, raça, idade e estilo de vida que recomenda o plano **Essencial**, **Plus** ou **Total**.
- **Calculadora de Idade Humana**: converte a idade do pet para anos humanos, com regras específicas para cães (por porte), gatos, coelhos, hamsters, pássaros, porquinhos-da-índia e tartarugas.
- **Busca de Clínicas Parceiras**: simulação de rede credenciada a partir do CEP, com loader animado.
- **Cards de Planos** com preços e coberturas carregados dinamicamente.
- **Universo PetCode**:
  - 7 cards de curiosidades com efeito *flip* 3D;
  - Accordion de cuidados pós-cirúrgicos.
- **Carrossel de depoimentos** de tutores.
- **Menu responsivo** com overlay mobile.

### 🧾 Fluxo de contratação
Processo em 3 etapas com indicador de progresso:
1. **Tutor**: dados pessoais
2. **Pet**: dados do animal
3. **Checkout**: ativação do plano

### 👤 Área do cliente
- Criação de conta e login com dados do primeiro pet.
- **Meus Pets**: adicionar e editar múltiplos pets.
- **Meu Plano**: visualização e troca de plano.
- Seções de **Segurança** e **Pagamentos** (placeholders para evolução futura).

### 🔐 Painel administrativo
- Listagem de todos os clientes, pets, planos e status de pagamento.
- Exclusão de cadastros.
- **Gestão de Ofertas e Planos**: edição de nome, preço e coberturas de cada plano, refletindo imediatamente no site.

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura da aplicação |
| [Tailwind CSS (CDN)](https://tailwindcss.com/) | Estilização e responsividade |
| [Font Awesome 6](https://fontawesome.com/) | Ícones |
| JavaScript (ES6+) | Lógica, navegação entre telas e renderização dinâmica |
| `localStorage` | Persistência de usuários, sessão e configuração de planos |

---

## 🚀 Como executar

Não é necessário instalar nada.

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/petcode.git

# 2. Acesse a pasta
cd petcode

# 3. Abra o arquivo no navegador
# (dê dois cliques em index.html ou use uma extensão como Live Server)
```

> Requer conexão com a internet para carregar o Tailwind CSS e o Font Awesome via CDN.

---

## 🔑 Acesso de demonstração

Para testar o painel administrativo, entre com:

| Campo | Valor |
|---|---|
| E-mail | `admin@petcode.com` |
| Senha | `admin123` |

Usuários comuns podem ser criados pelo botão **Entrar / Cadastrar**.

---

## 📁 Estrutura

```
petcode/
├── index.html    # Aplicação completa (HTML + JS)
└── README.md
```

### Telas (views) da aplicação

| View | Descrição |
|---|---|
| `view-home` | Página inicial |
| `view-cadastro` | Fluxo de contratação em 3 etapas |
| `view-conta` | Área do cliente |
| `view-admin` | Painel administrativo |

---

## 💾 Dados no localStorage

| Chave | Conteúdo |
|---|---|
| `petcode_usuarios` | Lista de todos os usuários cadastrados |
| `petcode_usuario_logado` | Usuário da sessão atual |
| `petcode_config_planos` | Nome, preço e coberturas dos planos |

---

## ⚠️ Aviso importante

Este é um **projeto de demonstração/portfólio**. Por não possuir back-end:

- Senhas são armazenadas **em texto puro** no navegador.
- O login de administrador é fixo no código.
- O checkout e a busca de clínicas são **apenas simulações**; nenhum pagamento real é processado.
- Os dados ficam restritos ao navegador de cada usuário.

**Não use dados pessoais reais** e não utilize esta estrutura em produção sem implementar autenticação, banco de dados e backend adequados.

---

## 🗺️ Próximos passos

- [ ] Back-end com API REST e banco de dados
- [ ] Autenticação segura (hash de senha, JWT)
- [ ] Integração com gateway de pagamento
- [ ] Busca real de clínicas por CEP (API de geolocalização)
- [ ] Validação de CPF e máscaras nos formulários
- [ ] Implementação das seções de Segurança e Pagamentos
- [ ] Separar HTML, CSS e JS em arquivos distintos

---

## 📄 Licença

Distribuído sob a licença MIT. Veja o arquivo `LICENSE` para mais informações.

---

<p align="center">Feito com 💚 para quem trata os pets como família.</p>

https://celadon-ganache-6048e1.netlify.app/
