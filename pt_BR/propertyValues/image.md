# Images (Imagens)

Para colocar imagens, você precisa delas em Algumas documentações recomendam o uso do módulo pip **Pillow**. Nesta documentação primeiro eu vou ensinar usando o próprio gerenciador de imagens do Tkinter, depois vou ensinar usando o Pillow.

## Usando o Gerenciador de imagens do Tkinter 

Uma ótima opção se seu programa é puramente python e você não quer nenhum pacote do PIP, ou se você não quer muita sofisticação e quer apenas usar GIFs e PNGs. Sim, Tk só suporta GIF e PNG nativamente.

```python
#Importando o módulo
from tkinter import *

root = Tk()
#Criando uma imagem do tipo PhotoImage
limg = PhotoImage(file='myImage.png')
#Colocando a imagem num Label e aplicando (sem criar a variável)
Label(root,image=limg).pack()
root.mainloop()
```

## Usando o Pillow

Uma ótima opção se seu programa precisa suportar mais tipos de imagens, além de GIF e PNG. Além de ter a possibilidade de mexer de uma maneira legal com a imagem, você

```python
#Importando o módulo, preste atenção a maneira que o PIL é importado, justamente por causa do conflito com o Image do Tk
from tkinter import *
from PIL import ImageTk
import PIL.Image as pImage

root = Tk()
#Aqui é criada uma imagem PhotoImage pelo PIL, que deriva de outra imagem criada pelo próprio PIL
limg = ImageTk.PhotoImage(pImage.open('myImage.png'))
#Esta imagem é posta normalmente no Label
Label(root,image=limg).pack()
#E voilá!
root.mainloop()
```
