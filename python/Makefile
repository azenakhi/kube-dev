build:
	docker build -t pydev . --build-arg https_proxy=http://X.X.X.X:3128
dev:
	docker run --rm -it -v `pwd`:/app -p 82:5000 -w /app pydev sh -c 'python app.py'