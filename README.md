# SmartResume AI Checker 📃

An intelligent resume analysis tool powered by GPT-4o-mini that provides personalized feedback and improvement suggestions for job seekers. Upload your resume and get expert-level critiques tailored to your target role.

## 🚀 Features

- **Multi-Format Support**: Upload resumes in PDF or TXT format
- **AI-Powered Analysis**: Leverages OpenAI's GPT-4o-mini for expert-level resume critique
- **Role-Specific Feedback**: Tailored recommendations based on your target job role
- **Comprehensive Review**: Analyzes content clarity, skills presentation, and experience descriptions
- **User-Friendly Interface**: Clean, intuitive Streamlit web interface
- **Instant Results**: Get detailed feedback in seconds

## 🛠 Tech Stack

- **Python 3.8+**
- **Streamlit**: Web application framework
- **OpenAI API**: GPT-4o-mini for intelligent analysis
- **PyPDF2**: PDF text extraction
- **python-dotenv**: Environment variable management

## 📋 Prerequisites

- Python 3.8 or higher
- OpenAI API key
- Git

## ⚡ Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/tiennho2608/SmartResume-AI-Checker.git
   cd SmartResume-AI-Checker
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   Or if using `uv`:
   ```bash
   uv sync
   ```

3. **Set up environment variables**
   ```bash
   # Create .env file in the root directory
   echo "OPENAI_API_KEY=your_openai_api_key_here" > .env
   ```

4. **Run the application**
   ```bash
   streamlit run main.py
   ```

5. **Open your browser**
   - Navigate to `http://localhost:8501`
   - Start analyzing resumes!

## 📁 Project Structure

```
SmartResume-AI-Checker/
├── main.py              # Main Streamlit application
├── .env                 # Environment variables (create this)
├── .env.example         # Example environment file
├── .gitignore          # Git ignore rules
├── .python-version     # Python version specification
├── pyproject.toml      # Project dependencies and metadata
├── uv.lock            # UV lock file for dependencies
└── README.md          # This file
```

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

### Dependencies
The main dependencies include:
```
streamlit>=1.28.0
PyPDF2>=3.0.0
openai>=1.0.0
python-dotenv>=1.0.0
```

## 📖 How to Use

1. **Launch the Application**
   ```bash
   streamlit run main.py
   ```

2. **Upload Your Resume**
   - Click "Browse files" or drag and drop your resume
   - Supported formats: PDF, TXT

3. **Specify Target Role (Optional)**
   - Enter the job role you're targeting for personalized feedback
   - Example: "Software Engineer", "Data Scientist", "Marketing Manager"

4. **Get Analysis**
   - Click "Analyze Resume" button
   - Wait for AI-powered feedback (usually takes 5-10 seconds)

5. **Review Feedback**
   - Get structured analysis covering:
     - Content clarity and impact
     - Skills presentation
     - Experience descriptions
     - Role-specific improvements

## 🎯 Analysis Features

The AI Resume Critiquer evaluates your resume across multiple dimensions:

### Content Analysis
- **Clarity**: Checks for clear, concise language
- **Impact**: Identifies areas to quantify achievements
- **Relevance**: Ensures content aligns with target role

### Skills Assessment
- **Technical Skills**: Reviews technical competencies
- **Soft Skills**: Evaluates interpersonal abilities
- **Keyword Optimization**: Suggests industry-relevant terms

### Experience Review
- **Achievement Focus**: Recommends result-oriented descriptions
- **Action Verbs**: Suggests powerful action words
- **Quantification**: Identifies opportunities to add metrics

### Role-Specific Feedback
- **Industry Standards**: Compares against role expectations
- **Required Skills**: Highlights missing competencies
- **Format Suggestions**: Recommends optimal structure

## 🔒 Privacy & Security

- **No Data Storage**: Resumes are processed in memory only
- **Secure API Calls**: All communications with OpenAI are encrypted
- **Local Processing**: Text extraction happens locally
- **No File Retention**: Uploaded files are not saved to disk

## 🚨 Error Handling

The application handles common issues:
- **Empty Files**: Alerts when uploaded file has no content
- **Invalid Formats**: Validates file types before processing
- **API Errors**: Graceful handling of OpenAI API issues
- **Network Issues**: Informative error messages for connectivity problems

## 🔧 Troubleshooting

### Common Issues

**"OpenAI API key not found"**
```bash
# Make sure your .env file exists and contains:
OPENAI_API_KEY=your_actual_api_key
```

**"File has no content"**
- Ensure your PDF is not image-based (scanned)
- Try converting to text format first
- Check file permissions

**"Model not accessible"**
- Verify your OpenAI API key has GPT-4o-mini access
- Check your OpenAI account billing status

### Performance Tips

- **Optimal File Size**: Keep resumes under 2MB for faster processing
- **Clear Text**: Use standard fonts for better PDF extraction
- **Specific Roles**: Provide detailed job roles for better feedback

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. Commit your changes
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. Push to the branch
   ```bash
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request

## 📈 Future Enhancements

- [ ] **Multi-language Support**: Resume analysis in multiple languages
- [ ] **ATS Compatibility Check**: Assess resume compatibility with ATS systems
- [ ] **Industry Templates**: Provide role-specific resume templates
- [ ] **Comparison Feature**: Compare multiple resume versions
- [ ] **Export Options**: Download feedback as PDF or Word document
- [ ] **Batch Processing**: Analyze multiple resumes simultaneously
- [ ] **Integration APIs**: Connect with job boards and career platforms

## 🐛 Known Issues

- PDF text extraction may not work with image-based or heavily formatted PDFs
- Very large files (>5MB) may cause timeout issues
- Some special characters might not display correctly

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Support

If you encounter any issues:

1. Check the [Issues](https://github.com/tiennho2608/SmartResume-AI-Checker/issues) page
2. Create a new issue with:
   - Detailed problem description
   - Steps to reproduce
   - Error messages (if any)
   - Your environment details

## 🌟 Acknowledgments

- **OpenAI**: For providing the GPT-4o-mini API
- **Streamlit**: For the amazing web framework
- **PyPDF2**: For reliable PDF text extraction
- **Community**: Thanks to all contributors and users

---

**Made with ❤️ to help job seekers land their dream jobs**

## 📊 Stats

- **Processing Time**: ~5-10 seconds per resume
- **Supported Formats**: PDF, TXT
- **API Model**: GPT-4o-mini
- **Max File Size**: 10MB recommended
