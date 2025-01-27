Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
python -m venv myenv
myenv\Scripts\activate
pip install -r requirements.txt
cd app
uvicorn main:app --reload
