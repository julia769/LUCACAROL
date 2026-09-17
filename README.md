Tarefa SP Assistant

Assistente educacional experimental para auxiliar estudantes durante atividades online.

Funcionalidades

Navegador Chromium controlado por Playwright.

Login realizado manualmente pelo usuário.

Leitura do conteúdo da página.

Análise de questões usando IA.

Geração de resposta sugerida.

Explicação do raciocínio.

Indicador de confiança.

Revisão antes de qualquer ação final.

Importante

Este projeto não envia automaticamente atividades escolares.

O usuário deve revisar a resposta e realizar manualmente o envio da atividade.

Requisitos

Python 3.10 ou superior

Google Chromium/Playwright

Chave de API da OpenAI

Instalação

Clone o projeto:

git clone https://github.com/SEU-USUARIO/tarefa-sp-assistant.git
cd tarefa-sp-assistant


Crie um ambiente virtual:

python -m venv .venv


Ative o ambiente.

No Windows:

.venv\Scripts\activate


No Linux/macOS:

source .venv/bin/activate


Instale as dependências:

pip install -r requirements.txt


Instale o navegador do Playwright:

playwright install chromium


Crie o arquivo .env:

cp .env.example .env


No Windows, também é possível simplesmente copiar .env.example para .env.

Depois coloque sua chave de API no arquivo .env.

Executando
python main.py


O navegador será aberto.

Faça o login manualmente e navegue até a atividade.

Depois pressione ENTER no terminal para que o assistente leia a página e gere uma sugestão de resposta.

Estrutura
agent/       → lógica de IA
browser/     → automação do navegador
ui/          → revisão das respostas
tests/       → testes
main.py      → ponto de entrada
config.py    → configuração

Segurança

Nunca coloque sua chave de API diretamente no código.

O arquivo .env está incluído no .gitignore para evitar que credenciais sejam publicadas no GitHub.

Licença

MIT