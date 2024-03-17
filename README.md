# eas-cli

sudo npm install -g eas-cli

# eas build

eas build --platform android

# Bundle aab

java -jar bundletool-all-1.15.6.jar build-apks --bundle=app.aab --output=my_job_app.apks --mode=universal --ks=<file-path>/my-upload-key.keystore --ks-key-alias=my-key-alias

# Generate Keystore

keytool -genkeypair -v -storetype PKCS12 -keystore my-upload-key.keystore -alias my-key-alias -keyalg RSA -keysize 2048 -validity 10000
