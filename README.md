# macmini dotfiles
Meine MacOS-Dotfiles, um die Einstellungen des MacMinis zu sichern.

# Quick Start
## Homebrew installieren
Homebrew ist ein package manager für MacOS. Folge den Installationsanweiseungen [der offiziellen Dokumentation](https://brew.sh/).

## Clone Dotfiles
Im Userverzeichnis
```
git clone https://github.com/TorbDev/dotfiles_macmini.git .dotfiles
```

## Brewfile nutzen
Durch das *Brewfile* werde alle notwendigen Abhängigkeiten durch Homebrew geladen

Im Verzeichnis mit dem *Brewfile*
```
brew bundle
```

Um ein neues *Brewfile* zu erstellen
```
brew bundle dump --force
```

## Einstellungen symlinken
Im Userverzeichnis
```
cd .dotfiles
stow .
```

## create ssh keys
```
ssh-keygen -t rsa
pbcopy < ~/.ssh/id_rsa.pub
```