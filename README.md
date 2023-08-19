# urba.almav.com.br-jardins-da-mantiqueira
Quick Start Mapa Interativo

## 1. Definir o elemento destino

EXEMPLO ELEMENTO DESTINO

```html
<div id="map"></div>
```

## 2. Script inicial

EXEMPLO FUNÇÃO RETORNO
```javscript
let map;
function initMap() {
  map = new almav.maps.Map(document.getElementById("map"), {
      "settings-id": 1,
  });
}
```
O código utiliza a função document.getElementById("map") para obter um elemento HTML com o ID "map". Esse elemento é uma div vazia onde o mapa será exibido. Além disso, é fornecida ao objeto Map uma propriedade "settings-id" com o valor 1, que é o valor padrão de configuração do mapa.

## 3. Script da API

Incluir API do almav Mapas no seu arquivo HTML:
```javascript
<script src="https://urba.maps.almav.com/maps/api/js?key=<chave>&callback=<retorno>" async></script>
```
`<chave>:` **Ma63ae86-1c36-42d4-bcfc-a953ddbfb546**
`<retorno>:` Quando você inclui o parâmetro obtigatório callback na URL do script, como no exemplo fornecido, o valor do parâmetro deve ser o nome de uma função que será chamada pelo script do almav Mapas API. Nesse caso, a função de callback é chamada initMap.

> ---
> IMPORTANTE
> 1. Ao incluir o Mapa Interativo via **iFrame**, funções como o botão de GPS e tela cheia não irão funcionar. Utilize sempre a implementação por meio do código javascript.
> 2. Administração do Mapa Interativo: será necessário autorizar todos os domínios que receberão a integração, **informe a Almav** sobre os endereços. Por exemplo: https://www.urba.com.br/

Demonstração do Mapa Interativo: https://urba.almav.com.br/jardins-da-mantiqueira

![alt text](https://maps.almav.com/maps/assets/Ma63ae86-1c36-42d4-bcfc-a953ddbfb546/thumb01.jpg)
