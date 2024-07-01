FROM python:3.9.19-slim 
WORKDIR /app 

# requirements.txt is copied to the working dir 
COPY requirements.txt .

# installing
RUN pip install --no-cache-dir -r requirements.txt 

# entire content of flask app to working dir
COPY . . 

EXPOSE 5000 

# final running command
CMD ["python", "app.py"]