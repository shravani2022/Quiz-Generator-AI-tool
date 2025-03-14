# Quiz-Generator-AI-tool
An AI-powered application that automatically generates educational quizzes from images, PDFs, and text content using Natural Language Processing (NLP) techniques.

## Overview

This application allows users to upload educational content (images or PDFs) or enter text directly, and automatically generates quiz questions based on the content. It uses state-of-the-art NLP models to analyze the content and create relevant questions.



## Features

- **Multiple Input Types**: Upload images, PDFs, or enter text directly
- **AI-Powered Question Generation**: Automatically creates quiz questions from the content
- **Interactive Quiz Interface**: Take quizzes with a user-friendly interface
- **Results and Explanations**: View your score and explanations for each question
- **Responsive Design**: Works on desktop and mobile devices




## Folder Structure

```plaintext
educational-quiz-generator/
│
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
├── LICENSE                 # License information
│
├── static/                 # Static files
│   ├── css/
│   │   └── style.css       # CSS styles
│   ├── js/
│   │   └── script.js       # Frontend JavaScript
│   └── img/                # Images for the UI
│       └── logo.png
│
├── templates/              # HTML templates
│   └── index.html          # Main application page
│
├── uploads/                # Temporary folder for uploaded files
│
└── models/                 # Model files (optional, for offline models)
```

## Technologies Used

- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, JavaScript
- **AI/ML**:

- Transformers library for NLP
- Vision Encoder-Decoder model for image captioning
- T5 model for question generation



- **Data Processing**: PyPDF2 for PDF text extraction, PIL for image processing


## Installation

1. Clone the repository:


```shellscript
git clone https://github.com/yourusername/educational-quiz-generator.git
cd educational-quiz-generator
```

2. Create a virtual environment (recommended):


```shellscript
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required dependencies:


```shellscript
pip install -r requirements.txt
```

4. Run the application:


```shellscript
python app.py
```

5. Open your web browser and navigate to `http://localhost:5000`


## Usage

1. **Upload Content or Enter Text**:

1. Click "Browse Files" to upload an image or PDF
2. Or enter educational text in the text area



2. **Generate Quiz**:

1. Click "Generate Quiz" to create questions based on your content



3. **Take the Quiz**:

1. Answer each question by selecting an option
2. Navigate through questions using the "Previous" and "Next" buttons



4. **View Results**:

1. See your score and review your answers
2. Read explanations for each question





## How It Works

1. **Content Processing**:

1. Images are processed using a Vision Encoder-Decoder model to generate textual descriptions
2. PDFs are processed by extracting text content
3. Text input is used directly



2. **Question Generation**:

1. The text content is analyzed using a T5-based question generation model
2. The model identifies key concepts and creates relevant questions



3. **Quiz Creation**:

1. Multiple-choice options are generated for each question
2. The quiz is presented to the user in an interactive format





## Customization

You can customize the application by:

1. **Changing the Models**:

1. Replace the question generation model in `app.py`
2. Use a different image captioning model



2. **Modifying the UI**:

1. Edit the CSS in `static/css/style.css`
2. Update the HTML in `templates/index.html`



3. **Adding Features**:

1. Implement user authentication
2. Add a database to store quiz results
3. Create a teacher dashboard for managing quizzes





## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- The Transformers library by Hugging Face
- The Flask web framework
- All the open-source contributors who made this project possible


---

## Future Improvements

- Implement more sophisticated question generation techniques
- Add support for more file types (e.g., DOCX, PPTX)
- Improve the quality of generated answer options
- Add more question types (e.g., true/false, fill-in-the-blank)
- Implement a spaced repetition system for learning
