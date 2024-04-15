## Build

```bash
cd ~/omniverse/kit-app-template
./build.sh
```

## Run as Desktop App

```bash
cd ~/omniverse/kit-app-template

./_build/linux-x86_64/release/my_company.my_app.sh
```

## Run as Headless App

```bash
cd ~/omniverse/kit-app-template/_build/linux-x86_64/release

./kit/kit ./apps/my_company.my_app.kit \
   --no-window \
   --allow-root \
   --/app/livestream/logLevel=debug
```
