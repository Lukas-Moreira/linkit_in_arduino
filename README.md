# LinkIt Smart 7688 Duo - Arduino Integration

Este repositório contém:

- 📦 Arquivos de configuração para uso do **LinkIt 7688 Duo** com Arduino IDE
<!-- - 🌡 Backend em **FastAPI** para coleta de dados de temperatura e umidade via serial
- 📊 Dashboard web com indicadores visuais em tempo real
- 🗃 Script SQL para criação do banco de dados MySQL -->

---

## 📁 Estrutura

### `arduino_package/`
Contém o `package_mtk_linkit_smart_7688_index.json`, necessário para incluir o LinkIt Duo na Arduino IDE via URL personalizada.

<!-- ### `fastapi_backend/`
- `fastapi.py`: API para inserção e leitura dos dados de temperatura e umidade.
- `linkit7688.py`: Leitura serial dos dados e envio para a API.
- `tempdata.sql`: Criação da tabela no banco de dados MySQL. -->

### `web_dashboard/`
Interface web com `gauge.html` e `gauge.js` para visualização dos dados em tempo real.

---

## Como usar?

### Arduino IDE

1. Vá em **Preferências** e adicione a URL:

```bash 
    https://raw.githubusercontent.com/Lukas-Moreira/linkit_in_arduino/main/arduino_package/package_mtk_linkit_smart_7688_index.json
```

2. Abra o **Gerenciador de Placas** e instale o pacote "LinkIt Smart 7688 Duo".

3. Ainda no **Gerenciador de Placas** instale o pacote "Arduino AVR Boards"