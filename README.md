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

## Author ✒️

_Guillermo Rodriguez / guillermo.rod.dev@gmail.com_

## License 📄

This project is under the license (MIT) - Look the file [LICENSE.md](LICENSE.md).