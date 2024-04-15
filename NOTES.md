## Build

```bash
cd ~/omniverse/kit-app-template
./build.sh
```

## Run App

```bash
cd ~/omniverse/kit-app-template
./_build/linux-x86_64/release/my_company.my_app.sh
```

-   user.config.json path

```bash
ls ~/.local/share/ov/data/Kit/my_company.my_app/2023.0/user.config.json
```

## Run headless

```bash

cd ~/omniverse/kit-app-template/_build/linux-x86_64/release

./kit/kit ./apps/my_company.my_app.kit \
   --enable omni.services.streaming.manager \
   --enable omni.kit.livestream.native \
   --no-window \
   --allow-root

./kit/kit ./apps/my_company.my_app.kit \
   --enable omni.services.streaming.manager \
   --enable omni.kit.livestream.native \
   --enable omni.kit.streamsdk.plugins \
   --no-window \
   --allow-root \
   --/app/livestream/logLevel=debug

./kit/kit ./apps/omni.isaac.sim.headless.native.kit \
   --no-window \
   --allow-root \
   --/app/livestream/logLevel=debug


```

## OK

```bash
cd ~/omniverse/kit-app-template/_build/linux-x86_64/release

./kit/kit ./apps/my_company.my_app.kit \
   --enable omni.services.streaming.manager \
   --enable omni.kit.livestream.native \
   --no-window
```

## How to create extension template

```bash
cd ~/omniverse/kit-app-template
./repo.sh template new
```
