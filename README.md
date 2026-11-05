# 🧪 Agentic API Testing & Documentation Generator

An AI-powered API testing and documentation project built with Python and Generative AI. It reads OpenAPI specifications, discovers endpoints, generates test scenarios, executes safe tests, analyzes results, and automatically creates API documentation.

## ✨ Features

- 📄 OpenAPI 3.x JSON/YAML specification support
- 🔎 Automatic API endpoint discovery
- 🧪 Positive, negative, and boundary test generation
- 🤖 LLM-assisted test scenario generation
- ⚡ Automated demonstration test execution
- ✅ Expected-versus-actual result validation
- 📝 Automatic Markdown API documentation
- 📊 CSV and JSON test reports
- 🧑‍💻 Human-reviewed AI recommendations

## 🛠️ Tech Stack

- Python
- Jupyter Notebook
- Pandas
- PyYAML
- JSON Schema
- OpenAI-compatible API
- Generative AI
- Python-dotenv

## 📂 Project Structure

```text
agentic-api-testing-documentation-generator/
│
├── agentic_api_testing_documentation_generator.ipynb
├── README.md
├── requirements.txt
├── .env.example
└── .gitignore
```

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/agentic-api-testing-documentation-generator.git

cd agentic-api-testing-documentation-generator
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the LLM API (Optional)

Create a `.env` file using `.env.example`.

```env
OPENAI_API_KEY=your_api_key_here
OPENAI_BASE_URL=
OPENAI_MODEL=gpt-4.1-mini
```

You can use an OpenAI-compatible provider by configuring its base URL and supported model.

Never upload your actual API key or `.env` file to GitHub.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
agentic_api_testing_documentation_generator.ipynb
```

Run the notebook cells from top to bottom.

## 🧠 How It Works

1. Load an OpenAPI specification.
2. Discover API endpoints and their request/response details.
3. Generate test scenarios from the API contract.
4. Optionally use an LLM to suggest additional test cases.
5. Execute a controlled test suite against a mock API.
6. Compare expected and actual response codes.
7. Generate API documentation automatically.
8. Export test cases and execution reports.

## 📊 Example Use Case

Consider a Task Management API containing:

- GET `/tasks`
- POST `/tasks`
- GET `/tasks/{task_id}`
- DELETE `/tasks/{task_id}`

The project discovers these endpoints, generates test scenarios, executes the demonstration tests against an in-memory API, and creates documentation describing the endpoints and their responses.

## 📁 Generated Outputs

The notebook creates an `api_test_output` directory containing:

- `generated_test_cases.csv`
- `test_results.csv`
- `test_report.json`
- `api_documentation.md`

## ⚠️ Current Limitations

- The demonstration executor uses an in-memory mock API rather than a live server.
- Advanced OpenAPI `$ref` resolution is not fully implemented.
- LLM-generated test scenarios require human review.
- Complete pytest generation and live staging-environment execution are future enhancements.

## 🔮 Future Enhancements

- Generate executable pytest test scripts.
- Integrate Postman collections.
- Add response-schema validation.
- Support authenticated staging API testing.
- Integrate GitHub Actions CI/CD.
- Add API test coverage analytics.
- Add intelligent failure classification.
- Integrate Jira and Slack reporting.
- Add human-approved state-changing test execution.

## 🔐 Responsible API Testing

- Test only APIs you own or have explicit permission to assess.
- Prefer mock or staging environments.
- Keep destructive tests disabled by default.
- Never expose API credentials or private specifications.
- Review AI-generated test cases before execution.

## 📄 License

Choose a license such as MIT before publishing and add the corresponding `LICENSE` file.

---

**Built with Python | OpenAPI | API Testing | Generative AI | LLM Agents**
