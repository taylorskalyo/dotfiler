#Dotfiler
Manage your configuration files easily with templating

##Installation
  1. ```git clone https://github.com/matthunz/dotfiler.git```
  2. ```cargo build --release```

  This creates a dotfiler executable under ~/bin. To run this, either add ~/bin to your PATH or move the file to /usr/bin

##Usage
  1. Move your file, for example xresources, into ```~/.config/dotfiler/templates```
  2. Make an entry for it inside config.toml with ```templatename = path/to/real/file```
  3. Replace any text inside to be changed with {{ variablename }} inside the template file
  4. Add the variable name under [themename] in config.toml
    Ex: [default]
  5. Run the program with ```dotfiler <themename>```
    If no theme name is specified, the program uses [default]
