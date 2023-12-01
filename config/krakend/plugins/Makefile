# build commands
b000:
	cd krakend-client-example_000 && \
	docker run -it -v "$PWD:/app" -w /app \
	krakend/builder:2.5.0 \
	go build -buildmode=plugin -o krakend-client-example.so . && \
	cd ..

b001:
	cd krakend-server-example_001 && \
	docker run -it -v "$PWD:/app" -w /app \
	krakend/builder:2.5.0 \
	go build -buildmode=plugin -o krakend-server-example.so . && \
	cd ..

bAll:
	make b000 && \
	make b001
