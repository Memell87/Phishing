# Phishing
Phishing com Kali Linux
Neste desafio, simulei um ataque de Phishing utilizando a ferramenta Social-Engineer Toolkit (SET) dentro do ecossistema Kali Linux. O objetivo principal foi entender na prática como ataques de engenharia social funcionam para aprender a mitigar essas vulnerabilidades em aplicações reais.

🛠 Ferramentas Utilizadas
Sistema Operacional: Kali Linux (via VM/VirtualBox)

Ferramenta: Social-Engineer Toolkit (SET)

Linguagens: HTML e JavaScript para o front-end customizado.

🚀 Passo a Passo Realizado
1. Preparação do Ambiente
Certifiquei-me de que o Kali Linux estava atualizado.

Criei um diretório local para armazenar o código do site customizado: mkdir ~/meu_teste_web.

2. Criação do Front-end Customizado
Em vez de utilizar o "Site Cloner" automático (que pode gerar erros de decodificação UTF-8 em sites complexos como o Facebook), desenvolvi um arquivo index.html simplificado.

Objetivo: Garantir que o servidor do SET capture os campos email e password com 100% de precisão.

Funcionalidade Extra: Implementei um script manual de Tabnabbing que altera o conteúdo da página quando o usuário troca de aba no navegador.

3. Configuração do SET
No terminal do Kali, executei o setoolkit e segui o fluxo:

Social-Engineering Attacks -> Opção 1

Website Attack Vectors -> Opção 2

Credential Harvester Attack Method -> Opção 3

Custom Import -> Opção 3

Defini o IP da máquina local e o caminho da pasta onde salvei o index.html.

4. Execução e Captura
Acessei o IP local através de um navegador simulando a vítima.

Inseri credenciais de teste (ex: teste@email.com e senha123).

O terminal do SET exibiu com sucesso os dados capturados em texto claro, sem erros de decodificação.

📊 Resultados Obtidos
Através do método de Custom Import, consegui:

Evitar erros de UnicodeDecodeError comuns em sites modernos.

Capturar credenciais de forma limpa e organizada no terminal.

Entender a importância de headers de segurança e validações no lado do cliente para evitar ataques de redirecionamento.

⚠️ Aviso Legal
Este projeto foi desenvolvido estritamente para fins educativos e acadêmicos, seguindo as diretrizes da plataforma DIO. O uso dessas técnicas em cenários reais sem autorização é ilegal e antiético.
