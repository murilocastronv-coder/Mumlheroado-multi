# MU Online na Render (site + multiplayer no mesmo endereço)

## Publicar
1. Copie estes arquivos para a raiz do seu repositório (substituindo `multiplayer-server.js`, `package.json` e a pasta `web/`) e envie ao GitHub.
2. Na Render: **New → Blueprint** (ele lê o `render.yaml`) ou **New → Web Service** com
   Build `npm install` e Start `npm start`.
3. Abra `https://SEU-SERVICO.onrender.com/game.html`. O multiplayer entra sozinho na sala **Lorencia**.

## Importante: o arquivo shell_login.data (219 MB)
No repositório ele é guardado com Git LFS. Se chegar à Render como ponteiro (~130 bytes),
o servidor redireciona automaticamente para a cópia em `SHELL_DATA_URL`
(padrão: a do autor original no GitHub Pages). Para usar a sua, defina essa variável.

## O que o multiplayer faz
Jogadores na mesma sala se veem como avatares sobre o mapa e conversam por chat (painel 🌐).
O mundo do jogo em si (monstros, combate) continua rodando no navegador de cada jogador.

## Plano gratuito da Render
O serviço dorme após ~15 min sem acesso; o primeiro acesso depois disso leva ~30–60 s.
