# libyuv-cmake
CMakeLists for libyuv

### Windows
default

### Unix
default

### Android
`cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_TOOLCHAIN_FILE=${ANDROID_NDK}/build/cmake/android.toolchain.cmake -DANDROID_ABI=arm64-v8a -DANDROID_STL=c++_shared -DANDROID_PLATFORM=android-22 -S ${PROJECT_DIR} -B ${BUILD_OUT_PATH}`

### Cmake Options
* `BUILD_TOOLS` build yuvconvert program; default OFF
* `BUILD_STATIC` build static lib; default ON
* `WITH_JPEG` build with jpeg; default OFF
* `ENABLE_TEST` built unit tests; default OFF
