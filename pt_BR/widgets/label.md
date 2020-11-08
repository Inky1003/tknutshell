# Label (tkinter.Label)

## Descrição

​	Um texto ou uma imagem a ser apresentado para o usuário.

​	Podem ser apresentados ambos no mesmo Widget.

## Uso padrão:

```python
from tkinter import *
# Criar uma instância Tk chamada root
root = Tk()
# Criar um frame chamado myFrame na instância root
myLabel = Label(root)
# Aplicar o frame na instância root
myFrame.pack()
```

## Propriedades

### Propriedades Padrão

`class` - Esta classe não deve ser mudada, e diz respeito ao que o Widget é.

`compound` - Especifica como mostrar o texto e/ou imagem. Os seus valores podem ser 

​	`center` - Mostrar texto centralizado em cima da imagem.

​	`top/bottom/left/right` - Mostra a imagem acima, do lado direito/esquerdo ou embaixo da imagem.

​	`none` - Mostra a imagem se estiver presente, caso contrário o texto.

------

`cursor` - O cursor do mouse específico ao passar o mouse em cima do Frame. Veja em [Cursores](../propertyValues/cursors.md) alguns cursores disponíveis.

`image` - A imagem a ser exibida. Veja em [Imagens](../propertyValues/image.md)

`padding` - 

