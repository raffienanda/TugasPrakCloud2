# Menggunakan base image Python yang ringan
FROM python:3.9-slim

# Menentukan direktori kerja di dalam container
WORKDIR /app

# Menyalin file requirements dan menginstall library
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Menyalin file utama aplikasi
COPY app.py .

# Membuka port 5000 (sesuai port Flask)
EXPOSE 5000

# Perintah untuk menjalankan aplikasi
CMD ["python", "app.py"]