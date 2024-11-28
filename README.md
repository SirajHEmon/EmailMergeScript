# CSV Email Merger Microapp

This is a simple Flask-based web application designed to merge two CSV files based on email addresses. The app reads a **Main CSV** containing emails and a **Data CSV** with additional data (including emails) and generates a new CSV file that only includes data corresponding to the emails in the **Main CSV**.

### Features:
- **Upload Two CSV Files**: One CSV file with a list of emails (`Main CSV`) and one CSV file with emails and corresponding data (`Data CSV`).
- **Merge on Email Column**: The application matches emails in the **Main CSV** with the emails in the **Data CSV** and merges the corresponding data.
- **Excludes Extra Emails**: Only the emails found in the **Main CSV** will be included in the merged result.
- **Download the Merged CSV**: The merged CSV file will be available for download after processing.

---

## Requirements

- **Python 3.x**
- **Flask**
- **Pandas**
- **Werkzeug**

To install the required dependencies, create a virtual environment and install the dependencies using `pip`:

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate

# Install the required dependencies
pip install -r requirements.txt
