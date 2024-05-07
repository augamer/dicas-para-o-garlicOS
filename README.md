# Dicas para o GarlicOS (Para Windows)

## Livro de receitas do GarlicOS

*Siga estas instruções para uma maneira fácil de deixar rodando rapidamente! Estas são instruções completas e serão a maneira mais fácil de começar a usar um novo **RG35XX 2023**.*

## Prepare um Cartão Micro SD

Obtenha um cartão SD de alta qualidade (por exemplo, SanDisk Extreme), *32 GB ou maior*, recomenda-se 64 GB para cima. Não economize aqui, eles são baratos e não use o cartão que acompanha o RG35XX porque é uma porcaria.

### Instale Aplicativos Auxiliares

Baixe e Instale [Disk Genius](https://www.diskgenius.com/download.php)

Baixe e Instale [Rufus](https://rufus.ie/en/).

Baixe e Instale [7-zip](https://www.7-zip.org/download.html).

### Coloque GarlicOS no Cartão Micro SD

Baixe os arquivos "RG35XX-MicroSDCardImage.7z.001" e "RG35XX-MicroSDCardImage.7z.002" do site [GarlicOS](https://www.patreon.com/posts/garlicos-for-76561333).

Abra "RG35XX-MicroSDCardImage.7z.001" no 7-zip e extraia para uma pasta no seu pc, por exemplo Downloads.  Dentro da pasta terá "garlic.img" e "README.txt"
Abra o **Rufus**.

Certifique-se de que o Cartão Micro SD correto esteja selecionado.

Clique "SELECT" e abra "garlic.img" na pasta que você extraiu.

Clique "START" para escrever a imagem no Cartão Micro SD.

### Nomeie e estenda as partições do Cartão Micro SD do GarlicOS

**Note**: Esta etapa só é necessária se você quiser usar um único Cartão Micro SD.

Abra **Disk Genius**.

Selecione seu cartão Micro SD no canto esquerdo

Estenda a partição FAT32 de 3.2GB do Cartão Micro SD assim:
* Clique com o botão direito na partição FAT32, escolha "Set Volume Name (V)" e nomeie-a como "ROMS". Isso tornará mais fácil encontrar esta partição no explorador de arquivos.
* Clique com o botão direito na mesma partição, escolha "Extend Partition (Ctrl_F12)" e clique em "Start" e depois em "Yes" duas vezes. Clique em “Complete” quando terminar.
* Observe a letra da unidade da partição “ROMS”. Se não houver letra de unidade, clique com o botão direito na mesma partição, escolha "Assign New Drive Letter (G)" e clique em "OK".

Renomeie a "Partição CFW":

* Clique com o botão direito na partição FAT16 de 10,0 MB, escolha "Set Volume Name (V)" e nomeie-a como "CFW".

Feche Disk Genius.

## Instalar ROMS

### Para baixar ROMS recomendo o [vimm.net](https://vimm.net/vault)
e para colocar as ROMS no Cartão Micro SD: 

Abra no Explorador de Arquivos a partição ROMS, abra a pasta ROMS e coloque cada ROM de cada console em sua respectiva pasta (por exemplo, ROMS de Super nintendo na pasta "SFC", ROMS de Gameboy Advance na pasta "GBA" e assim por diante)

### Para baixar BIOS recomendo esse Archive no archive.org: [Retroarch_System](https://archive.org/download/RetroarchSystemFiles/Retroarch-System/)

SEGA CD:
bios_CD_E.bin,
bios_CD_J.bin,
bios_CD_U.bin,

FAMICOM DISK SYSTEM:
disksys.rom

GAME BOY (para a logo no boot):
gb_bios.bin

GAME BOY COLOR (para a logo no boot):
gbc_bios.bin

GAME BOY ADVANCE:
gba_bios.bin

NEO GEO:
neogeo.zip (**Colocado na pasta de ROMS do Neo Geo**)

PLAYSTATION:
scph5501.bin

TURBOGRAFX-CD:
syscard1.pce,
syscard2.pce,
syscard3.pce,

e para colocar as BIOS no Cartão Micro SD:

Abra no Explorador de Arquivos a partição ROMS, abra a pasta BIOS e coloque as bios de cada console ali

## Extraia "Retro System Icons" (opcional)

Um pack de icones para cada videogame na seleção de jogos com um estilo retro
Baixe [Retro System Icons](https://github.com/Vidnez/retro-systems-icons-for-GarlicOS/releases), e dentro do ZIP copie a pasta "/retro_system_icons/system" para "/CFW/skin" na partição "ROMS".

## Extraia "Updated Retroarch Cores" (opcional)

Cores Atualizados para o Retroarch
Baixe [Updated Retroarch Cores](https://www.reddit.com/r/RG35XX/comments/16kwr0k/fyi_im_still_keeping_retroarch_cores_updated_for) e extraia para "/CFW/retroarch" na partição "ROMS".

## Use o Cartão Micro SD

Agora ejete o Cartão Micro SD com segurança e coloque-o na entrada TF1 do seu RG35XX!

### E esta tudo pronto para usar e aproveitar!
a partir daqui sera mais dicas para o futuro

## Atualizando o GarlicOS

Baixe [RG35XX-CopyPasteOnTopOfStock.7z.001 e RG35XX-CopyPasteOnTopOfStock.7z.002](https://www.patreon.com/posts/garlicos-for-76561333)

Abra o arquivo .7z.001 em 7-zip e extraia para a raiz do cartão SD.
Ejete o Cartão Micro SD e coloque na entrada TF1, agora é so ligar e esperar

## Configurações de vídeo do RetroArch

Isso faz com que os jogos Gameboy, Color e Advance tenham uma aparência muito melhor e melhore o desempenho. Não sei por que isso não é um padrão.

Abra a opção RetroArch no menu principal do GarlicOS.

* Settings > Video
  * [X] Threaded Video
* Settings > Video > Scaling
  * [X] Keep Aspect Ratio
selecione "Quit RetroArch" e pronto

## Overlays

Para ativar uma overlay para um sistema (FC, GB, GBA, GBC, SFC), durante um jogo:

*Nota: Primeiro segure MENU por um segundo e, em seguida, enquanto segura MENU, pressione X.*

* Menu + X para abrir o Quick Menu
* "B" para voltar pro menu principal do RetroArch
* Settings > On-Screen Display > On-Screen Overlay > Overlay Preset
* Escolha o preset de overlay correto para o sistema que você esta jogando.
* clique "B" 3x para voltar para o menu principal do Retroarch.
* Quick Menu > Overrides
* Save Core Overrides

## Ative o Estilo Gameboy

*Nota: Primeiro segure MENU por um segundo e, em seguida, enquanto segura MENU, pressione X.*

* Abra um jogo de GameBoy
* Menu + X para abrir o Quick Menu
* "Core Options"
  * GB Colorization: Auto
  * Internal Palette: GB - DMG
  * Interface Blending: Simple
* "B" para voltar.
* "Resume" (a configuração será salva automaticamente)

## Começar novo jogo

Por padrão, um jogo continua a partir do save state, o que é muito legal, mas se você quiser iniciar um jogo desde o início, inicie-o pressionando o botão START em vez de pressionar o botão “A”.

## Jogos Multi-disco

Para trocar discos em jogos Multi-disco:

*Nota: Primeiro segure MENU por um segundo e, em seguida, enquanto segura MENU, pressione X.*

* Menu + X para abrir o Quick Menu
* Disc Control > Eject Disc
* Change the Disc Index
* Insert Disc

## Atalhos

**no menu principal:**

| Button | Action |
|-|-|
POWER|Suspender
MENU + POWER|Desligar
A|Confirmar
B|Voltar
Select|Mudar velocidade da cpu
Start|Alterar o horario do relogio (no menu principal)
MENU + Vol +| brilho +
MENU + Vol -| brilho -

**No menu do jogo:**

| Button | Action |
|-|-|
Y|Salvar/Remover favorito
A| Abrir Jogo
Start|Abrir jogo sem continuar do save state

**Durante o jogo:**

*Nota: Primeiro segure MENU por um segundo e, em seguida, enquanto segura MENU, pressione X.*

| Button | Action |
|-|-|
MENU|Voltar para o GarlicOS
L1 + L2|Menu do MAME (apenas "Arcade")
MENU + X|Menu do Retroarch
MENU + UP|Screenshot
MENU + DOWN|Mutar audio
MENU + LEFT/RIGHT|Mudar o slot do save state
MENU + L1|Fast forward toggle
MENU + R1|Slow motion toggle
MENU + START|Pause
MENU + SELECT|Exibição de FPS

## Adaptador HDMI

A porta HDMI no rg35xx é uma porta Mini HDMI. Para usar o HDMI, obtenha um “cabo Mini HDMI macho para HDMI fêmea” e conecte uma extremidade ao 35xx e a outra extremidade a um cabo HDMI padrão.

## Colocar Videos (é bem mais complicado do que tudo aqui, nao é recomendado)

GarlicOS pode reproduzir arquivos de vídeo! Para converter vídeos para torná-los adequados para RG35XX:

Instale [ffmpeg](https://ffmpeg.org/download.html).

No terminal/cmd, use o seguinte comando (certifique-se de que a extensão de saída seja mkv):

```PowerShell
ffmpeg.exe -i [INPUT_FILENAME] -vf scale=640:-2  -vcodec libx264 -pix_fmt yuv420p -profile:v main -level 3.1 -preset medium -crf 23 -x264-params ref=4 -acodec libvorbis -movflags +faststart -hide_banner -loglevel error -stats [OUTPUT_FILENAME].mkv
```

copie o arquivo de vídeo para a pasta /Roms/VIDEOS na partição "ROMS".

`-vf scale=640:-2` mantém a proporção, largura de 640 e garante que o tamanho da largura e da altura seja múltiplo de 2.

Tem um player de video atualizado, [MPlayer](https://www.rg35xx.com/en/apps/apps-for-garlicos/) que tambem pode ser instalado.  siga as instruções no arquivo "readme.txt" no zip para instruções da instalação (esta em ingles).

## Pungent Best Set

*If you want to get up and running with a curated set of ROMS with only a 16GB SD card, try this.*

Insira o Cartão Micro SD no computador.

Abra a partição ROMS no Explorador de Arquivos.

Baixe [Pungent Best Set](https://archive.org/details/pungent-best-set_202304).

Extraia para a raiz da unidade “ROMS”.

Agora ejete o Cartão Micro SD com segurança e coloque-o na entrada TF1 do seu RG35XX e pronto

### Problema no Pungent Best Set

post de Gunseikan on Reddit:

* Baixei este pack e adicionei-o ao Garlic OS 1.4.9 no RG35XX. Por alguma razão, certas roms do NES estão lentas. Super Mario Bros. parece bom, mas Castlevania e Mega Man estão mais lentos, tanto na jogabilidade quanto no áudio. Testei isso para o núcleo FCEUmm e Nestopia: mesmo resultado. Overclocking Triend em retroarch: mesmo resultado. Tentei aumentar a velocidade do clock no rg35xx: mesmo resultado. Usando o sistema operacional padrão e roms, a coisa veio com os jogos rodando conforme planejado. As roms dos EUA rodaram em velocidade normal sem qualquer ajuste.*

Então se você usar o Pungent Best Set, observe que você pode querer substituir as roms do NES pelas versões dos EUA.

## Mapeamento de pasta ROMS

|Nome da Pasta|Sistema|
|-----------|------|
|AMIGA|Amiga (Commodore, 1985)|
|AMIGACD|Amiga CD 32 (Commodore, 1993)|
|APPS|Various|
|ARCADE|Arcade ([Mame 2003](https://archive.org/details/MAME_2003-Plus_Reference_Set_2018))|
|ATARI|Atari 2600 (Atari, 1977)|
|ATARIST|Atari ST (Atari, 1985)|
|C128|Commodore 128|
|COLECO|ColecoVision (Coleco, 1982)|
|COMMODORE|Commodore 64|
|CPC|Amstrad CPC (Amstrad, 1984)|
|CPS1|Capcom Play System 1 (Capcom, 1988)|
|CPS2|Capcom Play System 2 (Capcom, 1993)|
|CPS3|Capcom Play System 3 (Capcom, 1996)|
|DOOM|Doom (id, 1993)|
|DOS|MS-DOS (DOSBOX)|
|EIGHTHUNDRED|Atari 8bit (Atari, 1980)|
|FAIRCHILD|Fairchild Channel F (Fairchild, 1976)|
|FBA2012|Final Burn Alpha|
|FBNEO|Final Burn Neo|
|FC|Nintendo Entertainment System / NES (Nintendo, 1985)|
|FDS|Famicom Disk System (Nintendo, 1986)|
|FIFTYTWOHUNDRED|Atari 5200 (Atari, 1982)|
|GB|Nintendo Game Boy (Nintendo, 1989)|
|GBA|Nintendo Game Boy Advance (Nintendo, 2001)|
|GBC|Nintendo Game Boy Color (Nintendo, 1998)|
|GG|Sega Game Gear (Sega, 1991)|
|GW|Game & Watch (Nintendo, 1980)|
|INTELLIVISION|Mattel Intellivision (Mattel, 1979)|
|JAGUAR|Atari Jaguar (Atari, 1993)|
|LYNX|Atari Lynx (Atari, 1989)|
|MAME2000|MAME 2000|
|MD|Sega Genesis / MegaDrive (Sega, 1988)|
|MEGADUCK|Mega Duck (Welback, 1993)|
|MS|Sega Master System (Sega, 1986)|
|MSX|MSX - MSX2 (Microsoft, 1983)|
|NEOCD|SNK NeoGeo CD (SNK, 1994)|
|NEOGEO|SNK NeoGeo (SNK, 1990)|
|NGP|SNK NeoGeo Pocket & Color (SNK, 1999)|
|ODYSSEY|Magnavox Odyssey 2|
|PANASONIC|3DO (Panasonic, 1993)|
|PCE|NEC TurboGrafx-16 / PC-Engine(NEC/Hudson, 1989)|
|PCECD|NEC TurboGrafx CD / PC-Engine CDROM2 (NEC/Hudson, 1989)|
|PCFX|PCFX (NEC/Hudson, 1994)|
|PCNINETYEIGHT|NEC PC-98 (NEC, 1982)|
|PET|Commodore PET (Commodore, 1977)|
|PICO|PICO-8|
|POKE|Nintendo Pokemon mini (Nintendo, 2001)|
|PORTS|Ports collection|
|PS|Sony Playstation (Somy, 1995)|
|QUAKE|Quake (id, 1996)|
|SATELLAVIEW|Super Famicom Satellaview (Nintendo, 1995)|
|SCUMMVM|ScummVM|
|SEGACD|Sega CD / Mega-CD (Sega, 1991)|
|SEGASGONE|Sega SG-1000 (Sega, 1983)|
|SEVENTYEIGHTHUNDRED|Atari 7800 (Atari, 1986)|
|SFC|Super Nintendo / Super Famicom (Nintendo, 1991)|
|SGB|Super Game Boy (Nintendo, 1994)|
|SGFX|NEC SuperGrafx (NEC/Hudson, 1989)|
|SUFAMI|Bandai Sufami Turbo (Bandai, 1996)|
|SUPERVISION|Watara Supervision (Watara, 1992)|
|THIRTYTWOX|Sega 32X (Sega, 1994)|
|TIC|TIC-80 Tiny Computer (Various)|
|VB|Nintendo Virtual Boy (Nintendo, 1995)|
|VECTREX|GCE Vectrex (GCE, 1982)|
|VIC20|VIC-20 (Commodore, 1981)|
|VIDEOPAC|Odyssey2 VideoPac (Magnavox, 1978)|
|VIDEOS|Video Player|
|VMU|Dreamcast VMU (Sega, 1998)|
|WS|Bandai WonderSwan & Color (Bandai, 2000)|
|X68000|Sharp X68000 (Sharp, 1987)|
|ZXEIGHTYONE|Sinclair ZX81 (Sinclair, 1981)|
|ZXS|Sinclair ZX Spectrum (Sinclair, 1982)|

GarlicOS tambem suporta esse cores libreto:

|Nome da Pasta|Sistema|
|-----------|------|
|C128|Commodore 8-bit - [vice_x128](https://docs.libretro.com/library/vice/)|
|GPSP|Nintendo Game Boy Advance - [gpsp](https://docs.libretro.com/library/gpsp/)|
|NESTOPIA|NES/Famicom - [nestopia](https://docs.libretro.com/library/nestopia_ue/)|
|PCEIGHTYEIGHT|NEC PC-8000 / PC-8800 - [quasi88](https://docs.libretro.com/library/quasi88/)|
|PLUS4|Commodore Plus-4 [vice_xplus4](https://docs.libretro.com/library/vice/)|
|UZEBOX|Uzebox - [uzem](https://docs.libretro.com/library/uzem/)|
|XONE|Sharp X1 - [x1](https://github.com/libretro/xmil-libretro)|

Os seguintes núcleos não parecem ser suportados no GarlicOS:

|Nome da Pasta|Sistema|
|-----------|------|
|C64|Commodore 64 (Commodore, 1982)|
|CANNONBALL|Enhanced OutRun Engine|
|CAVESTORY|Cave Story (Pixel, 2004)|
|DAPHNE|LaserDisc Game Emulator|
|DUKE|Duke Nukem 3D (3D Realms, 1996)|
|GX4000|GX4000 (Amstrad, 1990)|
|MGBA|MGBA Emulator (Nintendo, 2001)|
|MSU1|Super Nintendo CD (Nintendo/Sony (1992)|
|OPENBOR|OpenBOR (2006)|
|PDF|PDF Reader|
|SM64|Super Mario 64 (Nintendo, 1996)|
|WOLF|Wofenstein 3D (id, 1992)|

`/CFW/config/coremapping.json` contém um mapeamento JSON da pasta ROM para o núcleo usado, por exemplo.

```JSON
"ARCADE": "km_mame2003_xtreme_libretro.so",
```

esses cores estão em `/CFW/retroarch/.retroarch/cores`.

## Instalar um novo Tema

Observe que o suporte a temas é bastante inconsistente entre as versões. Por enquanto, sugiro que você não instale um tema personalizado.

## Criar Imagens Personalizadas

Baixe [Skraper](https://www.skraper.net/)

Clique "Wizard", clique "YES"

* Enter Screenscraper Account info, clique "Validate", clique "NEXT"
* Front-End Selection: GENERIC EMULATION, clique "NEXT"
* Choose root of ROM path (e.g. /Roms on SD card), clique "NEXT"

Clique "FINISH"

Adicionar sistemas faltando (devido a diferenças de nomes de pastas)

* Clique "+"
* Desmarque "Show Categories"
* Em "Console" select:
  * ATARI 2600
  * ATARI 5200
  * ATARI 7800
  * GENESIS
  * MASTER SYSTEM
  * NES
  * PC-ENGINE CD-ROM
  * PLAYSTATION
  * SEGA 32X
  * SUPER NINTENDO
  * TURBOGRAFX-16
  * VIRTUAL BOY
  * WATARA SUPERVISION
  * WONDERSWAN
* Clique "OK"

Aba de Jogos & Front-End (Games & Front-End):

Modifique a pasta Games/Roms para cada um desses sistemas (clique em cada um de cada vez no painel esquerdo):

por exemplo. "F:\Roms\NEC PC Engine CD-Rom" para "F:\Roms\PCECD"

* ATARI 2600 : ATARI
* ATARI 5200 : FIFTYTWOHUNDRED
* ATARI 7800 : SEVENTYEIGHTHUNDRED
* GENESIS : MD
* MASTER SYSTEM : MS
* NEC PC ENGINE : PCE
* NEC PC-ENGINE CD-ROM : PCECD
* NES : FC
* PLAYSTATION : PS
* SEGA 32X : THIRTYTWOX
* SUPER NINTENDO : SFC
* VIRTUAL BOY : VB
* WATARA SUPERVISION : SUPERVISION
* WONDERSWAN : WS

Clique em "ALL SYSTEMS" (painel esquerdo)

Aba de Media:

Observe que 320x240 é usado aqui, apesar da resolução nativa ser 640x480. Isso é feito para criar arquivos de imagem menores que carregam mais rápido.

* Clique em "MANUAL" e Clique "-" (Remover)
* Clique em "IMAGES MIX"
  * Output folder: `%ROMROOTFOLDER%\media\images` -> `%ROMROOTFOLDER%\Imgs`
* em right box, clique ">" até "INTERNAL MIX" > "2 IMAGES MIX" aparecer.
* [X] Cleanup output folder before generating new medias
* [X] Resize width to: 320
* [X] Resize height to: 240
* [X] "Keep Image Ratio"

Clique play button no canto inferior direito, clique "OK"

Quando completo, você pode deletar os arquivos *.dat que estão em cada pasta de ROM.

Além disso, cada pasta ROM terá um arquivo *.Missing.Serial.txt - este arquivo contém ROMS que não eram conhecidos pelo skraper.

## Informações Técnicas

### Logo de boot

Na partição "CFW" (não na partição "ROMS") `boot_logo.bmp.gz` existe na raiz. Este é um arquivo BMP compactado gzipado de 640x480 e 24 bits. Substitua-o por um arquivo BMP diferente que você compactado, por exemplo. `gzip.exe --best .\boot_logo.bmp`, para alterar a logo de boot do GarlicOS.

### Mapeamento do MAME

`/CFW/config/mame.csv` é uma lista separada por vírgula do nome mame rom para um nome melhor, por ex.

`aligator,Alligator Hunt (World, protected)`

Se você descobrir que uma de suas roms do MAME não está exibindo um nome melhor, ela pode não estar nesta lista!

### Overlays do Retroarch

As imagens das overlays (arquivos .png) ficam em `/CFW/retroarch/.retroarch/overlay`.

### Diretórios do Retroarch

`/CFW/retroarch/.retroarch/retroarch.cfg` possui caminhos para arquivos e pastas interessantes, por ex.

```text
content_favorites_path = ":/.retroarch/content_favorites.lpl"
content_history_directory = "/mnt/SDCARD/Saves/CurrentProfile/lists"
content_history_path = "/mnt/SDCARD/Saves/CurrentProfile/lists/content_history.lpl"
savefile_directory = "/mnt/SDCARD/Saves/CurrentProfile/saves"
savestate_directory = "/mnt/SDCARD/Saves/CurrentProfile/states"
screenshot_directory = "/mnt/SDCARD/Screenshots"
```

### Logs do Retroarch

Se um jogo não iniciar, é possível que os logs do RetroArch lhe dêem alguma indicação do motivo.

Os logs são armazenados em `/CFW/retroarch/.retroarch/logs/retroarch.log`.

## FIM
## Creditos para: [milnak](https://gist.github.com/milnak): ele fez esse tutorial inteiro mas em ingles
