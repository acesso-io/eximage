# Eximage Android

Este projeto visa facilitar a leitura e manipulação de imagens capturadas pela câmera do Android.

### Pré requisitos

- Android Studio - IDE oficial de desenvolvimento Google. Versão 9 ou superior
- Maven Jitpack - Gerenciador de bibiotecas para a IDE.

### Instalando

- Abra o arquivo build.gradle (Projeto) e adicione Jitpack manager em repositorios, seu código deve parecer com isto: 

```groovy
allprojects {
    repositories {
        google()
        jcenter()
        maven { url 'https://jitpack.io'}
        }
}
```

- Em seguida, abra o arquivo build.gradle (App) e implemente nossa dependência em seu projeto: 

```
 implementation 'com.github.acesso-io:eximage:1.0.0@aar'
```

- Importe na sua classe de preferência para utilização.

```java
import br.com.acessodigital.eximage.exif.Exif;
```

Pronto! O seu projeto já está pronto para o uso de nossa biblioteca.

## Utilização

Todas os métodos pode ser acessados pela classe: 

```java
br.com.acessodigital.eximage.Eximage
```

Na mesma classe é possível obter:
 - Dados exif da imagem
 - Orientação
 - Conversão de Bitmap para JPEG
 - Rotacionar Bitmap
 - Espelhar Bitmap
 - Converter de YUV420 (formato nativo do buffer da câmera) para JPEG
 - Converter de NV21 para JPEG
 - Converter de YUV420  para NV21
 - Rotacionar o YUV420 em 90, 180 e 270 graus
 