
# Mach Door CAM Config

Addon/Plugin para Freecad para configuração dos parametros utilizados na geração de arquivos gcode para a Mach Door, produzida pela Mach CNC.


## Pré-requisitos

Freecad 1.0 devidamente instalado. Baixe gratuitamente de [freecad.org/downloads](https://www.freecad.org/downloads.php)
## Licença

O Software Freecad está licenciado sob a licença [LGPL2+](http://en.wikipedia.org/wiki/LGPL). Esse plugin também está licenciado sob a licença LGPL2.


## Instalação

Esse plugin não requer a execução de um instalador. Apenas baixe e descompacte o arquivo [MachDoorCAMConfig.zip](https://github.com/thomasvieira/machdoorcamconfig/blob/main/MachDoorCAMConfig.zip) na pasta MOD do Freecad e reinicie o Freecad. Tipicamente no Windows o caminho para a pasta MOD é ***C:\Users\Username\AppData\Roaming\FreeCAD\Mod*** onde Username é o nome de usuário do Windows.

Os arquivos ***mach_door_borda_direita_post.py, mach_door_borda_esquerda_post.py e mach_door_face_superior_post.py*** devem ser baixados colocados na pasta ***C:\Program Files\FreeCAD 1.0\Mod\CAM\Path\Post\scripts***

Também serão necessários os arquivos de macro e de template disponíveis [aqui](https://github.com/thomasvieira/machdoormacros). Esses arquivos devem ser copiados para a pasta Macro do Freecad. Tipicamente no Windows o caminho para a pasta Macro é ***C:/Users/Username/AppData/Roaming/FreeCAD/Macro*** onde Username é o nome de usuário do Windows.
## Utilização

Após a criação do corpo que você deseja usinar, execute os seguintes passos:

    1. Execute a macro "CriarCopias.FCMacro" e clique em OK na janela que abrir.
    2. Execute a macro "CriaTarefaFaceSuperior.FCMacro"
    3. Execute a macro "CriaTarefaBordaDireita.FCMacro"
    4. Execute a macro "CriaTarefaBordaEsquerda.FCMacro"
    5. Execute a macro "MostraModelo1.FCMacro"
    6. Execute a macro "MostraModelo2.FCMacro"
    7. Execute a macro "MostraModelo3.FCMacro"
    8. Execute novamente a macro "MostraModelo1.FCMacro"
    9. Selecione os contornos e faces a serem usinados e adicione a(s) operação(ções) necessárias.
    10. Execute novamente a macro "MostraModelo2.FCMacro"
    11. Selecione os contornos e faces a serem usinados e adicione a(s) operação(ções) necessárias.
    12. Execute novamente a macro "MostraModelo3.FCMacro"
    13. Selecione os contornos e faces a serem usinados e adicione a(s) operação(ções) necessárias.
    14. Execute a macro "Gerar_gcode_Face.FCMacro"
    15. Execute a macro "Gerar_gcode_Borda_Direita.FCMacro"
    16. Execute a macro "Gerar_gcode_Borda_Esquerda.FCMacro"
    17. Execute a macro "Gera_arquivo_de_corte_completo.FCMacro"

Seu arquivo estará disponível na pasta PostProcess
