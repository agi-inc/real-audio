# Real Audio - AGI SDK Agent

A demonstration agent using voice to perform automated web actions using the AGI SDK framework.

## Prerequisites

- Python 3.8 or higher
- OpenAI API key (or compatible provider)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/agi-inc/real-audio
   cd real-audio
   ```

2. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your API key:**

   ```bash
   export OPENAI_API_KEY="your-api-key"   # any supported provider key works
   ```

4. **Set up playwright:**
   ```python
   playwright install chromium --force
   ```

## Usage

Run the agent with default settings:

```bash
python run_agent.py
```

### Command Line Options

- `--model`: Model to use (default: gpt-4o)
- `--task`: Task to run (default: webclones.omnizon-1)
- `--headless`: Run in headless mode (default: False)

### Examples

```bash
# Run with a specific task
python run_agent.py --task webclones.dashdish-1

# Run in headless mode
python run_agent.py --headless true

# Run with different model
python run_agent.py --model gpt-4-turbo
```

## Available Tasks

The project includes audio tasks for various web applications:

- **dashdish**: Restaurant/food delivery platform tasks
- **fly-unified**: Flight booking platform tasks
- **gocalendar**: Calendar application tasks
- **gomail**: Email application tasks
- **networkin**: Professional networking platform tasks
- **omnizon**: E-commerce platform tasks
- **opendining**: Restaurant reservation platform tasks
- **staynb**: Accommodation booking platform tasks
- **topwork**: Job platform tasks
- **udriver**: Ride-sharing platform tasks
- **zilloft**: Real estate platform tasks

## Troubleshooting

Agent logs are stored in

1. **API Key Issues**: Ensure your OPENAI_API_KEY is properly set and has sufficient credits
2. **Dependencies**: Make sure all requirements are installed with `pip install -r requirements.txt`
3. **Browser Issues**: If running in GUI mode, ensure you have a display available

## Dependencies

- `agisdk`: AGI SDK framework
- `playwright`: Browser automation
- `numpy`: Numerical computing
- `openai`: OpenAI API client
- `Pillow`: Image processing
