```markdown
# image_processing

## Description
The `image_processing` package is designed to help you transform and analyze images. It includes:

### Processing:
- **Histogram Matching:** Align the colors of different images.
- **Structural Similarity:** Measure the similarity between two images.
- **Resize Image:** Adjust the size of your images.

### Utils:
- **Read Image:** Load images from your files.
- **Save Image:** Store images back to your disk.
- **Plot Image:** Display images for viewing.
- **Plot Result:** Show the results of your transformations.
- **Plot Histogram:** Visualize the color distribution of images.

## Installation

To install the package, use the package manager [pip](https://pip.pypa.io/en/stable/):

```bash
pip install almighty-image-processing
```

## How to Use

1. Import the necessary modules from the package.
2. Read the images you want to process.
3. Use the available functions for processing, plotting, and saving.

### Example:

```python
from image_processing.utils import io, plot
from image_processing.processing import combination, transformation

# Read images
image1 = io.read_image('path_to_image1.jpg')
image2 = io.read_image('path_to_image2.jpg')

# Plot the images
plot.plot_image(image1)
plot.plot_image(image2)

# Apply histogram transfer
result_image = combination.transfer_histogram(image1, image2)

# Plot the result
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
**AlmigthyMatheus**

## License
This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).