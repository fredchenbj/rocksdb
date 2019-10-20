### compile and run on mac
- use clang on mac
`c++ -std=c++11 simple_test.cc -o test -lpthread -lrocksdb -L../build -I../include`

- link dylib on mac
`install_name_tool -change @rpath/librocksdb.6.dylib /Users/admin/workspace/src/github.com/pingcap/rocksdb/build/librocksdb.6.dylib ./test`