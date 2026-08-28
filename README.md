# dashboard-viabilidade_Movel
Dashboard interativo para estudo de viabilidade de cobertura móvel (4G/5G) a partir de dados de ERBs (estações rádio-base).

# 📡 Estudo de Viabilidade – Cobertura Móvel

Dashboard interativo para análise de cobertura de telecomunicações. Carregue uma planilha com dados de antenas (ERBs), pesquise por endereços ou coordenadas, e visualize em um mapa interativo quais operadoras e tecnologias estão disponíveis em um raio de até 20 km.

![Preview do Dashboard](https://via.placeholder.com/800x400?text=Dashboard+Preview) 
*(Substitua esta imagem por um print real do seu dashboard depois)*

## 🚀 Funcionalidades

- 📂 **Upload de planilhas Excel (.xlsx/.xls)** – Carregue sua base de antenas com colunas como Operadora, Latitude, Longitude, Tecnologias (Tecs), Faixa, etc.
- 🗺️ **Mapa interativo (Leaflet)** – Visualize todas as antenas e os pontos pesquisados.
- 🔍 **Busca por endereço ou coordenadas** – Use o Nominatim (OSM) para geocodificar ou insira coordenadas diretamente (ex: `-28.72917, -54.9075`).
- 📏 **Raio dinâmico** – Ajuste o raio de busca de 0,5 km a 20 km com um slider.
- 🎯 **Filtros avançados** – Filtre os resultados por **Operadora** (Tim, Vivo, Claro, Oi) e por **Tecnologia** (4G, 5G, 3G, etc.).
- 📊 **Indicadores em tempo real** – Veja a contagem total de antenas, operadoras disponíveis, tecnologias presentes e a distância da antena mais próxima.
- 📋 **Lista de pontos pesquisados** – Gerencie múltiplos endereços/coordenadas pesquisados e navegue entre eles.
- 📑 **Tabela detalhada** – Visualize todas as antenas no raio com distância, localização, infraestrutura e faixa de frequência.
- 💾 **Exportação CSV** – Exporte a viabilidade de todos os pontos pesquisados para um arquivo CSV compatível com Excel.
- 📂 **Importação de lista** – Faça upload de um arquivo .txt ou .csv com várias coordenadas/endereços para pesquisar em lote.

## 🛠️ Tecnologias utilizadas

- **[Leaflet.js](https://leafletjs.com/)** – Mapas interativos leves.
- **[SheetJS (xlsx)](https://sheetjs.com/)** – Leitura de arquivos Excel.
- **[Font Awesome](https://fontawesome.com/)** – Ícones visuais.
- **[Nominatim (OSM)](https://nominatim.org/)** – Geocodificação de endereços (aberto e gratuito).
- **HTML5 + CSS3 + JavaScript (Vanilla)** – Interface 100% client-side (não precisa de servidor).

## 📁 Estrutura esperada da planilha Excel

Ao fazer o upload, o sistema espera que a planilha tenha as seguintes colunas (os nomes devem ser exatamente esses, ou o sistema tentará encontrar os mais próximos):

| Coluna | Descrição |
|--------|-----------|
| `Número Estação` | Identificador da estação |
| `Operadora` | Nome da operadora (ex: TIM, VIVO, CLARO, OI) |
| `SiglaUF` | Estado (ex: SP, RJ, MG) |
| `Mun` | Município |
| `Bairro` | Bairro |
| `Logradouro` | Endereço da antena |
| `Latitude` | Coordenada latitude (ex: -23.5505) |
| `Longitude` | Coordenada longitude (ex: -46.6333) |
| `Ibge` | Código IBGE (opcional) |
| `ClassInfraFisica` | Tipo de infraestrutura (ex: Torre, Poste) |
| `Tecs` | Tecnologias suportadas separadas por espaço (ex: 4G 5G) |
| `Faixa` | Faixa de frequência (ex: 700 MHz, 2.5 GHz) |

## 🧑‍💻 Como usar (online)

1. Acesse o link do GitHub Pages (ou Netlify/Vercel) onde este projeto está hospedado.
2. Clique em **"Carregar Pasta1.xlsx"** e selecione sua planilha.
3. Digite um endereço (ex: `Av. Paulista, 1000, São Paulo`) ou coordenadas (ex: `-23.5505, -46.6333`) no campo de busca.
4. Ajuste o raio de busca (padrão 5 km).
5. Clique em **"Buscar"** para visualizar as antenas no mapa e na tabela.
6. Use os filtros de Operadora e Tecnologia para refinar os resultados.
7. Exporte os resultados em CSV clicando no botão **"CSV"** na tabela.
