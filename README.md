# gpt4all_no_qt_build
compiled for dietpi all files from one run after compile and build amd64
steps:

1 apt update && apt upgrade
2 apt install cmake build-essential
3 git clone --recurse-submodules https://github.com/macguyversmusic/gptj-chat
4 mkdir build && cd build
5 cmake ..
6 cmake --build . --parallel
7 cp bin/chat /bin/chat
8 get a model https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin
9 chat -m "ggml-gpt4all-j-v1.3-groovy.bin" -t 4 

10:  chat with gpt4all on DietPI
