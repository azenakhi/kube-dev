build:
	docker build -t pydev . --build-arg https_proxy=http://X.X.X.X:XX  --build-arg http_proxy=http://X.X.X.X:XX
dev:
	docker run --rm -it -v `pwd`:/app -p 82:5000 -w /app pydev sh -c 'python app.py'