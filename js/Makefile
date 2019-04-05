build:
	docker build -t jsdev . --build-arg https_proxy=http://X.X.X.X:3128
dev:
	docker run --rm -it -v `pwd`:/app -p 81:3000 -w /app jsdev sh -c 'npx nodemon app.py'