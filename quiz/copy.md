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

Preço, garantia e prazo de acesso serão definidos depois. O checkout próprio aguarda definição. O MP3 do ElevenLabs já está incorporado. Nenhuma compra é iniciada enquanto preço e checkout não forem configurados. O avanço fica bloqueado até a reprodução terminar ou a pessoa mover a faixa até o fim do MP3. A transcrição enviada pelo usuário aparece em “Ler a oração”, sem personalização que a afaste do áudio.

Tudo é editado no objeto `CONFIGURACAO`, dentro do próprio HTML. Campos: `audioURL`, `checkoutURL`, `precoBRL`, `garantiaDias`, `acessoDias`, `vendedor`, `suporteEmail`, `entregaveis`. O áudio pode ser incorporado em base64 para manter o arquivo único. A transcrição da tela de oração deve corresponder à gravação final.

## Pesquisa histórica

- Santa Sé, Angelus de 30/08/2009: https://www.vatican.va/content/benedict-xvi/pt/angelus/2009/documents/hf_ben-xvi_ang_20090830.html
- Santa Sé, audiência de 09/01/2008: https://www.vatican.va/content/benedict-xvi/en/audiences/2008/documents/hf_ben-xvi_aud_20080109.html

## Verificação

Navegação completa das 11 telas e dos seis resultados; nome e pedido opcionais; rejeição de nome inválido; pedido exibido como texto; bloqueio do áudio com WAV real de teste; checkout configurado validado com rota simulada; estado pendente sem cobrança; navegação de volta; reinício; nove perguntas frequentes; larguras entre 320 e 1440 pixels sem transbordamento horizontal; sem erros de JavaScript ou recursos externos necessários. Nenhum deploy foi realizado.

## Revisão visual solicitada

Os prints orientaram proporções e espaçamento, mantendo textos, imagens e selo originais. As escolhas avançam automaticamente; o botão de retorno permite alterar respostas. O player de áudio tem reprodução e pausa, tempo decorrido e bloqueio de avanço até a conclusão quando houver gravação. Sem áudio, a oração escrita fica em um painel expansível. O HTML continua independente. A revisão foi gerada com `work/build_clean.py`.


## Revisão de iconografia e relato autorizado

A abertura usa uma representação original de Santa Mônica como viúva, com véu e manto escuros e um livro nas mãos. A etapa histórica usa outra composição, horizontal, adaptada da imagem enviada pelo usuário, sem cajado e com roupa escura. A miniatura do livro usa a mesma arte da nova capa do PDF. O player usa a foto ilustrativa do sacerdote enviada em arquivo pelo usuário, acompanhada da identificação de narração gerada por IA. As imagens ficam incorporadas em SVG com recortes nativos; o HTML continua independente.

O print original do casal foi incorporado ao bloco final de compra, com trechos em texto dentro de um painel expansível para facilitar a leitura. O usuário confirmou ser de uma cliente real da oferta e ter autorização de publicação. A imagem foi convertida para WebP sem perdas, com igualdade dos pixels verificada em relação ao PNG recebido no ZIP. Não foram criados nomes, avaliações, estatísticas ou fotos de clientes.

O MP3 recebido foi incorporado sem alterações de bytes. A duração é de aproximadamente 1 minuto e 23 segundos. O player reproduz, pausa, mostra tempo atual e duração, e permite avançar ou retroceder pela faixa. A próxima etapa libera ao terminar a reprodução ou ao posicionar a faixa no fim.


## Ajuste do bloco final de compra

A abertura recebeu um retrato de Santa Mônica com expressão acolhedora, sorriso discreto e iluminação mais clara, mantendo véu e manto escuros. O relato foi movido para dentro do cartão final de compra, depois das perguntas frequentes, imediatamente antes do preço e do único botão de checkout. A imagem original do print está incluída; a autorização do casal já foi confirmada pelo usuário.


## Integração dos arquivos recebidos

O HTML contém o print original, o MP3, a foto ilustrativa do sacerdote e a transcrição exata fornecida pelo usuário. A narração é identificada como gerada por IA, sem atribuição de gravação ao sacerdote. A foto original do casal teve seus pixels preservados integralmente. Todos os recursos estão incorporados no HTML, sem requisições externas para funcionar.

Verificação com o MP3 real: reprodução e pausa; bloqueio mantido antes do fim; liberação no fim por reprodução ou navegação pela faixa; transcrição conferida; avatar carregado; print antes do checkout; larguras 320, 390 e 737 px; sem erros de JavaScript. O teste de reprodução usou velocidade acelerada apenas no navegador de teste; o arquivo e a velocidade padrão entregue continuam originais.


A faixa permite clique, arraste e navegação por teclado. O progresso aparece nas ondas e no tempo decorrido. O aviso de voz gerada por IA e foto ilustrativa fica dentro de “Ler a oração”, oculto enquanto o painel está fechado.
