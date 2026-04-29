# Gabriel Keyboard

Um teclado mecânico customizável com iluminação RGB e controlador de firmware avançado.

## Características

- **101 Teclas** com diodos individuais para matrix scanning
- **16 LEDs RGBW** para iluminação customizável por tecla
- **Display LCD 16x2** para feedback visual (NHD-0216XZ)
- **Memória Flash 128 Mbit** (W25Q128JVSIQ) para armazenamento de configurações
- **Expansor I2C** (PCF8574ADWR) para gerenciamento de pinos
- **Conectividade USB** (USB4085-GF-A)
- **Regulador de tensão TLV75533** para alimentação estável
- **Firmware customizável** com suporte a macros e programação

## Estrutura do Projeto

```
GabrielKeyboard/
├── README.md                          # Este arquivo
├── GABRIELKEYBOARD.DSN               # Schematic (OrCAD)
├── GABRIELKEYBOARD.BOM               # Bill of Materials
├── gabrielkeyboard.pdf               # Diagrama do schematic
├── GabrielKeyboard.opj                # Projeto OrCAD
├── allegro/                            # Arquivos de PCB Layout (Allegro)
│   ├── gabrielkeyboard.brd            # Layout da PCB
│   └── ...
├── gabrielkeyboard_output/            # Arquivos de saída
│   ├── bom.sch.csv                   # BOM em CSV
│   └── variant.txt
├── GabrielKeyboard-PSpiceFiles/       # Simulações SPICE
└── signoise.run/                      # Análise de ruído

```

## Ferramentas Utilizadas

- **OrCAD Capture** - Design do schematic
- **OrCAD Presto** - Layout da PCB
- **Git** - Controle de versão

##  Como Visualizar

### Abrindo o Projeto

1. **Schematic**: Abra `GabrielKeyboard.opj` com OrCAD Capture
2. **PCB Layout**: Abra `allegro/gabrielkeyboard.brd` com Cadence Allegro ou OrCad Presto
3. **Schematic PDF**: Abra `GabrielKeyboard.pdf`

### Exportando Arquivos

- BOM em CSV: Utilize o arquivo em `gabrielkeyboard_output/bom.sch.csv`
- Arquivos de fabricação: Consulte os arquivos em `gabrielkeyboard_output/`

