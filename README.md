# Estados y Municipios de México

_Un paquete de php y javascript de los estados y municipios de mexico, soporta el comando mexico:publish para laravel_


### Install 🔧

```bash
    composer require mmo-and-friends/estados-municipios-mexico
```

### Quick Sample Php

```php
    use MmoAndFriends\Mexico\Mexico;
    use MmoAndFriends\Mexico\MexicoTrait;

    class Dummy {
        $estados = Mexico::estados();
        $municipios = Mexico::municipiosDeEstado($estados[0]->id)
    }

    class DummyTrait {
        use MexicoTrait;

        $estados = $this->estados()
        $municipios = $this->municipiosDeEstado($estados[0]->id)
    }
```

### Quick Sample Html

```html
    <div>
        <select id="select-estados-id">
        </select>
    </div>
    <div>
        <select id="select-municipios-id">
        </select>
    </div>

    <script src="./estados_municipios_mexico.js"></script>
    <script>
        /**
         * Cargar los selects con la informacion
         * @param {String|Element} selectEstados
         * @param {String|Element} selectMunicipios 
         * @param {Integer} estadoSeleccionado
         * @param {Integer} municipioSeleccionado
         */
        EstadosMunicipiosMexico.mountIn('#select-estados-id','#select-municipios-id')
    </script>

```
## Author ✒️

_Guillermo Rodriguez / guillermo.rod.dev@gmail.com_

## License 📄

This project is under the license (MIT) - Look the file [LICENSE.md](LICENSE.md).