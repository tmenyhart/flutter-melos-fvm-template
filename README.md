# Project workspace

Workspace for the project apps and related packages.

## General

- Workspace is managed by [Melos](https://melos.invertase.dev/)

- Flutter version is managed by [FVM](https://fvm.app/).

- Preferred code editor is [Visual Studio Code](https://code.visualstudio.com/)

- All applications should be created under the `app` directory.

- All packages should be created under the `package` directory.

- For available scripts, see the [melos.yaml](melos.yaml) file.

## Getting started

Install specified Flutter version
```sh
fvm use
fvm flutter doctor
```

Update used Flutter version
```sh
fvm use x.y.z
fvm flutter doctor
```

Get workspace dependencies
```sh
dart pub get
```

## Creating apps and packages

Creating a Flutter app
```sh
cd app/
fvm flutter create --template=app example_app
cd ..
melos bootstrap
```

Creating a Flutter package
```sh
cd package/
fvm flutter create --template=package example_package
cd ..
melos bootstrap
```

