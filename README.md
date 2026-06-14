# HTTPServer_Library
A high-performance, cross-platform C++ networking library with multi-threaded TCP/HTTP server support, epoll-based I/O multiplexing, and concurrent connection handling for thousands of simultaneous clients. 

# Steps to build

1) clone the project git clone <url_of_repository>

2) go to HTTPServer_Library directory

3) create a build directory

    mkdir build

4) go to build directory and execute the below command to generate the build system

    cmake ..

5) build the project using the below command

    cmake --build .

6) copy the following html files into debug directory

 /example/public/index.html 
 /example/public/tictactoe.html

7) generate certificate.pem and private_key.pem and place it in the build directory

    openssl genrsa -out private_key.pem 2048
    openssl req -new -x509 -key private_key.pem -out certificate.pem -days 365

8) execute the ./debug/httpserverdemo executable

    

