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

## 3. Script da API

Incluir a API do Almav Mapas no seu arquivo HTML:
```javascript
<script src="https://urba.maps.almav.com/maps/api/js?key=<chave>&callback=<retorno>" async></script>
```
`utilize a chave:` **Ma63ae86-1c36-42d4-bcfc-a953ddbfb546**

> ---
> IMPORTANTE
> 1. Ao incluir o Mapa Interativo via **iFrame**, funções como o botão de GPS e tela cheia não irão funcionar. Utilize sempre a implementação por meio do código javascript.
> 2. Administração do Mapa Interativo: será necessário autorizar todos os domínios que receberão a integração, **informe a Almav** sobre os endereços. Por exemplo: https://www.urba.com.br/

Demonstração do Mapa Interativo: https://urba.almav.com.br/jardins-da-mantiqueira

![alt text](https://urba.maps.almav.com/maps/assets/Ma63ae86-1c36-42d4-bcfc-a953ddbfb546/thumb01.jpg)
