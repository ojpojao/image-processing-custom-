<p align="center">
  <img src="https://hermes.dio.me/tracks/2a3a2d2b-7de7-457c-b4df-dcd327eae9eb.png" style="height: 200px; width:200px;"/>
</p>

# Image Processing Custom

## Bootcamp NTT DATA - Engenharia de Dados com Python
### Desafio de Projeto: Criando um Pacote de Processamento de Imagens com Python


### Descrição
Os recursos do pacote image_processing_custom_ são:

    Processamento:
        - correspondência de histograma
        - semelhança estrutural
        - redimensionamento de imagem
    Utilidades:
        - ler imagem
        - salvar imagem
        - plot de imagem
        - plot de resultados
        - plot de histogramas

### Instalação

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install image_processing_custom

```bash
python3 -m venv venv
source venv/bin/activate
pip install -U pip
pip install image_processing_custom
```

### Uso

```python
from image_processing_custom.utils import io, plot
from image_processing_custom.processing import combination, tranformation


image1_test = "image1_example.jpg"
image2_test = "image2_example.jpg"

image1 = io.read_image(image1_test)
image2 = io.read_image(image2_test)

plot.plot_image(image1)
plot.plot_image(image2)

result_image = combination.transfer_histogram(image1, image2)
plot.plot_result(image1, image2, result_image)
```

## Autor
ojpojao

## License
[MIT](https://choosealicense.com/licenses/mit/)
