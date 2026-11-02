# 🔬 Kits Didáticos de Física

Projeto aberto para o desenvolvimento de **kits didáticos de física de baixo custo**, integrando eletrônica embarcada (ESP32/Arduino), fabricação digital (FreeCAD + impressão 3D), aquisição de dados e software educacional.

> **Objetivo:** criar experimentos de física acessíveis, reprodutíveis e de código/hardware aberto, para uso em sala de aula e como projeto de extensão/pesquisa.

[![License: MIT](https://img.shields.io/badge/Código-MIT-blue.svg)](LICENSE)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/Hardware%20%26%20Docs-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE-hardware-docs)

---

## 🎯 Motivação

Este repositório reúne o desenvolvimento de kits que cruzam quatro áreas:

- **Eletrônica embarcada** — sensores + ESP32/Arduino para aquisição de sinais físicos
- **Fabricação digital** — suportes, trilhos e gabaritos modelados em FreeCAD e impressos em 3D
- **Software** — firmware, tratamento de dados (Python), dashboards web e persistência (SQL)
- **Educação** — cada kit acompanha roteiro pedagógico, fundamentação e sugestões de uso em aula

---

## 📂 Estrutura do repositório

```
kits-didaticos-fisica/
├── README.md                 # este arquivo
├── LICENSE                   # MIT (código)
├── LICENSE-hardware-docs     # CC BY-SA 4.0 (hardware, modelos 3D, textos)
├── .gitignore
├── docs/                     # documentação geral do projeto
├── common/                   # código reutilizável entre kits
│   ├── python/               # bibliotecas Python compartilhadas (leitura serial, plot, etc.)
│   └── web/                  # componentes de dashboard reutilizáveis
└── kits/
    ├── _template/            # modelo para criar um novo kit (copie esta pasta)
    ├── 01-queda-livre/
    ├── 02-mhs-pendulo/
    └── ...
```

### Anatomia de cada kit (`kits/<nome>/`)

| Pasta | Conteúdo |
|-------|----------|
| `firmware/` | Código do ESP32/Arduino |
| `3d-models/` | Arquivos FreeCAD (`.FCStd`) e STLs para impressão |
| `electronics/` | Esquemas, lista de componentes (BOM), diagramas de ligação |
| `data/` | Dados de exemplo e scripts de análise |
| `media/` | Fotos, gifs e vídeos do experimento |
| `docs/` | Roteiro pedagógico, teoria, guia de montagem |

---

## 🧪 Kits

| # | Kit | Conceito de física | Sensor principal | Status |
|---|-----|--------------------|------------------|--------|
| 01 | Queda livre | Cinemática, cálculo de *g* | Barreira óptica IR | 🚧 Em desenvolvimento |
| 02 | MHS (pêndulo) | Oscilações, período | Ultrassônico HC-SR04 | 📋 Planejado |
| 03 | Termodinâmica | Curvas de aquecimento/resfriamento | DS18B20 | 📋 Planejado |

> Legenda: ✅ Concluído · 🚧 Em desenvolvimento · 📋 Planejado

---

## 🚀 Como usar

1. Escolha um kit em `kits/`.
2. Leia o `docs/` do kit (teoria + guia de montagem).
3. Imprima as peças de `3d-models/`.
4. Monte a eletrônica seguindo `electronics/`.
5. Grave o firmware de `firmware/` no ESP32/Arduino.
6. Rode os scripts de `data/` para coletar e visualizar os resultados.

---

## 🛠️ Tecnologias

`ESP32` · `Arduino` · `Python` · `FreeCAD` · `Impressão 3D (FDM)` · `LabVIEW` · `SQL` · `HTML5/JS`

---

## 📜 Licença

Este projeto usa **licenciamento duplo**, prática comum em projetos de hardware aberto:

- **Código-fonte** (firmware, scripts, web): [MIT](LICENSE)
- **Hardware, modelos 3D e documentação**: [CC BY-SA 4.0](LICENSE-hardware-docs)

Você é livre para usar, modificar e distribuir, inclusive em contexto educacional, mantendo a atribuição.

---

## 👤 Autor

**Renan Ritter** — Técnico Eletrônico | Tecnólogo em Automação Industrial | Licenciado em Física
Gravataí, RS · Brasil

> Projeto pessoal de longo prazo, com potencial de uso como projeto de extensão. <!-- e base para pesquisa de mestrado em Informática/Tecnologias Digitais na Educação. -->
