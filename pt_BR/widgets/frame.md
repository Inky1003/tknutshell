# Frame (tkinter.Frame)

## Descrição

​	Um container para outros widgets. Cria um espaço no programa para organizar seus widgets.

## Uso padrão:

```python
from tkinter import *
# Criar uma instância Tk chamada root
root = Tk()
# Criar um frame chamado myFrame na instância root
myFrame = Frame(root)
# Aplicar o frame na instância root
myFrame.pack()
```

### Propriedades

#### Propriedades Padrão

`borderwidth` - O tamanho da borda do Frame em pixels

`cursor` - O cursor do mouse específico ao passar o mouse em cima do Frame. Veja em Cursores alguns cursores disponíveis.

`highlightbackground` - Especifica a cor do retângulo que contorna o Frame quando não há foco do usuário nele.

`highlightcolor` - Especifica a cor do retângulo que contorna o Frame quando há foco do usuário nele.

`highlightthickness` - Tamanho do retângulo que contorna o Frame de acordo com o foco do usuário.

`padx` - Indica quanto espaço extra o Widget deve ter na direção X. Se o elemento  pai (por exemplo outro Frame ou a própria janela em si) pode oferecer tal espaçamento, o Widget apresentará um espaço horizontal a mais dentro de si mesmo e dentro desse espaço o conteúdo.

`pady` - Indica quanto espaço extra o Widget deve ter na direção Y. Se o elemento  pai (por exemplo outro Frame ou a própria janela em si) pode oferecer tal espaçamento, o Widget apresentará um espaço vertical a mais dentro de si mesmo e dentro desse espaço o conteúdo.

`relief` - Efeito 3D que o Widget pode ter. Valores para esta propriedade podem ser `raised`,`sunken`, `flat`,`ridge`,`solid` e `groove`.

`takefocus` - Quando você aperta Tab, dependendo do valor que você põe nesta propriedade, o objeto selecionado vem na sua ordem definida por esta propriedade. Exemplo: Se Frame1 tiver essa propriedade como 1 e Frame2 como 2, ao apertar Tab várias vezes, primeiro Frame1 será selecionado e depois Frame2.

#### Propriedades específicas do Widget

`background` - Cor de Background do Frame. Pode não ser definida, sendo uma string vazia.

`class` - Esta classe não deve ser mudada, e diz respeito ao que o Widget é.

`colormap` - Define um mapa de cores para ser usado com a Frame.

`container` Valor booleano (true ou false) que indica se um aplicativo vai ser embutido neste Frame.

`height` - Altura em pixels da janela

`width` - Largura em pixels da janela

`visual` - Especifica informações visuais para todas as formas

## Funções do widget

`cget` - obtém um valor de uma propriedade do Widget.

Uso: `valor = myFrame.cget(propriedade)`

`configure` - Uma das opções para configurar uma propriedade do Widget.

Uso: `myFrame.configure(propriedade=valor)`