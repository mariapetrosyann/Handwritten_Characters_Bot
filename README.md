# Handwritten Characters Recognition Telegram Bot

This project aims to develop a Telegram bot that recognizes handwritten Characters from images. The bot uses a Convolutional Neural Network (CNN) trained on a dataset of handwritten characters, digits, and symbols. The bot can handle images of various sizes by resizing them before making predictions.

## Project Structure

- `Validation/`: Contains the dataset of handwritten characters, digits, and symbols.
- `handwritten_text_recognition.py`: Python script for training the model and running the Telegram bot.
- `handwritten_text_recognition.ipynb`: Jupyter Notebook for training the model and running the Telegram bot within Google Colab.

## Dataset

The dataset contains 39 classes of handwritten characters, digits, and symbols, each stored in separate folders. The structure is as follows:

```
Validation/
│
└───Validation/
    │
    ├───#/
    │   ├───img1.png
    │   └───...
    │
    ├───$/
    │   ├───img.png
    │   └───...
    │
    └───... (other symbols, digits, and letters)
```

## Getting Started

### Prerequisites

- Python 3.7+
- TensorFlow
- Keras
- NumPy
- Pillow
- python-telegram-bot

### Installation

1. Clone the repository:

```bash
git clone https://github.com/your_username/Handwritten_Characters_Bot.git
cd HandwrittenCharacters
```

2. Install the required libraries:

```bash
pip install tensorflow numpy pillow python-telegram-bot
```

### Training the Model

To train the model, you can use the `handwrittencharacters.py` script or the `HandwrittenCharacters.ipynb` Jupyter Notebook.

#### Using the Python Script

1. Run the script:

```bash
python handwrittencharacters.py
```

#### Using the Jupyter Notebook

1. Open the notebook:

```bash
jupyter notebook handwritten_text_recognition.ipynb
```

### Running the Telegram Bot

To run the Telegram bot, ensure that you have a trained model available. You can either train a new model using the steps above or use the provided `trained_model.h5`.

1. Edit the `handwrittencharacters.py` script to include your Telegram bot token:

```python
application = ApplicationBuilder().token("Replace_with_your_token").build()  # Replace with your token
```

2. Run the bot:

```bash
python handwrittencharacters.py
```
### Telegram Bot

The link of the Telegram Bot: https://t.me/DzeragirBot
`Please note that the Bot will not work any time, because I used my computer server to run the Bot`

### Usage

1. Start the bot by sending the `/start` command.
2. Send a photo of handwritten text to the bot.
3. The bot will recognize the text and reply with the recognized characters.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any suggestions or improvements.

## Acknowledgments

Special thanks to the creators of the dataset and the open-source libraries used in this project.
