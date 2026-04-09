# Sentiment API AI

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![AI](https://img.shields.io/badge/AI-Powered-purple)
![License](https://img.shields.io/badge/License-MIT-green)

An AI-powered sentiment analysis API that classifies text into positive, negative, or neutral sentiment with confidence scores. Provides a REST API interface for real-time sentiment detection in reviews, social media, and customer feedback.

---

## Features

- **Sentiment Classification** -- Categorizes text as positive, negative, or neutral
- **Confidence Scoring** -- Returns probability scores for each sentiment class
- **Aspect-Based Analysis** -- Detects sentiment toward specific topics within text
- **REST API** -- Production-ready API endpoint for integration with any application
- **Batch Analysis** -- Process multiple texts in a single API call
- **Language Support** -- Handles sentiment analysis across multiple languages

---

## Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.9+ | Core runtime |
| OpenAI / LLM API | Sentiment inference |
| FastAPI / Flask | REST API framework |
| Makefile | Build and test automation |

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/sentiment-api-ai.git
cd sentiment-api-ai

# Install dependencies
pip install -r requirements.txt

# Start the API server
python core/ai_worker.py --serve --port 8000
```

---

## Project Structure

```
sentiment-api-ai/
├── core/
│   └── ai_worker.py       # Main AI processing engine
├── Makefile                # Build and test commands
├── LICENSE                 # MIT License
├── SECURITY.md             # Security policy
└── README.md
```

---

## API Usage

```bash
# Analyze sentiment
curl -X POST http://localhost:8000/analyze \
  -H "Content-Type: application/json" \
  -d '{"text": "This product is excellent!"}'
```

---

## Usage

```bash
# Build the project
make build

# Run tests
make test
```

---

## Contributing

1. Fork the repository
2. Create a feature branch -- `git checkout -b feature/your-feature`
3. Commit your changes -- `git commit -m "feat: add new feature"`
4. Push and open a Pull Request

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**Built by [Razin Ahmed](https://github.com/razinahmed)**
