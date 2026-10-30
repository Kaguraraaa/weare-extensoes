# WeAre! — extensões / extensions

> 🇧🇷 [Português](#português) · 🇺🇸 [English](#english)

---

## Português

Repositório de extensões do **WeAre!**, um leitor de mangás que mantenho para **uso pessoal**.
É um projeto de hobby e **não é um serviço para o público em geral**: não há suporte, garantia de
funcionamento nem cronograma de atualizações. Se você chegou aqui procurando extensões, use os
repositórios da comunidade — em especial o [Keiyoushi](https://github.com/keiyoushi/extensions-source).

### Por que existe

Às vezes uma fonte quebra (o site muda o HTML, o domínio ou o formato dos dados) e a correção
oficial demora. Aqui ficam só as extensões que corrigi para o meu próprio uso, até que a versão da
comunidade volte a funcionar.

### O que tem aqui

| Extensão | Versão | Mudança em relação à original |
|---|---|---|
| MangaDash (pt-BR) | 1.6.1 | Mensagem clara em obra +18 sem login (antes: erro `null`); no servidor (Suwayomi) avisa que capítulos em PDF só abrem no Android (antes: `Stub!`). |

- `apk/` — extensões para Android (Mihon e derivados).
- `jar/` — as mesmas extensões já convertidas para o Suwayomi (servidor), que não consegue converter APKs gerados pelas ferramentas atuais.
- `index.pb` + `repo.json` — índice no formato de repositório do Mihon/Suwayomi.
- `alteracoes/` — diff exato das mudanças sobre o código original.

### Detalhes técnicos

- O pacote usa o prefixo `app.weare.extension.*` para não colidir com a assinatura da extensão
  original. O **id da fonte é o mesmo**, então obras salvas continuam ligadas — mas é preciso
  desinstalar a versão original antes de instalar esta.
- Assinatura própria. Impressão digital SHA-256 do certificado:
  `c8f970b9b95b1119fd0cea4808fbc9d318b6d4662ebf600005f5e6713c8abb31`.
- Não contorno CAPTCHA, Cloudflare, login ou paywall, e não adiciono fontes que exijam isso.

### Créditos e licença

Código derivado do [keiyoushi/extensions-source](https://github.com/keiyoushi/extensions-source)
(Apache-2.0), commit `dbf6c05`. Todo o mérito do código das fontes é dos mantenedores originais;
as mudanças estão em `alteracoes/`. Distribuído sob a mesma licença — veja `LICENSE` e `NOTICE`.
Este projeto não tem relação com o Keiyoushi, o Mihon, o Suwayomi ou os sites das fontes.

---

## English

Extension repository for **WeAre!**, a manga reader I maintain for **personal use**.
It is a hobby project and **not a service for the general public**: no support, no guarantee that
anything works, no update schedule. If you are looking for extensions, use the community
repositories — especially [Keiyoushi](https://github.com/keiyoushi/extensions-source).

### Why it exists

Sometimes a source breaks (the site changes its HTML, domain or data format) and the official fix
takes a while. This repository only holds the extensions I patched for my own use, until the
community version works again.

### What's inside

| Extension | Version | Change from the original |
|---|---|---|
| MangaDash (pt-BR) | 1.6.1 | Clear message for 18+ titles without login (was: `null` error); on the server (Suwayomi) it says PDF chapters only open on Android (was: `Stub!`). |

- `apk/` — extensions for Android (Mihon and forks).
- `jar/` — the same extensions pre-converted for Suwayomi (server), which cannot convert APKs built by current tooling.
- `index.pb` + `repo.json` — index in the Mihon/Suwayomi repository format.
- `alteracoes/` — exact diff of the changes over the original code.

### Technical notes

- Packages use the `app.weare.extension.*` prefix so they don't clash with the original extension's
  signature. The **source id is unchanged**, so saved titles stay linked — but the original
  extension must be uninstalled first.
- Own signing key. Certificate SHA-256 fingerprint:
  `c8f970b9b95b1119fd0cea4808fbc9d318b6d4662ebf600005f5e6713c8abb31`.
- No CAPTCHA, Cloudflare, login or paywall circumvention, and no sources that require it.

### Credits and license

Derived from [keiyoushi/extensions-source](https://github.com/keiyoushi/extensions-source)
(Apache-2.0), commit `dbf6c05`. All credit for the source code goes to the original maintainers;
the changes are in `alteracoes/`. Distributed under the same license — see `LICENSE` and `NOTICE`.
This project is not affiliated with Keiyoushi, Mihon, Suwayomi or any of the source websites.
