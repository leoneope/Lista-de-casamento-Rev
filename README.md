# Site de Casamento - Leo & Dan 💕

Um site completo para gerenciamento de casamento com paleta de cores terracota, desenvolvido especialmente para Leo e Dan.

## 🎨 Design

- **Paleta de Cores**: Terracota (#C65D32, #E07B39, #F4A261, #A0522D)
- **Tipografia**: Georgia, Times New Roman (serif)
- **Estilo**: Elegante, romântico e responsivo

## ✨ Funcionalidades

### 📱 Site Principal (`index.html`)
- Página inicial com informações do casamento
- Design responsivo para mobile e desktop
- Navegação suave entre seções
- Informações sobre data, local e história do casal

### 👥 Confirmação de Presença (`rsvp.html`)
- Formulário completo de RSVP
- Campos condicionais baseados na confirmação
- Contagem de adultos e crianças
- Campo para restrições alimentares
- Mensagens personalizadas para os noivos

### 🎁 Lista de Presentes (`gifts.html`)
- Lista interativa de presentes
- Filtros por categoria e status
- Sistema de "presentear" com informações do comprador
- Estatísticas em tempo real
- Interface intuitiva e responsiva

### ⚙️ Painel Administrativo (`admin.html`)
- Gerenciamento completo de convidados
- Administração da lista de presentes
- Visualização de confirmações RSVP
- Configurações do casamento
- Estatísticas e relatórios

## 🚀 Como Usar

### 1. Hospedagem no GitHub Pages

1. Faça fork ou clone este repositório
2. Vá em **Settings** > **Pages**
3. Selecione **Deploy from a branch**
4. Escolha **main** branch e **/ (root)**
5. Clique em **Save**

### 2. Estrutura de Arquivos

```
leo-dan-wedding/
├── src/
│   └── static/
│       ├── index.html      # Página principal
│       ├── admin.html      # Painel administrativo
│       ├── rsvp.html       # Confirmação de presença
│       └── gifts.html      # Lista de presentes
├── README.md               # Este arquivo
└── requirements.txt        # Dependências (se usar Flask)
```

### 3. Personalização

#### Alterar Informações do Casal
Edite os arquivos HTML e modifique:
- Nomes dos noivos
- Data do casamento
- Locais da cerimônia e recepção
- História do casal

#### Modificar Lista de Presentes
No arquivo `gifts.html`, edite o array `gifts` no JavaScript:

```javascript
gifts = [
    {
        id: 1,
        name: 'Nome do Presente',
        description: 'Descrição detalhada',
        price: 299.90,
        category: 'cozinha', // cozinha, quarto, casa, lua-de-mel, outros
        purchased: false,
        icon: '🍳'
    }
    // ... mais presentes
];
```

#### Personalizar Cores
Modifique as variáveis CSS em cada arquivo:

```css
:root {
    --terracota-primary: #C65D32;
    --terracota-secondary: #E07B39;
    --terracota-light: #F4A261;
    --terracota-dark: #A0522D;
    --cream: #F5F5DC;
    --warm-white: #FFF8F0;
}
```

## 💾 Armazenamento de Dados

O site utiliza `localStorage` do navegador para armazenar:
- Lista de convidados
- Confirmações RSVP
- Status dos presentes
- Configurações do casamento

**Nota**: Para um site em produção, considere integrar com um backend real para persistência de dados.

## 📱 Responsividade

O site é totalmente responsivo e funciona perfeitamente em:
- 📱 Smartphones
- 📱 Tablets
- 💻 Desktops
- 🖥️ Monitores grandes

## 🎯 Funcionalidades Técnicas

- **CSS Grid e Flexbox** para layouts responsivos
- **JavaScript Vanilla** para interatividade
- **LocalStorage** para persistência de dados
- **Animações CSS** para melhor experiência
- **Formulários validados** com feedback visual
- **Modais** para interações complexas

## 🔧 Desenvolvimento Local

Para testar localmente:

1. Clone o repositório
2. Abra `src/static/index.html` em um navegador
3. Ou use um servidor local:
   ```bash
   cd src/static
   python -m http.server 8000
   ```
4. Acesse `http://localhost:8000`

## 📝 Licença

Este projeto foi desenvolvido especialmente para Leo e Dan. Sinta-se livre para usar como base para seu próprio site de casamento!

## 💝 Créditos

Desenvolvido com muito carinho para Leo & Dan
Data do Casamento: 15 de Dezembro de 2025

---

**Que este site ajude a tornar seu dia especial ainda mais memorável! 💕**

