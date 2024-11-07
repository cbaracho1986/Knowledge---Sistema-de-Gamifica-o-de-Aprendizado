# Knowledge-Sistema-de-Gamifica-o-de-Aprendizado

Um sistema web de gamificação para aprendizado usando o método ANKI de repetição espaçada.

## Funcionalidades

- Sistema de login e registro
- Gamificação com pontos e níveis
- Sistema ANKI de repetição espaçada
- Gerenciamento de decks de estudo
- Estatísticas detalhadas
- Calendário de revisões
- Sistema de tags
- Importação de conteúdo via CSV

## Instalação

1. Clone este repositório:
```bash
git clone https://github.com/seu-usuario/gamification-system.git
cd gamification-system
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
Crie um arquivo `.env` na raiz do projeto com as seguintes variáveis:
```env
NODE_ENV=development
PORT=3000
```

4. Inicie o servidor de desenvolvimento:
```bash
npm start
```

## Estrutura do Projeto

```
gamification-system/
├── public/
│   ├── index.html
│   └── styles.css
├── src/
│   ├── components/
│   │   ├── AnkiSystem.js
│   │   ├── CalendarSystem.js
│   │   ├── ChartComponents.js
│   │   ├── DeckComponents.js
│   │   └── StatsDashboard.js
│   ├── services/
│   │   ├── auth.js
│   │   ├── activities.js
│   │   ├── points.js
│   │   ├── deck-system.js
│   │   └── content-manager.js
│   ├── utils/
│   │   └── helpers.js
│   └── app.js
└── README.md
```

## Uso

1. Crie uma conta ou faça login
2. Crie um novo deck de estudo
3. Importe conteúdo via CSV ou adicione manualmente
4. Comece a estudar e ganhe pontos
5. Acompanhe seu progresso nas estatísticas

## Formato do CSV para Importação

O arquivo CSV deve conter as seguintes colunas:
- title: Título da atividade
- type: Tipo (multiple_choice ou text)
- question: Pergunta
- answer: Resposta correta
- options: Opções para múltipla escolha (separadas por ;)
- difficulty: Dificuldade (easy, medium, hard)
- description: Descrição da atividade

Exemplo:
```csv
title,type,question,answer,options,difficulty,description
"Matemática","multiple_choice","Quanto é 2+2?","4","3;4;5;6","easy","Soma simples"
"Geografia","text","Capital do Brasil?","brasilia","","easy","Capitais"
```

## Tecnologias Utilizadas

- HTML5/CSS3
- JavaScript (ES6+)
- TailwindCSS
- Recharts (gráficos)
- LocalStorage para persistência

## Contribuindo

1. Fork o projeto
2. Crie sua branch de feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para detalhes.

## Autores

* **Seu Nome** - *Trabalho inicial* - [SeuUsuario](https://github.com/seu-usuario)

## Agradecimentos

* Método ANKI
* Recharts
* TailwindCSS
