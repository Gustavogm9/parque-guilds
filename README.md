# ParqueOS · Protótipo protegido

Protótipo navegável do ParqueOS (Parque Tecnológico de S. J. do Rio Preto), criptografado com StatiCrypt.

- URL: https://parque.guilds.com.br
- Senha: parque-2026

## Como publicar (manual, 1ª vez)

1. Criar repo e subir esta pasta:
   gh repo create parque-guilds --public --source . --push
   (ou git init + remote + push normal)
2. GitHub → Settings → Pages → Deploy from branch (main, /root)
3. DNS (Wix): CNAME `parque` → `SEU-USUARIO.github.io`
4. Aguardar o certificado HTTPS do Pages (alguns minutos)

## Atualizar o protótipo

Recriptografar e substituir o index.html:
npx staticrypt parqueos_prototipo.html -p "parque-2026" --short -o index.html
