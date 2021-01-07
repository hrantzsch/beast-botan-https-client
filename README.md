This repository contains an example of a simple HTTPS client using Boost.Beast and Botan's `tls::stream`.

The client fetches the latest news from https://botan.randombit.net/news.html.

You can easily build and run it using Conan. Replace `g++` with the compiler that is configured in your conan profile.

```
conan install . --build missing
g++ main.cpp -std=c++14 -o simple_client @conanbuildinfo.args
./simple_client
```
