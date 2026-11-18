[← Voltar ao Portfólio Central](../index.html)

---

# Guia de Comandos Git e GitHub

Resumo prático dos principais comandos do Git e o passo a passo para versionar e enviar alterações para o GitHub.

---

## 1. Configuração Inicial

Antes de fazer o primeiro commit em um computador, configure seu nome e e-mail (os mesmos da sua conta no GitHub):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

---

## 2. Principais Comandos

| Comando | Explicação Breve |
| :--- | :--- |
| `git init` | Inicializa um novo repositório Git na pasta atual. |
| `git clone <url>` | Clona (baixa) um repositório remoto do GitHub para o seu computador. |
| `git status` | Mostra quais arquivos foram modificados, criados ou estão prontos para commit. |
| `git add <arquivo>` | Adiciona um arquivo específico à área de preparação (*Staging Area*). |
| `git add .` | Adiciona **todos** os arquivos novos e modificados à área de preparação. |
| `git commit -m "mensagem"` | Salva um ponto na história do projeto local com uma descrição do que foi feito. |
| `git push` | Envia os commits locais para o repositório remoto no GitHub. |
| `git pull` | Baixa e aplica as atualizações mais recentes do GitHub no seu computador. |
| `git log --oneline` | Exibe o histórico resumido dos commits realizados. |
| `git checkout -b <branch>` | Cria uma nova ramificação (*branch*) e muda imediatamente para ela. |

---

## 3. Como Commitar e Enviar para o GitHub

### Fluxo Diário (Repositório já conectado ao GitHub)

1. **Verifique os arquivos alterados:**
   ```bash
   git status
   ```
2. **Prepare os arquivos para o commit:**
   ```bash
   git add .
   ```
3. **Crie o commit com uma mensagem descritiva:**
   ```bash
   git commit -m "Adiciona guia de comandos Git"
   ```
4. **Envie para o GitHub:**
   ```bash
   git push
   ```

### Primeiro Envio (Projeto novo criado localmente)

1. **Inicie o repositório na pasta do projeto:**
   ```bash
   git init
   ```
2. **Adicione os arquivos e registre o primeiro commit:**
   ```bash
   git add .
   git commit -m "Primeiro commit"
   ```
3. **Defina a branch principal como `main`:**
   ```bash
   git branch -M main
   ```
4. **Vincule ao repositório remoto e envie os arquivos:**
   ```bash
   git remote add origin [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
   git push -u origin main
   ```
