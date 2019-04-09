build:
	docker build -t jsdev . --build-arg https_proxy=${proxy} --build-arg http_proxy=${proxy}
dev:
	docker run --rm -it -v `pwd`:/app -p 81:3000 -w /app jsdev sh -c 'npx nodemon app.js'