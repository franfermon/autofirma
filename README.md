# autofirma

Autofirma solo inicia con java 11. Para poder hacerlo, hay que hacer sudo alternatives --config java en consola y seleccionar 11. Una vez hecho ya inicia

## temurin

Parece que Fedora ha hecho drop java 11

```sudo rpm --import https://packages.adoptium.net/artifactory/api/gpg/key/public```
```sudo tee /etc/yum.repos.d/adoptium.repo <<EOF```
```
[Adoptium]
name=Adoptium
baseurl=https://packages.adoptium.net/artifactory/rpm/fedora/\$releasever/\$basearch
enabled=1
gpgcheck=1
EOF
```
```sudo dnf install temurin-11-jdk``
