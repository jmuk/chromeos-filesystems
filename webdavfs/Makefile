.PHONY: zip clean grunt install

# Name of this file system provider.
NAME=webdavfs

# Name of target ZIP archive.
ZIP=$(NAME).zip

# Compress the extension file into a ZIP archive for distribution or uploading
# to the Chrome Webstore.
zip: grunt
	zip $(ZIP) extension/*

# Builds the extension.
grunt:
	grunt

# Removes any automatically generated files.
clean:
	rm -rf $(ZIP) extension.crx extension/vendor extension/*.js test/build extension/build.*

# Installs build tools.
install:
	npm install
