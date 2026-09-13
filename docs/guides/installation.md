# Install and Run the Documentation Site

## Audience

This guide is for reviewers or contributors who want to run the portfolio locally.

## Prerequisites

- Git
- Python 3.10 or later
- A terminal with access to Python and pip

## Installation

1. Clone the repository and open its directory:

    ```bash
    git clone https://github.com/owlildrownit-dev/Portfolio.git
    cd Portfolio
    ```

2. Create a virtual environment:

    ```bash
    python -m venv .venv
    ```

3. Activate the environment.

    Windows PowerShell:

    ```powershell
    .venv\Scripts\Activate.ps1
    ```

    Linux or macOS:

    ```bash
    source .venv/bin/activate
    ```

4. Install the dependencies:

    ```bash
    python -m pip install -r requirements.txt
    ```

5. Start the local server:

    ```bash
    mkdocs serve
    ```

6. Open `http://127.0.0.1:8000`.

## Verification

Confirm that:

- the home page opens without a build error;
- the Portfolio navigation contains all samples;
- search returns results;
- the theme can switch between light and dark modes.

## Stop the server

Press `Ctrl+C` in the terminal where MkDocs is running.

## Troubleshooting

If `mkdocs` is not recognized, confirm that the virtual environment is active and run:

```bash
python -m mkdocs serve
```
