.PHONY: configs

all: configs

configs:
	cd configs/cloud && spruce merge ${HOME}/ops/configs/templates/cloud.yml | spruce json | ${HOME}/ops/cc-me/cc-me

