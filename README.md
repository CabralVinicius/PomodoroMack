Documentação do Projeto Pomodoro Multitemático

1. Visão Geral
O Pomodoro Multitemático é um sistema de gestão de tempo baseado na técnica Pomodoro (25 minutos de trabalho / 5 minutos de descanso), integrado a playlists do YouTube e personalizável com temas visuais imersivos. O projeto combina funcionalidades práticas com elementos lúdicos para aumentar a produtividade e o engajamento do usuário.

2. Objetivos
Fornecer um timer Pomodoro funcional e intuitivo.

Integrar música de foco (lo-fi) via playlists do YouTube.

Oferecer experiências visuais temáticas (oceânica, espacial, etc.).

Ser acessível em dispositivos desktop e mobile.

3. Funcionalidades Principais
Funcionalidade	Descrição
Timer Pomodoro	Ciclos de 25min (trabalho) e 5min (descanso) com controles de início/pausa/reset
Player Integrado do YouTube	Reprodução automática de playlists pré-configuradas
Temas Visuais	Opções de temas imersivos (oceânico, espacial, etc.) com animações personalizadas
Interface Responsiva	Adaptação a diferentes tamanhos de tela
Efeitos Sonoros	Notificações auditivas nas transições entre ciclos
Personalização	Ajuste de volumes, tempos de ciclo e seleção de playlists
4. Requisitos Técnicos
4.1 Tecnologias Utilizadas
Frontend: HTML5, CSS3, JavaScript (Vanilla)

APIs: YouTube IFrame Player API

Bibliotecas: Font Awesome (ícones)

Hospedagem: Servidor web estático (local ou remoto)

4.2 Pré-requisitos
Navegador moderno (Chrome, Firefox, Edge)

Conexão com internet (para integração com YouTube)

5. Arquitetura do Sistema
mermaid
Copy
flowchart TD
    A[Interface] --> B(Timer Pomodoro)
    A --> C(Player YouTube)
    A --> D(Temas Visuais)
    B --> E[Controle de Ciclos]
    C --> F[API YouTube]
    D --> G[Animações CSS]
6. Temas Disponíveis
6.1 Oceânico
Elementos: Bolhas animadas, plantas marinhas, gradientes azulados.

Interação: Fundo muda de cor entre ciclos (azul → verde).

6.2 Espacial
Elementos: Estrelas cadentes, planetas pulsantes, efeitos neon.

Interação: Efeitos de propulsão ao iniciar o timer.

7. Manual do Usuário
7.1 Configuração Inicial
Substitua o ID da playlist do YouTube no código (variável list).

Hospede os arquivos em um servidor web.

7.2 Controles
Iniciar: Inicia a contagem regressiva.

Pausar: Congela o timer.

Resetar: Reinicia para o ciclo padrão.

Volume: Ajuste diretamente no player do YouTube.

7.3 Personalização
Temas: Altere as variáveis CSS em :root.

Tempos: Modifique workDuration e breakDuration no JavaScript.

8. Estrutura do Código
plaintext
Copy
pomodoro/
├── index.html          # Estrutura principal
├── style.css           # Estilos e animações
└── script.js           # Lógica do timer + integração YouTube
9. Testes e Validação
Caso de Teste	Resultado Esperado
Ciclo completo (25min)	Transição automática para descanso com notificação
Pausa durante contagem	Timer congela no tempo restante
Troca de playlist	Player carrega nova playlist sem recarregar a página
Acesso mobile	Interface se adapta a telas menores
10. Melhorias Futuras
Sistema de Login: Salvar preferências do usuário.

Novos Temas: Floresta, Cyberpunk, Retrô.

Estatísticas: Gráficos de produtividade.

Extensão para Navegador: Acesso rápido.

11. Referências
YouTube IFrame Player API Documentation

Técnica Pomodoro (Francesco Cirillo)

Paletas de cores: Coolors.co

12. Contribuição
Para contribuir com o projeto:

Faça um fork do repositório.

Adicione novos temas ou funcionalidades.

Envie um pull request com as mudanças.

Equipe: 
Versão: 2.0 (Multi-Tema)
Licença: MIT (Livre para uso e modificação)
