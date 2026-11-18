# Laudo Corporal

Importa o PDF de uma bioimpedância e gera um laudo de composição corporal no estilo dos
relatórios clínicos (análise de composição, músculo-gordura, obesidade, segmentar, histórico),
exportável em PDF A4 para entregar ao paciente.

## Uso

1. Abra `index.html` no navegador (ou publique no GitHub Pages: Settings → Pages → branch).
2. **Importar laudo em PDF**: o arquivo é lido no próprio aparelho; nada é enviado a servidor.
3. Confira os valores em **Conferir dados** (todos editáveis).
4. **Exportar PDF do paciente**: gera `Laudo_<Nome>_<data>.pdf` com 2 páginas A4.

Também dá para digitar os valores de qualquer balança à mão.

## Formatos reconhecidos

- **Avanutri (AVABIO-380, relatório "Relatório de Avaliações")**: identificação, faixas de
  normalidade do aparelho, massa magra e gordura segmentar, TMB, índice apendicular, idade
  metabólica, gordura visceral, impedâncias (5/50/250 kHz) e histórico.
  - A "Massa Livre de Gordura" da Avanutri é tratada como **massa magra** (água + proteína, sem
    minerais): ela soma com os segmentos e, com gordura + minerais, fecha o peso.
  - O PDF não traz a massa muscular esquelética do dia: ela é estimada pela proporção
    músculo/massa magra da última avaliação do histórico e marcada com `*`.

## Modelo

Peso = gordura + minerais + massa magra (água + proteína). Valores ausentes são estimados e marcados com `*`.
Laudo informativo; não substitui avaliação clínica.
