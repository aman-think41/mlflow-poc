
## Installation Steps

1. **Clone the Repository**
   Open your terminal and run the following command to clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Create a Virtual Environment**
   Create a virtual environment to manage dependencies:
   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies**
   Install the required packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

5. **Set Up Environment Variables**
   Create a `.env` file in the root directory of the project and add the necessary environment variables. You can refer to the `.env.example` file for guidance.

6. **Start MLFlow Tracking Server**
   ```bash
   mlflow ui
   ```
7. **Setup required files**
    - Create a `questions.json` file in the root directory of the project and add the questions you want to test.
    - Create a `guidelines.txt` file in the root directory of the project and add the guidelines for the persona.

8. **Run the Tests**
   ```bash
   python3 runner.py
   ```


You should see the tests running and the results in the MLFlow UI.