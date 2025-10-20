📱 # AppConsultoriaADV

<img width="1025" height="580" alt="image" src="https://github.com/user-attachments/assets/00dd442e-1b50-4782-ba10-bc9a66af0d91" />

<img width="1304" height="532" alt="image" src="https://github.com/user-attachments/assets/ef7eb632-690d-4f10-bf48-3198e2d0ac3d" />

<img width="976" height="702" alt="image" src="https://github.com/user-attachments/assets/eef965e7-104f-49f7-800d-d43c3fbdc898" />




Aplicativo Android desenvolvido em Kotlin com Jetpack Compose, voltado para automatizar o atendimento e o acompanhamento de processos jurídicos de um escritório de advocacia.
O projeto foi desenvolvido com arquitetura moderna, integração com API REST e persistência de dados local, garantindo performance, escalabilidade e experiência fluida ao usuário,atuei como responsável pela integração completa do aplicativo tendo também atuado para front-end.

⚙️ Principais Tecnologias Utilizadas:

🧩 Linguagem e Framework

* Kotlin – Linguagem principal, com uso extensivo de coroutines e flows para operações assíncronas.
* Jetpack Compose – Framework declarativo de UI, utilizado em todas as telas (Login, Home, Perfil, Notificações, Chat, etc.).

🏗️ Arquitetura

* MVVM (Model-View-ViewModel) – Organização das camadas de lógica, estado e interface, separando responsabilidades.
* Repository Pattern – Camada intermediária para comunicação entre o ViewModel e a API (Retrofit).
* StateFlow / MutableStateFlow – Controle reativo de estados e atualizações de UI.

🌐 Comunicação com a API
* Retrofit + OkHttp – Consumo da API REST hospedada em servidor.

💬 Comunicação em Tempo Real

* Socket.IO (WebSocket) – Implementado via ChatSocketManager para envio e recepção instantânea de mensagens.
* Atualização de UI em tempo real utilizando StateFlow e LazyColumn com auto-scroll.

🔐 Persistência e Sessão

* DataStore – Armazenamento local e seguro de tokens, CPF, ID e dados de sessão do usuário.
* TokenStorage / SharedUserViewModel – Recuperação automática dos dados após login e persistência global no app.

💉 Injeção de Dependência
* Hilt (Dagger) – Configuração completa de dependency injection para ViewModels, Repositórios e Retrofit.

🧠 Gerenciamento de Estado e UI

* Navegação por rotas usando @Serializable (Kotlinx Serialization).
* Componentes composables reutilizáveis: CustomButton, InputField, UploadBox, ChatBubble, etc.
* Tratamento visual de loading, erro e sucesso com LaunchedEffect e toasts personalizados.
* 
🧾 Persistência Temporária e Mock
* Uso de mock de mensagens e dados locais em etapas de testes antes da integração final com o backend.

  
