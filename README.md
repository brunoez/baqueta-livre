# Baqueta Livre

Pad de estudo gratuito para bateristas. Roda inteiro no navegador, sem login, sem mensalidade e sem servidor. Os únicos dados guardados são os exercícios que cada pessoa cria, e eles ficam no próprio aparelho.

**Acesse:** https://brunoez.github.io/baqueta-livre/

## O que tem

**Rudimentos**
- Os 40 rudimentos, filtrados por família: rulos, diddles, flams e drags.
- Sticking D/E que acende no tempo, com acentos e notas de graça indicados.
- Escolha da figura rítmica de cada toque: semibreve, mínima, semínima, colcheia, tercina, semicolcheia, sextina, fusa e semifusa, cada uma com o desenho da nota.
- Metrônomo com contagem de 4 tempos, BPM de 40 a 220 e volume separado para direita, esquerda e metrônomo.

**Grooves**
- Mais de 50 ritmos: rock, pop, funk, shuffle, samba, bossa, baião, xote, forró, reggae, eletrônico e metal.
- Grade com cinco linhas coloridas: prato de ataque, prato de condução, chimbal, caixa e bumbo.
- Botão para levar qualquer groove ao Estúdio e editar.

**Estúdio de viradas**
- Grade por peça (ataque, condução, tons, surdo, caixa, chimbal e bumbo) com linha de mão D/E.
- Subdivisão em colcheias, tercinas, semicolcheias ou sextinas, de 1 a 4 compassos.
- Salvar, atualizar, abrir e excluir exercícios.
- Compartilhar um exercício por código de texto (começa com `BL1:`) e importar o de outra pessoa.

**Organização do estudo**
- Cronômetro ou timer (1 a 180 minutos) que só conta enquanto o exercício toca.
- Aumento automático de BPM, por exemplo +5 BPM a cada 1 minuto, até um limite.

**Sons**
- Som dos toques: pad de estudo, caixa, tom, bloco de madeira, cowbell ou aro.
- Bateria acústica ou eletrônica (808).
- Metrônomo: clique, madeira, cowbell, bipe suave ou chimbal.

## Privacidade e armazenamento

Não há contas, cookies de rastreamento, análise de uso nem chamadas a servidores. Os exercícios salvos ficam no `localStorage` do navegador, ligados ao endereço do site. Isso significa:

- Limpar os dados do navegador apaga os exercícios.
- Trocar de aparelho ou de navegador começa do zero. Para levar um exercício, gere o código em *Compartilhar ou importar* e cole no outro aparelho.
- Mudar o endereço do site também faz os exercícios salvos "sumirem" para quem já usava.
- No iPhone, o Safari pode apagar dados de sites que ficam muitos dias sem uso, a menos que o site seja adicionado à tela inicial.

## Como hospedar no GitHub Pages

1. Coloque o arquivo `index.html` na raiz de um repositório público.
2. Abra a aba **Settings** do repositório e depois **Pages**.
3. Em *Build and deployment*, escolha *Deploy from a branch*, a branch `main` e a pasta `/ (root)`, e salve.
4. Aguarde 1 a 2 minutos. O endereço aparece no topo da página.

## Estrutura

```
index.html   # o app completo: HTML, CSS e JavaScript em um único arquivo
README.md
```

Não há dependências nem etapa de build. A única chamada externa é às fontes do Google Fonts, e sem internet o app usa as fontes do aparelho. Todo o áudio é sintetizado no navegador com a Web Audio API, então não há arquivos de som.

## Observações

- Os padrões de sticking dos rudimentos são uma transcrição de referência da lista de 40 rudimentos. Se algum diferir da sua fonte (principalmente entre flams e drags), ajuste os dados no início do script, na lista `RUD_SRC`.
- Os sons são sintetizados e não substituem gravações de bateria real.
- No iPhone, a chave de silenciar pode deixar o áudio mudo.
- Funciona em navegadores atuais com suporte a Web Audio (Chrome, Edge, Firefox e Safari).

## Licença

Defina aqui a licença que preferir (por exemplo, MIT) antes de divulgar o repositório.
