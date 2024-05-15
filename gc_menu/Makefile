ifeq ($(OS),Windows_NT)
    CURR_DIR_PATH = $(CURDIR)
else
    CURR_DIR_PATH = $(shell pwd)
endif

GCC:=gcc
INC+=-I${CURR_DIR_PATH}/../
SRC+=${CURR_DIR_PATH}/gc_menu.c

INC+=-I${CURR_DIR_PATH}/inc

SRC+=${CURR_DIR_PATH}/menu_test.c
SRC+=${CURR_DIR_PATH}/src/hmi_main.c
SRC+=${CURR_DIR_PATH}/src/hmi_camera.c
SRC+=${CURR_DIR_PATH}/src/hmi_music.c
SRC+=${CURR_DIR_PATH}/src/hmi_set.c
SRC+=${CURR_DIR_PATH}/src/hmi_expand.c
SRC+=${CURR_DIR_PATH}/src/hmi_video.c


AIM_NAME:=menu_demo

.PHONY:all
all:
	${GCC} ${INC} ${SRC} -o ${CURR_DIR_PATH}/${AIM_NAME} -std=c99

.PHONY:clean
clean:
	rm -rf ${CURR_DIR_PATH}/${AIM_NAME}
