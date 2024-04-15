# NLG Library

This is a simple Natural Language Generation (NLG) library for JavaScript. It provides basic functionality for generating sentences and paragraphs based on provided data.

## Installation

You can install the NLG library via npm:

```bash
npm install nlg-library
```

## Usage

```javascript
const NLG = require('nlg-library');

// Initialize NLG instance
const nlg = new NLG();

// Generate a sentence
const sentence = nlg.generateSentence({ name: 'John', weather: 'sunny' });
console.log(sentence);
// Output: "Hello, John! Today's weather is sunny."

// Generate a paragraph
const paragraph = nlg.generateParagraph({ name: 'Alice', weather: 'cloudy' }, 3);
console.log(paragraph);
// Output: "Hello, Alice! Today's weather is cloudy. Hello, Alice! Today's weather is cloudy. Hello, Alice! Today's weather is cloudy."
```

## API

### `new NLG()`

Creates a new instance of the NLG library.

### `generateSentence(data)`

Generates a single sentence based on the provided data.

- `data` (Object): Data object containing information to be included in the sentence.

### `generateParagraph(data, numSentences)`

Generates a paragraph containing the specified number of sentences.

- `data` (Object): Data object containing information to be included in the sentences.
- `numSentences` (Number): The number of sentences to generate in the paragraph.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
