# 🔐 PDF Cracker Web App

A sleek, automated Flask web application that extracts password hashes from encrypted PDF files and attempts to crack them using a wordlist. Designed for security demos, educational use, or internship showcases, this tool combines modern UI sensibility with backend automation.

---

## 🚀 Features

- Upload encrypted PDF files via a web interface
- Extract password hashes using `pdf2john`
- Crack passwords using `John the Ripper` and a wordlist
- Supports custom wordlist uploads or defaults to `rockyou.txt`
- Displays encryption type (AES/RC4) and revision
- Logs results to a SQLite database
- Responsive UI with error handling and feedback

---

## 🧰 Technologies Used

Component

Purpose

Flask

Web framework for routing and rendering

pyhanko

PDF parsing and cryptographic handling

pdf2john

Hash extraction from encrypted PDFs

John the Ripper

Password cracking engine

SQLite

Logging cracked attempts

HTML/CSS

Frontend interface

⚙️ Setup Instructions

🧰 1. Run setup.py to Prepare the Environment

Open your terminal and navigate to the project folder:

cd ~/Desktop/pdf_cracker_web

Run the setup script:

python3 setup.py

This script will:

Detect your OS

Create a virtual environment (venv/)

Download rockyou.txt wordlist

Install required Python packages (flask, pyhanko)

Check if John the Ripper is installed

Launch the app using the virtual environment

🧪 2. Manual Virtual Environment Activation (Optional)

If you want to run things manually:

source venv/bin/activate

Then install dependencies:

pip install flask pyhanko==0.20.1

🖥️ 3. Run the App

Once the environment is ready:

python app.py

Or use the virtual environment directly:

./venv/bin/python app.py

🌐 4. Access the Web Interface

Open your browser and go to:

http://127.0.0.1:5000

You’ll see the upload form where you can:

Upload a password-protected PDF

Optionally upload a custom wordlist

View extracted hash, encryption type, cracking results, and error messages

🧼 5. Stopping the App

To stop the server, press:

CTRL + C

📌 Notes

This app is for educational and ethical use only.

Do not use on unauthorized or private documents.

For production deployment, use a WSGI server like Gunicorn.

📄 License

MIT License © 2025 Bhagya

 ---  Let me know if you want me to generate a matching `requirements.txt`, add screenshots, or prep a GitHub release draft. You're ready to showcase this like a pro!
