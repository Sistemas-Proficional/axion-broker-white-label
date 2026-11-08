# Configuração do repositório AXION

## Conteúdo

- Três apresentações completas: português, espanhol e inglês.
- Escopo e FAQ nos três idiomas.
- Duas capturas AXION originais, com legendas por idioma.
- Contato para orçamento: [WhatsApp +55 11 91253-6227](https://wa.me/5511912536227).
- [Glossário](docs/keyword-glossary.md) com 60 termos únicos, incluindo todas as 51 tags solicitadas e os termos da referência.

## Campo About e Topics

Os arquivos abaixo registram a configuração desejada, mas não alteram o campo About automaticamente:

- [Descrição e endereço sugeridos](.github/repository-metadata.json).
- [20 tópicos selecionados](.github/topics.json).

O limite do GitHub é de 20 tópicos por repositório. A seleção contém os 19 tópicos da referência mais `binary-options`. As outras tags estão no glossário.

### Aplicar pela interface

Na página principal do repositório, abrir a engrenagem ao lado de **About**, cadastrar os tópicos de `.github/topics.json` e salvar em **Save changes**.

### Aplicar por GitHub CLI

Depois de autenticar o GitHub CLI na conta proprietária, executar na raiz do repositório:

```sh
gh api --method PUT repos/Sistemas-Proficional/axion-broker-white-label/topics --input .github/topics.json
```

Depois, conferir o resultado no campo About ou pela API. A gravação de arquivos de documentação não equivale à aplicação desses metadados.

## Estrutura

```text
README.md
README.es.md
README.en.md
CONTACT.md
assets/
  axion-landing-page.png
  axion-binary-options-demo.png
docs/
  keyword-glossary.md
  pt/
    escopo-e-integracoes.md
    perguntas-frequentes.md
  es/
    alcance-e-integraciones.md
    preguntas-frecuentes.md
  en/
    scope-and-integrations.md
    frequently-asked-questions.md
.github/
  topics.json
  repository-metadata.json
PUBLISHING.md
```

## Referência visual

As imagens originais foram fornecidas pelo desenvolvedor. Elas apresentam a página institucional AXION e o terminal de opções binárias em conta demo. A documentação descreve o material disponível e organiza os itens que dependem do escopo contratado.
