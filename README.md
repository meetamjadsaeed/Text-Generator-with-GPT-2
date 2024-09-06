# Text Generator with GPT-2

This project demonstrates a simple text generation application using the GPT-2 model from Hugging Face's Transformers library. The application allows users to input some initial text, and then it generates additional text based on the input.

## Features

- **Text Generation**: Uses GPT-2 for generating text based on user input.
- **Interactive Interface**: Provides a web-based interface for users to input text and generate more content.
- **Probabilistic Sampling**: Implements sampling with a probability threshold to control text generation diversity.

## Dependencies

The project requires the following Python libraries:

- `numpy`
- `torch`
- `transformers`
- `panel`

You can install them using the following command:

```bash
pip install numpy torch transformers panel
```

## How It Works

1. **Model and Tokenizer Initialization**:
   - Loads the GPT-2 tokenizer and model from Hugging Face.

2. **Text Generation Function**:
   - Defines `get_pred()` to generate text based on a given input using the GPT-2 model.
   - Applies softmax to logits to get probabilities, sorts them, and samples the next token based on a probability threshold.

3. **Interactive Panel Application**:
   - Uses the Panel library to create a web interface with a text input widget and a button to generate text.
   - Links the text input widget to a display area and updates it with generated text on button click.

4. **Web Interface**:
   - Displays an interactive UI with options to input text, generate additional text, and view results.

## Usage

1. Run the script:

    ```bash
    python script_name.py
    ```

2. Open the web interface in your browser. You can enter initial text and click the "Generate" button to generate more text.

## Example

![Text Generator Interface](./path/to/screenshot.png)  <!-- Replace with actual screenshot path -->

## License

This project is open-source and available under the MIT License.
