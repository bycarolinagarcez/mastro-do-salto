# Mastro do Salto — Guia Digital de Hóspedes

Projeto independente baseado na estrutura do guia Casinha d’Aldeia, personalizado para a casa Mastro do Salto, em Tavira.

## Utilização

- `index.html`: guia digital para hóspedes (Português, English, Español, Français, Deutsch).
- `admin/index.html`: painel de administração para editar textos, horários, Wi-Fi, fotografias, locais, experiências e contactos.
- `content.json`: dados iniciais da casa.

Para testar localmente: `python3 -m http.server 8000` e abrir `http://localhost:8000/`.

## Antes de publicar

1. Inserir no painel os dados confirmados pela anfitriã: check-in, check-out, Wi-Fi, morada exata e contactos autorizados.
2. Substituir as fotografias remotas provenientes do anúncio Airbnb por ficheiros fornecidos pela proprietária, para garantir carregamento estável e direitos de utilização.
3. Rever recomendações e informações dos equipamentos.
4. Publicar num repositório e hosting separados da Equicampo. Configurar a publicação GitHub no admin para o novo repositório.

**Nota:** Não foram inventados dados privados ou instruções de acesso. Os horários no anúncio não estavam disponíveis na leitura pública.

## GitHub Pages

Criar repositório público `mastro-do-salto` na conta GitHub escolhida, carregar os ficheiros na raiz e ativar Settings > Pages > Deploy from a branch > main > /(root). O endereço do guia será https://UTILIZADOR.github.io/mastro-do-salto/ e o painel estará em /admin/. O admin deteta automaticamente o utilizador do GitHub Pages e publica apenas no repositório `mastro-do-salto`. Criar um fine-grained personal access token com permissão Contents: Read and write apenas neste repositório.
