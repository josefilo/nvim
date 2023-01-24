# nvim
Repositório destinado ao versionamento do meu arquivo de configuração do vim

O funcionamento da maior parte dos plugins depende de você deve ter o neovim >= 0.8
<p>
instale as seguintes dependências:
  
```sh
sudo apt install git build-essential cmake git pkg-config libtool g++ libunibilium4 libunibilium-dev \
ninja-build gettext libtool libtool-bin autoconf automake unzip curl doxygen lua-term lua-term-dev luarocks
```
Vá ao .config e clone o repositório

```sh
cd ~/.config/
git clone https://github.com/Josefreitas788/nvim.git
```

Adicione as fontes que est repositório do terminalroot, é importante para que os icones apareçam
<p>
    https://github.com/wbthomason/packer.nvim#requirements
    <p>  

Adicione o gerenciador de plugins
```sh
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
 ```

  
Esse é o link do gerenciador(antes de executar o PackerInstall você precisa comentar algumas partes com erro do código na primeira vez que for executar):
 
  ```sh
  :PackerInstall
 ```

Siga os seguintes passos se desejar instalar o GitHub Copilot:
```sh
git clone https://github.com/github/copilot.vim \
   ~/.config/nvim/pack/github/start/copilot.vim
 ```
 ```sh
:Copilot setup
:Copilot enable
 ```
 
Talves seja preciso adicionar essa dependência:
```sh
sudo luarocks install luafilesystem
```



obs: pretendo ir adicionando plugins conforme for sentindo a necessidade
