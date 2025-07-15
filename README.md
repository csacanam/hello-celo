# hello-celo

Este proyecto aplica todo lo aprendido en el **DeFi Builder Bootcamp** organizado por **Celo Colombia**.

Aquí encontrarás contratos inteligentes desarrollados con [Foundry](https://book.getfoundry.sh/) y Solidity, así como scripts y pruebas para desplegar y verificar los contratos en la red de Celo.

## Estructura del proyecto

- `src/`: Contratos inteligentes en Solidity
- `script/`: Scripts de despliegue y automatización
- `test/`: Pruebas automatizadas
- `broadcast/`: Logs de despliegue

## Requisitos

- [Foundry](https://book.getfoundry.sh/getting-started/installation)
- Node.js (opcional, para scripts adicionales)

## Configuración

1. Copia el archivo `.env.example` a `.env` y agrega tus variables de entorno:
   ```sh
   cp .env.example .env
   ```
2. Llena los valores necesarios en `.env` (por ejemplo, `RPC_URL`, `PRIVATE_KEY`, etc).

## Comandos útiles

### Compilar contratos

```sh
forge build
```

### Ejecutar pruebas

```sh
forge test
```

### Formatear código

```sh
forge fmt
```

### Tomar snapshot de gas

```sh
forge snapshot
```

### Levantar nodo local (Anvil)

```sh
anvil
```

### Desplegar contratos

```sh
forge script script/Deploy.s.sol --rpc-url $RPC_URL --private-key $PRIVATE_KEY --broadcast
```

### Usar Cast (herramienta CLI de Foundry)

```sh
cast <subcomando>
```

### Ayuda de comandos

```sh
forge --help
anvil --help
cast --help
```

---

¡Este repositorio es parte del aprendizaje y la comunidad de Celo Colombia! 🚀
