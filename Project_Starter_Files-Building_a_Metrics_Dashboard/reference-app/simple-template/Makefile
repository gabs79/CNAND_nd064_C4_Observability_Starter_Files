include ../Makefile.defs

IMAGE_NAME := simple-template
DEPLOYMENT := /invalid
PORT := 8085

.PHONY: run
run: build
	docker rm -f ${IMAGE_NAME}
	docker run --rm -d --name ${IMAGE_NAME} -p ${PORT}:${PORT} ${IMAGE_NAME}:${TAG} ${run-arg}