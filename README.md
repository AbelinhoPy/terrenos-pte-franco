# Terrenos Pte. Franco — Mapa Cadastral e Comparativo

Aplicação web interativa para visualização cadastral, análise comparativa de terrenos e estudo de viabilidade imobiliária em Presidente Franco e região (rodada v11 / 2026).

## Recursos e Correções Implementadas
1. **Separação de Comparáveis e Descartados**: Preservação das categorias originais de glebas (1–5 ha e 5–20 ha) e filtro de status com descarte justificado por restrições ambientais (faixa de proteção do Rio Monday, Ley 4241/10, arroio e nascentes).
2. **Duplicatas Vinculadas**: 7 pares idênticos identificados e vinculados entre séries PF e B (PF-30/B-08, PF-31/B-10, PF-25/B-07, etc.), com contador segregando registros de propriedades únicas.
3. **Inconsistências Cadastrais**:
   - **PF-05**: Preservação do dado numérico (3.877 m²) e sinalização da discrepância documental com o título (3.887 m²).
   - **PF-25**: Reclassificado de Grupo A para Grupo A2 (> 8.000 m²) conforme critério dimensional (11.815 m²).
4. **Filtro de Preço Sem Limite Real**: Deslizador numérico sem teto artificial de 1.100 USD/m² e aplicação consistente a todos os imóveis (incluindo ofertas alvo).
5. **Sincronização de Seleção**: Limpeza automática do painel e marcadores quando o terreno selecionado deixa de estar visível pelos filtros.
6. **Transparência Avaliatória**: Substituição de rótulos sumários por etiquetas documentais ("Avaliação preliminar do relatório").
7. **Precisão Cartográfica**: Adoção do termo "pino informado no anúncio/Maps", distinguindo de levantamento cadastral oficial.
8. **Acessibilidade Completa**: Navegação total por teclado nos pontos SVG e tabela, atributos ARIA dinâmicos e respeito a `prefers-reduced-motion`.
9. **Estabilidade de Navegação**: Limites de zoom (clamping), botão de reset e prevenção de seleção acidental durante arrasto.
10. **Design Moderno e Responsivo**: Tema claro e escuro, cards de métricas em tempo real (KPIs) e layout intuitivo.
