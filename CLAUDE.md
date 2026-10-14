# Controle GLP

Página única (`index.html`) publicada na Vercel em https://controle-glp.vercel.app/ (publica sozinho a cada envio para o GitHub).

- Banco: Supabase `vjbyyjfmilmeyzeiinxf`, login único da equipe (e-mail e senha).
- O Controle de Curvas saiu daqui e tem repositório e link próprios: github.com/felipe10trentini-oss/controle-curvas → https://controle-curvas.vercel.app/. O `vercel.json` redireciona o endereço antigo `/curvas.html` para lá; não recriar `curvas.html` neste repositório.

## Dois computadores mexem neste projeto

O GitHub é a cópia oficial. Para um computador nunca apagar o trabalho do outro:

1. **Antes de qualquer alteração:** `git pull` (se a pasta não existir, `git clone https://github.com/felipe10trentini-oss/Controle-GLP.git`).
2. **Logo depois de cada alteração pronta:** `git add`, `git commit` e `git push` — sem esperar o fim do dia. O push já publica na Vercel.
3. Nunca enviar arquivos pelo "Add files via upload" do GitHub a partir de uma cópia antiga: baixe a versão atual antes, ou use o git.
4. Se o `git pull` der conflito, pare e pergunte ao usuário qual versão vale.
