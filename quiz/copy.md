# 40 Dias de Restauração com Santa Mônica

Versão ativa: `index.html`, independente, com CSS, JavaScript, ilustração e fontes incorporados. Cópia para upload: `output/santa-monica.html` na raiz do repositório. O quiz original do framework está em `_backup_v1/`; a primeira versão de Santa Mônica, com painel lateral, foi preservada em `_backup_v2/`.

## Estrutura

As 11 telas seguem a sequência fornecida pelo usuário: abertura; situação emocional; intenção; tempo da espera; apoio; história da santa; pedido escrito; oração com áudio; prontidão; preparação; resultado e oferta.

O nome opcional fica na prontidão, depois do áudio, para manter 11 telas. Uma pergunta por tela, alternativas que avançam com um toque, progresso, transições com respeito a movimento reduzido e resultado com nome, intenção, disposição e pedido escrito. Respostas ficam somente na memória da página.

## Identidade e conteúdo

A revisão visual usa fundo creme liso, coluna central de 356 px úteis nas perguntas, logo compacto, fonte Poppins e botões azul-petróleo. Os textos do quiz foram encurtados e o painel lateral foi removido. O dourado aparece discretamente no selo original. A oferta usa cartões separados, mais largos, para facilitar a leitura. Selo vetorial original com ramos de oliveira e chama; ilustração original de Santa Mônica. Textos e orações originais, sem depoimentos, preços de referência ou promessas de conversão.

O livro da jornada é **O Caminho das Lágrimas: 40 Dias de Intercessão com Santa Mônica**. Os 40 dias seguem exatamente as fases do PDF: **As lágrimas sinceras**, **A força da persistência**, **O exemplo de vida** e **A entrega confiante**, com dez dias em cada fase. A identidade e a nomenclatura para página, checkout e anúncios estão em `produto/identidade-oferta.md`.

A oferta anuncia um único PDF com 40 encontros de três páginas, ilustrações, reflexão, orações tradicionais completas, 40 preces originais diferentes, prática e diário integrado. A oração dirigida a Santa Mônica aparece na abertura e no Dia 40, rotulada como texto original do livro. Diário e preces são componentes do mesmo PDF, sem bônus avulsos prometidos.

A caixa de apoio apresenta CVV 188 (gratuito, 24 horas), CAPS AD (cuidado gratuito pelo SUS; localização pela UBS) e SAMU 192 (emergências de saúde, gratuito, 24 horas). Fontes do CVV e do Ministério da Saúde verificadas em 1º de novembro de 2026; não se apresenta CVV como atendimento de emergência.

## Pendências confirmadas pelo usuário

Preço, garantia e prazo de acesso serão definidos depois. Checkout próprio e áudio também aguardam envio. Nenhuma compra é iniciada enquanto preço e checkout não forem configurados. Quando houver áudio, o avanço fica bloqueado até o evento real de término da reprodução. Enquanto não houver arquivo, a oração escrita permite revisar o fluxo.

Tudo é editado no objeto `CONFIGURACAO`, dentro do próprio HTML. Campos: `audioURL`, `checkoutURL`, `precoBRL`, `garantiaDias`, `acessoDias`, `vendedor`, `suporteEmail`, `entregaveis`. O áudio pode ser incorporado em base64 para manter o arquivo único. A transcrição da tela de oração deve corresponder à gravação final.

## Pesquisa histórica

- Santa Sé, Angelus de 30/08/2009: https://www.vatican.va/content/benedict-xvi/pt/angelus/2009/documents/hf_ben-xvi_ang_20090830.html
- Santa Sé, audiência de 09/01/2008: https://www.vatican.va/content/benedict-xvi/en/audiences/2008/documents/hf_ben-xvi_aud_20080109.html

## Verificação

Navegação completa das 11 telas e dos seis resultados; nome e pedido opcionais; rejeição de nome inválido; pedido exibido como texto; bloqueio do áudio com WAV real de teste; checkout configurado validado com rota simulada; estado pendente sem cobrança; navegação de volta; reinício; nove perguntas frequentes; larguras entre 320 e 1440 pixels sem transbordamento horizontal; sem erros de JavaScript ou recursos externos necessários. Nenhum deploy foi realizado.

## Revisão visual solicitada

Os prints orientaram proporções e espaçamento, mantendo textos, imagens e selo originais. As escolhas avançam automaticamente; o botão de retorno permite alterar respostas. O player de áudio tem reprodução e pausa, tempo decorrido e bloqueio de avanço até a conclusão quando houver gravação. Sem áudio, a oração escrita fica em um painel expansível. O HTML continua independente. A revisão foi gerada com `work/build_clean.py`.


## Revisão de iconografia e relato autorizado

A abertura usa uma representação original de Santa Mônica como viúva, com véu e manto escuros e um livro nas mãos. A etapa histórica usa outra composição, horizontal, adaptada da imagem enviada pelo usuário, sem cajado e com roupa escura. A miniatura do livro usa a mesma arte da nova capa do PDF. O player de áudio usa um símbolo de cruz, sem repetir o retrato. As imagens ficam incorporadas em SVG com recortes nativos; o HTML continua independente.

O relato sobre oração e diálogo no casamento foi incluído em texto, com trechos fiéis ao print. O usuário confirmou ser de uma cliente real da oferta e ter autorização de publicação. A foto original aguarda o print em arquivo JPG/PNG para incorporação sem alteração. Não foram criados nomes, avaliações, estatísticas ou fotos de clientes.

O arquivo de áudio MP3 ainda não foi enviado. O player mantém o bloqueio real até o término quando um áudio for configurado.
