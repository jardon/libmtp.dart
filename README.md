Dart FFI Bindings for libmtp

This project provides Dart FFI (Foreign Function Interface) bindings for the libmtp C library, allowing Dart and Flutter applications to directly interact with media devices and runtimes on Linux.

Prerequisites

C Development Tools: You must have a C compiler and development headers installed (gcc, pkg-config, etc.).

libmtp: The libmtp-dev or equivalent package must be installed on your development system.

Dart SDK: A recent version of the Dart SDK is required.

## Setup

1. Update `pubspec.yaml`

Add the necessary dependencies to your project's pubspec.yaml file:

```yaml
dependencies:
  ffi: ^2.1.0
dev_dependencies:
  ffigen: ^10.0.0
```

Then run dart pub get.

2. Generate Bindings (ffigen)

```bash
dart run ffigen --config ffigen.yaml
```

This will generate the required `libmtp.dart` file.
