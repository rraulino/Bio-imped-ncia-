# Laudo Corporal

Transforma os números de qualquer balança/aparelho de bioimpedância num laudo completo,
no estilo dos relatórios clínicos de composição corporal:

- Análise da composição corporal (água, proteína, minerais, gordura, massa magra) com faixas normais
- Análise músculo-gordura em % do padrão para a altura
- Análise de obesidade (IMC e % de gordura)
- Pontuação estimada, perfil C/I/D, controle de peso, TMB, visceral, RCQ
- Análise segmentar (se o aparelho medir)
- Histórico com variações entre medições e backup em JSON

É um único `index.html`, sem servidor. Abra no navegador ou publique no GitHub Pages
(Settings → Pages → Branch). Os dados ficam só no navegador (localStorage).

Valores que o aparelho não fornece são estimados a partir da massa livre de gordura e marcados com `*`.
Laudo informativo; não substitui avaliação profissional.
