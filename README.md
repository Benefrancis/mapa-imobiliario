# Analisando Ofertas de Imóveis por Unidade da Federação Brasileira



# Tecnologias Utilizadas no projeto

[GeoPandas](https://geopandas.org/en/stable/)
Utilizamos o Vamos utilizar o [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb) para construir o projeto. Para que você consiga usá-lo, é necessário ter uma conta Gmail, pois todo notebook ficará armazenado no Google Drive.
[Dados e  imagens aéreas e orbitais, mapas, malhas](https://www.ibge.gov.br/geociencias/downloads-geociencias.html?caminho=organizacao_do_territorio/malhas_territoriais/malhas_de_setores_censitarios__divisoes_intramunicipais/2021/Malha_de_setores_%28shp%29_por_UFs), além de conteúdos da INDE, atlas e arquivos Google Earth, entre outros (todos os arquivos utilizados são públicos).

 
# Camadas do Mapa

A biblioteca Folium permite a criação da visualização de mapas a partir de camadas. A primeira delas é a camada de fundo de mapa, que é composta por elementos essenciais em uma visualização cartográfica porque fornece o contexto geográfico para entender e analisar os dados que serão apresentados no mapa.

Por padrão, são disponibilizadas diversas camadas, que podem ser encontradas diretamente na [documentação da biblioteca](https://python-visualization.github.io/folium/modules.html#folium.folium.Map), na descrição do método Map():

OpenStreetMap
Mapbox Bright (Com níveis de zoom limitados)
CartoDB Positron
CartoDB Dark Matter
Além dos tipos de visualização padrão, podemos explorar [camadas personalizadas da Leaflet](http://leaflet-extras.github.io/leaflet-providers/preview/), que é uma biblioteca JavaScript usada para criar mapas interativos na internet e serve como base de construção do Folium.

Camadas de base podem ser criadas com o método [folium.TileLayer()](https://python-visualization.github.io/folium/modules.html#folium.raster_layers.TileLayer) e adicionadas na visualização usando a função add_to(). Além disso, é possível alternar entre as visualizações de camadas de forma interativa, bastando criar um controle de camadas usando o método [folium.LayerControl()](https://python-visualization.github.io/folium/modules.html#folium.map.LayerControl).