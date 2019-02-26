DIST_DIRECTORY = ../static
BOOTSTRAP_LESS = ./less/bootstrap.less
BOOTSTRAP_RESPONSIVE_LESS = ./less/responsive.less
DATE=$(shell date +%I:%M%p)
CHECK=\033[32m✔\033[39m
HR=\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#

build:
	@echo "\n${HR}"
	@echo "Building Bootstrap..."
	@echo "${HR}\n"
	mkdir -p ${DIST_DIRECTORY}/img
	mkdir -p ${DIST_DIRECTORY}/css
	mkdir -p ${DIST_DIRECTORY}/js
	cp img/* ${DIST_DIRECTORY}/img/
	./node_modules/.bin/recess --compile ${BOOTSTRAP_LESS} > ${DIST_DIRECTORY}/css/bootstrap.css
	./node_modules/.bin/recess --compile ${BOOTSTRAP_RESPONSIVE_LESS} > ${DIST_DIRECTORY}/css/bootstrap-responsive.css
	@echo "Compiling LESS with Recess...               ${CHECK} Done"