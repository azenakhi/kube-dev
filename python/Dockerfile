FROM python:alpine as build
WORKDIR /app
COPY requirements.txt ./
RUN pip install -r requirements.txt

FROM python:alpine
WORKDIR /app
COPY --from=build /app/requirements.txt ./
COPY --from=build /root/.cache /root/.cache
RUN pip install -r requirements.txt
COPY . .
CMD ["python", "app.py"]