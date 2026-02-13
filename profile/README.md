# nextime-frame – Sistema de Processamento de Vídeos
Bem-vindo à organização **nextime-frame**, onde desenvolvemos uma solução moderna, escalável e baseada em serviços AWS para processamento de vídeos, criada no contexto do desafio **FIAP X**.

Nosso objetivo é permitir que usuários façam upload de vídeos, acompanhem o status do processamento e realizem o download das imagens extraídas em um arquivo `.zip`, tudo de forma segura, resiliente e preparada para alta demanda.

O projeto evolui um protótipo simples apresentado a investidores, transformando-o em uma aplicação robusta, utilizando boas práticas de arquitetura de software, microsserviços e computação em nuvem.

---

## Visão Geral do Projeto

O **nextime-frame** é um sistema distribuído de processamento de vídeos que permite o processamento simultâneo de múltiplos arquivos, garantindo confiabilidade mesmo em cenários de pico.

A solução foi desenhada para operar integralmente na **AWS**, utilizando serviços gerenciados para garantir escalabilidade, segurança e observabilidade.

O fluxo principal consiste em:
1. Upload de vídeo pelo usuário
2. Enfileiramento da solicitação
3. Processamento assíncrono frame a frame
4. Compactação das imagens geradas em `.zip`
5. Disponibilização do arquivo final para download
6. Notificação do usuário em caso de sucesso ou erro

---

## Arquitetura do Projeto

![Arquitetura](https://res.cloudinary.com/dqvkg85dl/image/upload/v1771021155/arquitetura_njp3uo.gif)

## Principais Funcionalidades

- **Processamento Paralelo de Vídeos**  
  Suporte a múltiplos vídeos sendo processados simultaneamente, garantindo escalabilidade horizontal.

- **Alta Resiliência e Confiabilidade**  
  Uso de mensageria para garantir que nenhuma requisição seja perdida, mesmo em picos de acesso.

- **Autenticação e Autorização**  
  Proteção do sistema por autenticação via usuários, garantindo segurança e isolamento de dados.

- **Acompanhamento de Status**  
  O usuário pode visualizar todos os seus vídeos enviados e acompanhar o status de cada processamento.

- **Notificações Automatizadas**  
  Em caso de erro ou conclusão do processamento, o usuário é notificado por e-mail.

- **Persistência de Dados**  
  Todas as informações do fluxo são armazenadas em banco de dados NoSQL, garantindo histórico e rastreabilidade.

---

## Arquitetura e Tecnologias

O projeto utiliza uma arquitetura orientada a eventos, baseada em microsserviços e totalmente integrada ao ecossistema AWS.

### Stack Tecnológica

#### ☁️ Cloud & Infraestrutura (AWS)
- **API Gateway** – Exposição segura das APIs
- **Amazon Cognito** – Autenticação e gerenciamento de usuários
- **Amazon SQS** – Mensageria e processamento assíncrono
- **Amazon EKS** – Orquestração de containers
- **Amazon SES** – Envio de notificações por e-mail
- **IAM** – Gerenciamento de permissões e segurança

#### 💾 Persistência
- **MongoDB (NoSQL)** – Armazenamento dos dados de vídeos, status e usuários

#### 🐳 Ambiente Local
- **Docker**
- **LocalStack** – Simulação dos serviços AWS localmente

#### 📊 Observabilidade
- **Datadog** – Monitoramento, métricas, logs e alertas

#### 🔄 DevOps
- **GitHub** – Versionamento do código
- **GitHub Actions** – CI/CD para build, testes e deploy

---

## Qualidade e Boas Práticas

- Arquitetura de microsserviços
- Processamento assíncrono orientado a eventos
- Uso de filas para desacoplamento
- Testes automatizados
- Pipeline de CI/CD
- Infraestrutura escalável e observável
- Documentação técnica e arquitetural

---

## Entregáveis do Projeto

### 📄 Documentação
- Documentação completa da arquitetura
- Diagramas de fluxo e componentes
- Scripts de criação de banco de dados e infraestrutura

### 💻 Código
- Repositórios versionados no GitHub
- Código organizado seguindo boas práticas

### 🎥 Apresentação
- Vídeo de até **10 minutos**, apresentando:
  - Documentação do projeto
  - Arquitetura escolhida
  - Demonstração do sistema em funcionamento

---

## Como Contribuir

Atualmente, o projeto **nextime-frame** não está aceitando contribuições externas, pois faz parte de um escopo acadêmico controlado.  
Agradecemos o interesse e o apoio.

---

## Equipe

A equipe **nextime-frame** é formada por desenvolvedores comprometidos com boas práticas de arquitetura, cloud computing e qualidade de software.

<div style="text-align: center;">
<table>
  <tr>
    <td style="text-align: center;">
      <img src="https://avatars.githubusercontent.com/Fernandeess" alt="Avatar Matheus Fernandes Rodrigues" width="100" style="border-radius: 50%;" /><br/>
      <sub><b>Matheus Fernandes Rodrigues</b></sub><br/>
      <sub>Fernandeess</sub>
    </td>
    <td style="text-align: center;">
      <img src="https://avatars.githubusercontent.com/leobr1t0" alt="Avatar Leonardo Brito de Oliveira" width="100" style="border-radius: 50%;" /><br/>
      <sub><b>Leonardo Brito de Oliveira</b></sub><br/>
      <sub>leobr1t0</sub>
    </td>
    <td style="text-align: center;">
      <img src="https://avatars.githubusercontent.com/lokoabners" alt="Avatar Erick Abner de Lourdes" width="100" style="border-radius: 50%;" /><br/>
      <sub><b>Erick Abner de Lourdes</b></sub><br/>
      <sub>lokoabners</sub>
    </td>
    <td style="text-align: center;">
      <img src="https://avatars.githubusercontent.com/MarceloACJunior" alt="Avatar Marcelo Alcantara" width="100" style="border-radius: 50%;" /><br/>
      <sub><b>Marcelo Alcantara</b></sub><br/>
      <sub>MarceloACJunior</sub>
    </td>
  </tr>
</table>
</div>

---

## Licença

Este projeto é licenciado sob a **Licença MIT**.

Obrigado por acompanhar o desenvolvimento do **nextime-frame** 🚀  
Estamos transformando processamento de vídeos em uma solução cloud-native, escalável e pronta para produção.
