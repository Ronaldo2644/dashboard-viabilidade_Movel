
# 📡 DASHBOARD - Estudo de Viabilidade – Cobertura Móvel  (2G/3G/4G/5G)

Dashboard interativo para análise de cobertura de telecomunicações. Carregue uma planilha com dados de antenas (ERBs), pesquise por endereços ou coordenadas, e visualize em um mapa interativo quais operadoras e tecnologias estão disponíveis em um raio de até 20 km.

<img width="1911" height="901" alt="image" src="https://github.com/user-attachments/assets/d81712da-79ba-48c3-a3eb-4072feb5fad1" />


## 🚀 Funcionalidades

- 📂 **Upload de planilhas Excel (.xlsx/.xls)** – Carregue sua base de antenas com colunas como Operadora, Latitude, Longitude, Tecnologias (Tecs), Faixa, etc.
- 🗺️ **Mapa interativo (Leaflet)** – Visualize todas as antenas e os pontos pesquisados.
- 🔍 **Busca por endereço ou coordenadas** – Usa o Nominatim (OSM) para geocodificar ou inserindo as coordenadas diretamente (ex: `-28.72917, -54.9075`) ou (nome de referencia; -28.72917, -54.9075) que é "o melhor cenário para identificar o ponto".
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

[![Baixar ERBs](https://img.shields.io/badge/📥_Baixar_ERBs-0066b3?style=for-the-badge&logo=download&logoColor=white)](https://www.telecocare.com.br/mapaerbs/index.php)


## 🧑‍💻 Como usar (online)

[![Acessar Dashboard](https://img.shields.io/badge/▶️_Acessar_Dashboard-1b4a7a?style=for-the-badge&logo=githubpages&logoColor=white)](https://ronaldo2644.github.io/dashboard-viabilidade_Movel/)

1. Acesse o link .
2. Clique em **"Carregar ERBs.xlsx"** e selecione sua planilha.
3. Digite um endereço (ex: `Av. Paulista, 1000, São Paulo`) ou coordenadas (ex: `-23.5505, -46.6333`) no campo de busca.
4. Ajuste o raio de busca (padrão 5 km).
5. Clique em **"Buscar"** para visualizar as antenas no mapa e na tabela.
6. Use os filtros de Operadora e Tecnologia para refinar os resultados.
7. Exporte os resultados em CSV clicando no botão **"CSV"** na tabela.

## ☕ Apoie o projeto
Se este dashboard ajudou você em seus estudos ou trabalho, considere contribuir com um café ☕!  
Sua doação incentiva novas funcionalidades, correções e manutenção do projeto ou novas ideias.

Como contribuir
 - PIX: `QRCODE ABAIXO`
 - PayPal: https://www.paypal.com/donate/?hosted_button_id=UK57366LPFBS8
 - QR Code – aponte a câmera do seu celular para o código abaixo e faça sua doação via PIX:

<img src="https://github.com/Ronaldo2644/dashboard-viabilidade_Movel/raw/main/QRCODE.jpeg" alt="QR Code PIX" width="200" height="200" />

