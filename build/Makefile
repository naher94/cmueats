# @file Makefile
# @brief Builds the single JS file for deployment.
# 
# Yeah yeah I should use Gulp, but it's literally one file so. . . yeah.
#
# @author Oscar Bezi (oscar@bezi.io)
#===============================================================================

../index.min.js: index-src.js
	babel index-src.js -o index-babel.js
	uglifyjs --compress --mangle -o ../index.min.js -- index-babel.js

clean:
	rm index-babel.js
