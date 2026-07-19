# Kit XX — [Nome do Kit]

> Modelo de kit. **Copie esta pasta `_template/`** e renomeie para criar um novo kit (ex.: `01-queda-livre`).

## 📌 Resumo

| Item | Descrição |
|------|-----------|
| **Conceito de física** | (ex.: cinemática, cálculo de *g*) |
| **Nível** | (ex.: ensino médio / superior) |
| **Sensor principal** | (ex.: barreira óptica IR) |
| **Microcontrolador** | ESP32 / Arduino |
| **Grandeza medida** | (ex.: tempo, distância, temperatura) |
| **Status** | 📋 Planejado |

---

## 🎓 Fundamentação teórica

Breve descrição do fenômeno físico e das equações envolvidas.
(Ver detalhes em `docs/teoria.md`.)

## 🧰 Lista de materiais (BOM)

| Componente | Qtd | Observação |
|------------|-----|------------|
| ESP32 DevKit | 1 | |
| Sensor ... | | |
| ... | | |

Detalhes em `electronics/BOM.md`.

## 🔌 Montagem eletrônica

Diagrama de ligação em `electronics/`. Resumo dos pinos:

| Sinal | Pino ESP32 |
|-------|-----------|
| ... | ... |

## 🖨️ Peças 3D

Arquivos em `3d-models/`. Imprimir em PLA/PETG. Parâmetros sugeridos:
- Altura de camada: 0.2 mm
- Preenchimento: 20%

## 💻 Firmware

Código em `firmware/`. Como compilar/gravar:
```
# instruções (Arduino IDE / PlatformIO)
```

## 📊 Coleta e análise de dados

Scripts em `data/`. Exemplo de uso:
```
python data/analise.py
```

## 🧪 Roteiro pedagógico

Passo a passo para uso em aula em `docs/roteiro.md`.

## 📷 Mídia

Fotos e vídeos em `media/`.
