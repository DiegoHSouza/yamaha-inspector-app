🏍️ Yamaha Inspector App
Aplicativo mobile para gestão e avaliação de motocicletas seminovas.

Este projeto foi desenvolvido com foco em Arquitetura Limpa, Performance e UX Profissional, simulando um ambiente real de engenharia de software para resolver dores do dia a dia de concessionárias.

Status Tech Lang

📱 Sobre o Projeto
O Yamaha Inspector nasce da necessidade de digitalizar e padronizar o processo de vistoria de motos. O objetivo é substituir processos manuais e planilhas por uma aplicação robusta que permite:

Autenticação segura de consultores.
Gerenciamento de vistorias via painel Kanban (Enviada, Andamento, Perda, Ganho).
Inserção ágil de novos dados de veículos.
🛠️ Tecnologias & Arquitetura
A arquitetura foi desenhada para garantir escalabilidade e fácil manutenção, seguindo as melhores práticas do desenvolvimento mobile moderno:

Core: React Native (Expo SDK 50+)
Linguagem: TypeScript (Tipagem Estrita)
Navegação: React Navigation
Nested Navigation: Combinação de Stack Navigator (Login) com Bottom Tabs (Dashboard).
Custom Tab Bar: Botão de ação centralizado ("Floating Action Button").
Design System: - Layouts resilientes (Flexbox) adaptáveis a diferentes tamanhos de tela.
Componentes desacoplados e reutilizáveis (Input, Button com Auto-Scaling).
Arquitetura: Clean Architecture (Separação de responsabilidades):
src/screens: Lógica das telas.
src/components: Interface de Usuário reutilizável.
src/routes: Configuração de navegação.
src/types: Contratos de dados (Interfaces e DTOs).
✨ Funcionalidades Destaque
1. Sistema de Navegação Híbrido
Implementação profissional de navegação aninhada. O usuário passa por uma Stack de Autenticação e é redirecionado para um TabNavigator, onde o histórico de rotas é gerenciado de forma segura (.replace ao invés de .navigate).

2. Layouts Resilientes (Bulletproof UI)
Uso avançado de Flexbox e propriedades como adjustsFontSizeToFit. Isso garante que textos dinâmicos (como filtros de status) se adaptem ao layout, mantendo a consistência visual independente do dispositivo ou tamanho de fonte do sistema.

3. Dashboard Interativo
Implementação de "Kanban Mobile" utilizando abas de filtro de estado (State Driven UI) para alternar a visualização das listas de vistorias, otimizando a experiência do usuário em telas verticais.

🚀 Como rodar o projeto
Pré-requisitos: Node.js instalado.

Clone o repositório:
git clone [https://github.com/DiegoHSouza/yamaha-inspector-app.git](https://github.com/DiegoHSouza/yamaha-inspector-app.git)
Entre na pasta do projeto:

Bash

cd yamaha-inspector-app
Instale as dependências:

Bash

npm install
# ou
npx expo install
Execute o projeto:

Bash

npx expo start
Utilize o aplicativo Expo Go no seu celular (Android ou iOS) para escanear o QR Code gerado pelo terminal.

👨‍💻 Autor
Desenvolvido por Diego H. Souza.

Estudante de Ciência da Computação e Desenvolvedor Mobile em transição de carreira (Background em Liderança Comercial). Apaixonado por transformar problemas de negócio em soluções de software elegantes e bem arquitetadas.
