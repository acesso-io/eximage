## :rocket: Sobre o nossa Biblioteca Eximage-Android

Este projeto visa facilitar a leitura, manipulação e verificação dos metadados de imagens capturada no Android, e oference os seguintes recursos:

 - Extração de dados exif da imagem
 - Informações de orientação (pelo buffer do preview e captura)
 - Conversão de Bitmap para JPEG
 - Rotação da imagem em 90°, 180° e 270° (Bitmap, JPEG, YUV, NV21)
 - Espelhamento (flipx)
 - Conversão de YUV420 (formato nativo do buffer da câmera) para JPEG
 - Conversão de NV21 para JPEG
 - Conversão de YUV420  para NV21

### Pré requisitos

- Android Studio - IDE oficial de desenvolvimento Google. Versão 9 ou superior
- Maven Jitpack - Gerenciador de bibiotecas para a IDE.

### Instalação

Abra o arquivo build.gradle (Projeto) e adicione Jitpack manager em repositorios, seu código deve parecer com isto: 

```groovy
allprojects {
    repositories {
        google()
        jcenter()
        maven { url 'https://jitpack.io'}
        }
}
```

Em seguida, abra o arquivo build.gradle (App) e implemente nossa dependência em seu projeto: 

```
 implementation 'com.github.acesso-io:eximage:1.0.8@aar'
```

Importe a classe

```java
import br.com.acessodigital.eximage.Eximage;
```

Pronto! 

Você já consegue utilizar a nossa biblioteca.

## Utilização

Todas os métodos podem ser acessados pela classe: 

```java
br.com.acessodigital.eximage.Eximage
```
 
## Versionamento

Nós usamos [Github](https://github.com/) para versionar. Para as versões disponíveis, veja as [tags do repositório](https://github.com/acesso-io/eximage/releases). 

## Autores

* **Rafael Martins da Costa** - *Engenheiro de Software* - [GitHub](https://github.com/rafaelmartinsdacosta)

Veja também nossa lista de [contribuidores](https://github.com/acesso-io/eximage/graphs/contributors) que participaram deste projeto.


Feito com ♥ by Acesso Digital - [Visita nosso Site!](https://acesso.io)
