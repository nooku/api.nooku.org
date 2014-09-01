# api.nooku.org

## Installation & Usage

If you haven't already, install ApiGen by downloading the latest release from [the official download section](https://github.com/apigen/apigen/downloads).
Example:

```shell
# Clone this repository
git clone https://github.com/nooku/api.nooku.org.git
cd api.nooku.org
# Download the installation package
curl -o ApiGen-2.8.0.zip https://github.com/downloads/apigen/apigen/ApiGen-2.8.0-standalone.zip
# Unzip the archive
unzip ApiGen-2.8.0.zip
# Make the script writable
chmod +x apigen/apigen.php
# Clean-up
rm ApiGen-2.8.0.zip
```

Now build the documentation using the following command: 

```shell
php -d memory_limit=512M apigen/apigen.php -d ./output --config ~/Projects/nooku/nooku-framework/apigen.neon --template-config=./apigen/templates/nooku/config.neon
```

Make sure to replace the path to `nooku-framework` with the correct path on your machine.


## Deployment

```rake deploy ```

Assuming you already have the [rake](https://rubygems.org/gems/rake) installed.
