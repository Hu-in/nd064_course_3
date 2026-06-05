# 1. Use Python 3.8 base image
FROM python:3.10-slim

# 2. Set working directory
WORKDIR /app

# 3. Copy project files
COPY . .

# 4. Install dependencies


RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r techtrends/requirements.txt


# 5. Expose application port
EXPOSE 3111

# 6. Initialize database + start the app
CMD ["sh", "-c", "python project/techtrends/init_db.py && python project/techtrends/app.py --host=0.0.0.0"]
