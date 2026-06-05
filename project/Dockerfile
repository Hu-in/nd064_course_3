# 1. Use Python 3.8 base image
FROM python:3.10-slim

# 2. Set working directory
WORKDIR /app
RUN apt-get update && apt-get install -y gcc
# 3. Copy project files
COPY . .

# 4. Install dependencies

RUN pip install --upgrade pip
RUN pip install flask


# 5. Expose application port
EXPOSE 3111

# 6. Initialize database + start the app
CMD ["sh", "-c", "python techtrends/init_db.py && python techtrends/app.py"]
