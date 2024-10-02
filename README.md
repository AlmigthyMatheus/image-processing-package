```markdown
# image_processing

## Description
The package `image_processing` is used to:

### Processing:
- Histogram matching
- Structural similarity
- Resize image

### Utils:
- Read image
- Save image
- Plot image
- Plot result
- Plot histogram

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install `almighty-image-processing`.

```bash
pip install almighty-image-processing
```

## Usage

```python
from image_processing.utils import io, plot
from image_processing.processing import combination, transformation

image1 = io.read_image('path_to_image1.jpg')
image2 = io.read_image('path_to_image2.jpg')

plot.plot_image(image1)
plot.plot_image(image2)

result_image = combination.transfer_histogram(image1, image2)

plot.plot_result(image1, image2, result_image)
```

## Project Structure
```
image-processing-package/
│
├── image_processing/
│   ├── __init__.py
│   ├── utils/
│   │   ├── io.py
│   │   └── plot.py
│   └── processing/
│       ├── combination.py
│       └── transformation.py
│
├── tests/
│   └── test_processing.py
│
├── README.md
├── setup.py
├── requirements.txt
└── LICENSE
```

## Author
AlmigthyMatheus

## License
[MIT](https://choosealicense.com/licenses/mit/)
