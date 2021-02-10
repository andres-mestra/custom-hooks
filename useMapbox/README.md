# useMapbox

Custom hook de integración de  React con MapBox.

<a href="https://mapbox.com" target="_blank">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/Mapbox_logo_2017.svg/1280px-Mapbox_logo_2017.svg.png" width="128" /></a>
</a>

Dependencias:
```
yarn add mapbox-gl uuid rxjs
```

Ejemplo:

```js
import * as React from 'react'
import { useMapbox } from '../hooks/useMapbox'


const puntoInicial = {
  lng: -122.4611,
  lat: 37.7986,
  zoom: 13.5,
}

export const MapaPage = () => {
  
  const { coords, setRef} = useMapbox(puntoInicial);

  return (
    <>
    <div className="infoCoords">
      Lng:  { coords.lng } | lat: { coords.lat } | zoom: { coords.zoom }
    </div>
      <div
        ref={ setRef }
        className="mapContainer"
      />
    </>
  )
}

```
