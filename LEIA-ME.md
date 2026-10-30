# Agenda v2 (app instalável, ligada ao GitHub)

1. **Código da app (repositório público, sem dados):** crie um repositório público `agenda-app`, envie estes 5 ficheiros
   (`index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`) e ative *Settings → Pages →
   Deploy from a branch → main / (root)*. O endereço fica `https://SEU-UTILIZADOR.github.io/agenda-app/`.
2. **Token:** GitHub → Settings → Developer settings → Fine-grained tokens → *Generate*. Repositório: **só** `regibox-sync`
   (o privado). Permissão: *Contents → Read and write*. Validade curta (por exemplo 90 dias). Nunca o partilhe: quem o tiver lê
   os nomes dos alunos.
3. **Repositório privado:** substitua `collector.py`, `config.json`, `README.md` e `.github/workflows/sync.yml` pelos do zip `regibox-sync`.
4. **No telemóvel:** abra o endereço da app no Chrome, menu ⋮ → *Instalar app*. Em *Definições* escreva `SEU-UTILIZADOR/regibox-sync`,
   cole o token e guarde. Para passar os dados da v1: copie o texto da cópia de segurança da v1 e restaure-o na v2.
5. Em *Tipos de aula*, marque o "Open Box" como *sem pagamento* e crie as suas entradas Open Box na agenda.

A v1 continua a funcionar sem alterações. A agenda grava-se no GitHub ~4 segundos após cada alteração, o que dispara a sincronização com
o Regibox; depois de 1 a 2 minutos, toque em *Atualizar Regibox*. Funciona offline com os últimos dados.
