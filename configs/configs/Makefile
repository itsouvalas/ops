.PHONY: configs proto mgmt

all: configs

configs:
	cd configs/cloud && spruce merge ${HOME}/ops/configs/templates/cloud.yml | spruce json | ${HOME}/ops/cc-me/cc-me

proto: mgmt

mgmt:
	gb b proto update-config --type=cloud --name=lab-proto ${HOME}/ops/configs/configs/cloud/lab.yml

