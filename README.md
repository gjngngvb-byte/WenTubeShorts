# WenTube Shorts

Painel web inicial para acompanhar a futura fábrica de Shorts.

## Estado atual
- Interface responsiva de controle.
- Campo para inserir um link individual do YouTube.
- Fila local da sessão com título/link e fase atual.
- Visão das etapas planejadas do pipeline e configurações iniciais.

## Limitações desta preparação
Esta é apenas a camada visual (frontend). A fila é mantida em memória no navegador e desaparece ao recarregar a página. Ainda não existe worker de download, banco de dados, armazenamento de vídeos, autenticação, monitoramento real de canais ou integração de publicação com YouTube. Os números do painel são estados iniciais, não métricas reais.

## Executar localmente
Abra `index.html` no navegador. Não há dependências nem build.

## Próximas integrações
1. API/backend com fila persistente e estados reais.
2. Worker de processamento em ambiente compatível com arquivos grandes.
3. Armazenamento de mídia e logs.
4. Monitoramento de canais e detecção de novos vídeos, com processamento apenas de mídia que possa ser obtida legitimamente.
5. OAuth do YouTube e publicação automática após validação.
6. Autenticação do painel e proteção das credenciais.

Nunca coloque tokens, chaves OAuth ou segredos no frontend ou no repositório.
