# nvim
Repositório destinado ao versionamento do meu arquivo de configuração do vim

O funcionamento da maior parte dos plugins depende de você deve ter o neovim >= 0.8

Caso não haja o neovim nessa versão nos repositórios da sua distro eu recomendo que instale o neovim usando os seguintes comandos:
```sh
$ git clone https://github.com/neovim/neovim
$ cd neovim
$ make CMAKE_BUILD_TYPE=RelWithDebInfo
$ sudo make install
```
<p>
instale as seguintes dependências:
  
```sh
$ sudo apt install git build-essential cmake git pkg-config libtool g++ libunibilium4 libunibilium-dev \
ninja-build gettext libtool libtool-bin autoconf automake unzip curl doxygen lua-term lua-term-dev luarocks
```
Vá ao .config e clone o repositório

```sh
$ cd ~/.config/
$ git clone https://github.com/Josefreitas788/nvim.git
```

Adicione as fontes que est repositório do terminalroot, é importante para que os icones apareçam
<p>
    https://github.com/wbthomason/packer.nvim#requirements
    <p>  

Adicione o gerenciador de plugins
```sh
$ git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
 ```

  
Esse é o link do gerenciador(antes de executar o PackerInstall você precisa comentar algumas partes do código com erros na primeira vez que for executar):
 
  ```sh
  :PackerInstall
 ```

Siga os seguintes passos se desejar instalar o GitHub Copilot:
```sh
$ git clone https://github.com/github/copilot.vim \
   ~/.config/nvim/pack/github/start/copilot.vim
 ```
```sh
:Copilot setup
:Copilot enable
```
 
Talves seja preciso adicionar essa dependência:
```sh
$ sudo luarocks install luafilesystem
```


Para o plugin de linguagens funcionar, ela precisa estar no ```$PATH```, como eu uso o "asdf", coloquei o seguinte comando no .bashrc

#GOPATH -> Você consegue o com o comando "go env"
```sh
export PATH="$HOME/.asdf/installs/golang/1.19.5/packages/bin:$PATH"
```


obs: pretendo ir adicionando plugins conforme for sentindo a necessidade

