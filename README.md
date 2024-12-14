# nvim-conf
basado en https://github.com/bcampolo/nvim-starter-kit/

instalo las dependencias 
```
sudo apt install ripgrep xclip npm
```

luego respaldo la carpeta de configuracion de Neovim y los estados actuales (opcional)
```
mv ~/.config/nvim{,.bak}

mv ~/.local/share/nvim{,.bak}
mv ~/.local/state/nvim{,.bak}
mv ~/.cache/nvim{,.bak}
```

- me pongo en la carpeta de configuraciones
- clono el repositorio
- cambio el nombre para que coincida con el de neovim
- re-ubico la carpeta de fonts para que funcionen los íconos (NerdFontsSymbolsOnly)
- hago rebuild del cache para que se puedan utilizar las fuentes para los iconos
```
cd ~/.config
git clone https://github.com/NeiraDiego/nvim-conf
mv neovim-conf neovim
mkdir ~/.fonts
mv neovim/NerdFontsSymbolsOnly ~/.fonts/
fc-cache -f -v
```
