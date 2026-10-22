# Controle Geral (antes "Controle GLP")

Páginas estáticas publicadas na Vercel em https://controle-geral-mann-exata.vercel.app/ (o endereço antigo controle-glp.vercel.app continua funcionando; publica sozinha a cada envio para o GitHub). O endereço raiz abre o **Controle Geral** (`painel.html`) pelo redirecionamento do `vercel.json`.

- `painel.html`: Controle Geral (página inicial): custos, quilometragem, utilização, manutenção, tratamentos HT, suportes e Configurações (usuários, operadores, veículos).
- `index.html`: Controle GLP e Dedetização (OS). Abre dentro do Controle Geral (iframe, `?embed=1`) e usa a mesma sessão; `#ordemservico` mostra só a Dedetização e o resto só o Controle GLP.
- Banco: Supabase `vjbyyjfmilmeyzeiinxf`. Cada pessoa tem login e senha próprios (cadastrados em Configurações) e o banco libera só as abas permitidas (RLS). Não existe mais login único da equipe.
- O Controle de Curvas saiu daqui e tem repositório e link próprios: github.com/felipe10trentini-oss/controle-curvas → https://controle-curvas.vercel.app/. O `vercel.json` redireciona o endereço antigo `/curvas.html` para lá; não recriar `curvas.html` neste repositório.

## Dois computadores mexem neste projeto

O GitHub é a cópia oficial. Para um computador nunca apagar o trabalho do outro:

1. **Antes de qualquer alteração:** `git pull` (se a pasta não existir, `git clone https://github.com/felipe10trentini-oss/Controle-GLP.git`).
2. **Logo depois de cada alteração pronta:** `git add`, `git commit` e `git push` — sem esperar o fim do dia. O push já publica na Vercel.
3. Nunca enviar arquivos pelo "Add files via upload" do GitHub a partir de uma cópia antiga: baixe a versão atual antes, ou use o git.
4. Se o `git pull` der conflito, pare e pergunte ao usuário qual versão vale.