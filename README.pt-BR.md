# Bootstrap CV example

Site educacional de CV com várias páginas para a persona de exemplo "Rosie Odenkirk", não biografia verificada de Iuri.

[English](README.md)

## Ideia e processo

Código revisado em 01/10/2026. Baseado em template/material do Code Institute. Não foram encontrados planejamento datado, wireframes ou diário original nos arquivos revisados. Dados e afirmações do CV de exemplo não são fatos sobre o dono do repositório.

## Arquitetura e design

Páginas home, resume, contact, interests, GitHub e 404. Assets estáticos fornecem estilos/scripts. Layout de CV de curso, não portfólio pessoal redesenhado.

- `assets/js/github-information.js`: busca dados públicos de usuário/repos por jQuery, trata vazio/404/limite e renderiza HTML.
- `assets/js/maps.js`: cria mapa Google com marcadores demonstrativos e clustering.
- `assets/js/sendEmail.js`: envia nome, email e pedido por EmailJS, registra sucesso/falha no console e bloqueia navegação normal do form.
- package.json inclui `@emailjs/browser` ^3.10.0; contact.html também carrega cliente por CDN.

## Preview local

```bash
python3 -m http.server 8000
```

Abra localhost:8000. Bibliotecas/APIs externas precisam de rede. Não envie formulário com dados pessoais: faz requisição EmailJS externa. Nenhum email, mapa/API, instalação ou aplicação executado aqui; deploy público não confirmado.

## Testes, privacidade e limites

Manifest revisado sem script dedicado de testes. Nada testado. Verifique navegação, 404, responsividade, labels, estados GitHub vazio/erro/limite e renderização segura com dados fictícios. Respostas GitHub são inseridas em HTML; revise escape/URLs. Confirme configuração Maps/EmailJS, destinatário, consentimento e mensagens visíveis de sucesso/erro antes de habilitar contato real. Identificadores do navegador são configuração, não autorização de email ou API paga.

## Capturas

Nenhuma captura verificada/adicionada. Assets futuros datados em docs/assets/ devem identificar este CV fictício e esconder contatos/chaves. Não apresente afirmações da persona como histórico de Iuri.

## Créditos e licença

Material Code Institute e bibliotecas/assets mantêm direitos originais, sem licença nova. README original preservado no [apêndice em inglês](README.md#original-readme), como referência histórica.
