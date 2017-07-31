

# Installation on 31 July 2017 @ map479@map479-DQ57T


```
$ mkdir build && cd build && cmake WITH_JPEG=OFF ..
-- The C compiler identification is GNU 5.4.0
-- The CXX compiler identification is GNU 5.4.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- C++11 activated.
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Looking for pthread_create
-- Looking for pthread_create - not found
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Looking for XOpenDisplay in /usr/lib/x86_64-linux-gnu/libX11.so;/usr/lib/x86_64-linux-gnu/libXext.so
-- Looking for XOpenDisplay in /usr/lib/x86_64-linux-gnu/libX11.so;/usr/lib/x86_64-linux-gnu/libXext.so - found
-- Looking for gethostbyname
-- Looking for gethostbyname - found
-- Looking for connect
-- Looking for connect - found
-- Looking for remove
-- Looking for remove - found
-- Looking for shmat
-- Looking for shmat - found
-- Looking for IceConnectionNumber in ICE
-- Looking for IceConnectionNumber in ICE - found
-- Found X11: /usr/lib/x86_64-linux-gnu/libX11.so
-- Looking for png_create_read_struct
-- Looking for png_create_read_struct - found
-- Looking for jpeg_read_header
-- Looking for jpeg_read_header - found
-- Searching for BLAS and LAPACK
-- Found PkgConfig: /usr/bin/pkg-config (found version "0.29.1")
-- Checking for module 'cblas'
--   No package 'cblas' found
-- Checking for module 'lapack'
--   Found lapack, version 3.10.2
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of void*
-- Check size of void* - done
-- Found LAPACK library
-- Found ATLAS BLAS library
-- Looking for cblas_ddot
-- Looking for cblas_ddot - found
CUDA_TOOLKIT_ROOT_DIR not found or specified
-- Could NOT find CUDA (missing:  CUDA_TOOLKIT_ROOT_DIR CUDA_NVCC_EXECUTABLE CUDA_INCLUDE_DIRS CUDA_CUDART_LIBRARY) (Required is at least version "7.5")
-- *** cuDNN V5.0 OR GREATER NOT FOUND.  DLIB WILL NOT USE CUDA. ***
-- *** If you have cuDNN then set CMAKE_PREFIX_PATH to include cuDNN's folder.
-- Configuring done
-- Generating done
-- Build files have been written to: /home/map479/dlib/build


```




```
$ sudo cmake --build . --target install
Scanning dependencies of target dlib
[  0%] Building CXX object dlib/CMakeFiles/dlib.dir/base64/base64_kernel_1.cpp.o
[  1%] Building CXX object dlib/CMakeFiles/dlib.dir/bigint/bigint_kernel_1.cpp.o
[  2%] Building CXX object dlib/CMakeFiles/dlib.dir/bigint/bigint_kernel_2.cpp.o
[  3%] Building CXX object dlib/CMakeFiles/dlib.dir/bit_stream/bit_stream_kernel_1.cpp.o
[  4%] Building CXX object dlib/CMakeFiles/dlib.dir/entropy_decoder/entropy_decoder_kernel_1.cpp.o
[  5%] Building CXX object dlib/CMakeFiles/dlib.dir/entropy_decoder/entropy_decoder_kernel_2.cpp.o
[  6%] Building CXX object dlib/CMakeFiles/dlib.dir/entropy_encoder/entropy_encoder_kernel_1.cpp.o
[  7%] Building CXX object dlib/CMakeFiles/dlib.dir/entropy_encoder/entropy_encoder_kernel_2.cpp.o
[  8%] Building CXX object dlib/CMakeFiles/dlib.dir/md5/md5_kernel_1.cpp.o
[  9%] Building CXX object dlib/CMakeFiles/dlib.dir/tokenizer/tokenizer_kernel_1.cpp.o
[ 10%] Building CXX object dlib/CMakeFiles/dlib.dir/unicode/unicode.cpp.o
[ 10%] Building CXX object dlib/CMakeFiles/dlib.dir/data_io/image_dataset_metadata.cpp.o
[ 11%] Building CXX object dlib/CMakeFiles/dlib.dir/data_io/mnist.cpp.o
[ 12%] Building CXX object dlib/CMakeFiles/dlib.dir/dnn/cpu_dlib.cpp.o
[ 13%] Building CXX object dlib/CMakeFiles/dlib.dir/dnn/tensor_tools.cpp.o
[ 14%] Building CXX object dlib/CMakeFiles/dlib.dir/sockets/sockets_kernel_1.cpp.o
[ 15%] Building CXX object dlib/CMakeFiles/dlib.dir/bsp/bsp.cpp.o
[ 16%] Building CXX object dlib/CMakeFiles/dlib.dir/dir_nav/dir_nav_kernel_1.cpp.o
[ 17%] Building CXX object dlib/CMakeFiles/dlib.dir/dir_nav/dir_nav_kernel_2.cpp.o
[ 18%] Building CXX object dlib/CMakeFiles/dlib.dir/dir_nav/dir_nav_extensions.cpp.o
[ 19%] Building CXX object dlib/CMakeFiles/dlib.dir/linker/linker_kernel_1.cpp.o
[ 20%] Building CXX object dlib/CMakeFiles/dlib.dir/logger/extra_logger_headers.cpp.o
[ 20%] Building CXX object dlib/CMakeFiles/dlib.dir/logger/logger_kernel_1.cpp.o
[ 21%] Building CXX object dlib/CMakeFiles/dlib.dir/logger/logger_config_file.cpp.o
[ 22%] Building CXX object dlib/CMakeFiles/dlib.dir/misc_api/misc_api_kernel_1.cpp.o
[ 23%] Building CXX object dlib/CMakeFiles/dlib.dir/misc_api/misc_api_kernel_2.cpp.o
[ 24%] Building CXX object dlib/CMakeFiles/dlib.dir/sockets/sockets_extensions.cpp.o
[ 25%] Building CXX object dlib/CMakeFiles/dlib.dir/sockets/sockets_kernel_2.cpp.o
[ 26%] Building CXX object dlib/CMakeFiles/dlib.dir/sockstreambuf/sockstreambuf.cpp.o
[ 27%] Building CXX object dlib/CMakeFiles/dlib.dir/sockstreambuf/sockstreambuf_unbuffered.cpp.o
[ 28%] Building CXX object dlib/CMakeFiles/dlib.dir/server/server_kernel.cpp.o
[ 29%] Building CXX object dlib/CMakeFiles/dlib.dir/server/server_iostream.cpp.o
[ 30%] Building CXX object dlib/CMakeFiles/dlib.dir/server/server_http.cpp.o
[ 30%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/multithreaded_object_extension.cpp.o
[ 31%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/threaded_object_extension.cpp.o
[ 32%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/threads_kernel_1.cpp.o
[ 33%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/threads_kernel_2.cpp.o
[ 34%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/threads_kernel_shared.cpp.o
[ 35%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/thread_pool_extension.cpp.o
[ 36%] Building CXX object dlib/CMakeFiles/dlib.dir/threads/async.cpp.o
[ 37%] Building CXX object dlib/CMakeFiles/dlib.dir/timer/timer.cpp.o
[ 38%] Building CXX object dlib/CMakeFiles/dlib.dir/stack_trace.cpp.o
[ 39%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/fonts.cpp.o
[ 40%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/widgets.cpp.o
[ 40%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/drawable.cpp.o
[ 41%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/canvas_drawing.cpp.o
[ 42%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/style.cpp.o
[ 43%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_widgets/base_widgets.cpp.o
[ 44%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_core/gui_core_kernel_1.cpp.o
[ 45%] Building CXX object dlib/CMakeFiles/dlib.dir/gui_core/gui_core_kernel_2.cpp.o
[ 46%] Building CXX object dlib/CMakeFiles/dlib.dir/image_loader/png_loader.cpp.o
[ 47%] Building CXX object dlib/CMakeFiles/dlib.dir/image_saver/save_png.cpp.o
[ 48%] Building CXX object dlib/CMakeFiles/dlib.dir/image_loader/jpeg_loader.cpp.o
[ 49%] Building CXX object dlib/CMakeFiles/dlib.dir/image_saver/save_jpeg.cpp.o
[ 50%] Linking CXX static library libdlib.a
[ 50%] Built target dlib
Scanning dependencies of target dlib_shared
[ 50%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/base64/base64_kernel_1.cpp.o
[ 51%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/bigint/bigint_kernel_1.cpp.o
[ 52%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/bigint/bigint_kernel_2.cpp.o
[ 53%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/bit_stream/bit_stream_kernel_1.cpp.o
[ 54%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/entropy_decoder/entropy_decoder_kernel_1.cpp.o
[ 55%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/entropy_decoder/entropy_decoder_kernel_2.cpp.o
[ 56%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/entropy_encoder/entropy_encoder_kernel_1.cpp.o
[ 57%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/entropy_encoder/entropy_encoder_kernel_2.cpp.o
[ 58%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/md5/md5_kernel_1.cpp.o
[ 59%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/tokenizer/tokenizer_kernel_1.cpp.o
[ 60%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/unicode/unicode.cpp.o
[ 60%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/data_io/image_dataset_metadata.cpp.o
[ 61%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/data_io/mnist.cpp.o
[ 62%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/dnn/cpu_dlib.cpp.o
[ 63%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/dnn/tensor_tools.cpp.o
[ 64%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/sockets/sockets_kernel_1.cpp.o
[ 65%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/bsp/bsp.cpp.o
[ 66%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/dir_nav/dir_nav_kernel_1.cpp.o
[ 67%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/dir_nav/dir_nav_kernel_2.cpp.o
[ 68%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/dir_nav/dir_nav_extensions.cpp.o
[ 69%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/linker/linker_kernel_1.cpp.o
[ 70%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/logger/extra_logger_headers.cpp.o
[ 70%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/logger/logger_kernel_1.cpp.o
[ 71%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/logger/logger_config_file.cpp.o
[ 72%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/misc_api/misc_api_kernel_1.cpp.o
[ 73%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/misc_api/misc_api_kernel_2.cpp.o
[ 74%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/sockets/sockets_extensions.cpp.o
[ 75%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/sockets/sockets_kernel_2.cpp.o
[ 76%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/sockstreambuf/sockstreambuf.cpp.o
[ 77%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/sockstreambuf/sockstreambuf_unbuffered.cpp.o
[ 78%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/server/server_kernel.cpp.o
[ 79%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/server/server_iostream.cpp.o
[ 80%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/server/server_http.cpp.o
[ 80%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/multithreaded_object_extension.cpp.o
[ 81%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/threaded_object_extension.cpp.o
[ 82%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/threads_kernel_1.cpp.o
[ 83%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/threads_kernel_2.cpp.o
[ 84%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/threads_kernel_shared.cpp.o
[ 85%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/thread_pool_extension.cpp.o
[ 86%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/threads/async.cpp.o
[ 87%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/timer/timer.cpp.o
[ 88%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/stack_trace.cpp.o
[ 89%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/fonts.cpp.o
[ 90%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/widgets.cpp.o
[ 90%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/drawable.cpp.o
[ 91%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/canvas_drawing.cpp.o
[ 92%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/style.cpp.o
[ 93%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_widgets/base_widgets.cpp.o
[ 94%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_core/gui_core_kernel_1.cpp.o
[ 95%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/gui_core/gui_core_kernel_2.cpp.o
[ 96%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/image_loader/png_loader.cpp.o
[ 97%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/image_saver/save_png.cpp.o
[ 98%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/image_loader/jpeg_loader.cpp.o
[ 99%] Building CXX object dlib/CMakeFiles/dlib_shared.dir/image_saver/save_jpeg.cpp.o
[100%] Linking CXX shared library libdlib.so
[100%] Built target dlib_shared
Install the project...
-- Install configuration: "Release"
-- Installing: /usr/local/lib/libdlib.a
-- Installing: /usr/local/lib/libdlib.so.19.4.99
-- Installing: /usr/local/lib/libdlib.so
-- Installing: /usr/local/include/dlib
-- Installing: /usr/local/include/dlib/bit_stream.h
-- Installing: /usr/local/include/dlib/graph_utils.h
-- Installing: /usr/local/include/dlib/lzp_buffer
-- Installing: /usr/local/include/dlib/lzp_buffer/lzp_buffer_kernel_1.h
-- Installing: /usr/local/include/dlib/lzp_buffer/lzp_buffer_kernel_2.h
-- Installing: /usr/local/include/dlib/lzp_buffer/lzp_buffer_kernel_c.h
-- Installing: /usr/local/include/dlib/lzp_buffer/lzp_buffer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/any.h
-- Installing: /usr/local/include/dlib/any
-- Installing: /usr/local/include/dlib/any/any.h
-- Installing: /usr/local/include/dlib/any/any_function_abstract.h
-- Installing: /usr/local/include/dlib/any/any_abstract.h
-- Installing: /usr/local/include/dlib/any/any_trainer.h
-- Installing: /usr/local/include/dlib/any/any_decision_function.h
-- Installing: /usr/local/include/dlib/any/any_function_impl2.h
-- Installing: /usr/local/include/dlib/any/any_function.h
-- Installing: /usr/local/include/dlib/any/any_function_impl.h
-- Installing: /usr/local/include/dlib/any/any_trainer_abstract.h
-- Installing: /usr/local/include/dlib/any/any_decision_function_abstract.h
-- Installing: /usr/local/include/dlib/algs.h
-- Installing: /usr/local/include/dlib/sequence
-- Installing: /usr/local/include/dlib/sequence/sequence_compare_abstract.h
-- Installing: /usr/local/include/dlib/sequence/sequence_kernel_c.h
-- Installing: /usr/local/include/dlib/sequence/sequence_kernel_abstract.h
-- Installing: /usr/local/include/dlib/sequence/sequence_compare_1.h
-- Installing: /usr/local/include/dlib/sequence/sequence_sort_abstract.h
-- Installing: /usr/local/include/dlib/sequence/sequence_kernel_1.h
-- Installing: /usr/local/include/dlib/sequence/sequence_sort_2.h
-- Installing: /usr/local/include/dlib/sequence/sequence_sort_1.h
-- Installing: /usr/local/include/dlib/sequence/sequence_kernel_2.h
-- Installing: /usr/local/include/dlib/member_function_pointer.h
-- Installing: /usr/local/include/dlib/md5.h
-- Installing: /usr/local/include/dlib/stack_trace.h
-- Installing: /usr/local/include/dlib/graph_cuts.h
-- Installing: /usr/local/include/dlib/pipe
-- Installing: /usr/local/include/dlib/pipe/pipe_kernel_abstract.h
-- Installing: /usr/local/include/dlib/pipe/pipe_kernel_1.h
-- Installing: /usr/local/include/dlib/string
-- Installing: /usr/local/include/dlib/string/string_abstract.h
-- Installing: /usr/local/include/dlib/string/string.h
-- Installing: /usr/local/include/dlib/pipe.h
-- Installing: /usr/local/include/dlib/std_allocator.h
-- Installing: /usr/local/include/dlib/cmake_utils
-- Installing: /usr/local/include/dlib/cmake_utils/test_for_cudnn
-- Installing: /usr/local/include/dlib/cmake_utils/test_for_neon
-- Installing: /usr/local/include/dlib/cmake_utils/test_for_cuda
-- Installing: /usr/local/include/dlib/cmake_utils/use_cpp_11.cmake
-- Installing: /usr/local/include/dlib/cmake_utils/test_for_cpp11
-- Installing: /usr/local/include/dlib/cmake_utils/check_if_neon_available.cmake
-- Installing: /usr/local/include/dlib/cmake_utils/tell_visual_studio_to_use_static_runtime.cmake
-- Installing: /usr/local/include/dlib/cmake_utils/add_global_compiler_switch.cmake
-- Installing: /usr/local/include/dlib/opencv.h
-- Installing: /usr/local/include/dlib/base64
-- Installing: /usr/local/include/dlib/base64/base64_kernel_abstract.h
-- Installing: /usr/local/include/dlib/base64/base64_kernel_1.h
-- Installing: /usr/local/include/dlib/memory_manager_stateless.h
-- Installing: /usr/local/include/dlib/entropy_encoder.h
-- Installing: /usr/local/include/dlib/svm.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_abstract.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_3.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_1.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_5.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_2.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_6.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model/entropy_decoder_model_kernel_4.h
-- Installing: /usr/local/include/dlib/set_utils.h
-- Installing: /usr/local/include/dlib/stack.h
-- Installing: /usr/local/include/dlib/lz77_buffer.h
-- Installing: /usr/local/include/dlib/filtering
-- Installing: /usr/local/include/dlib/filtering/rls_filter_abstract.h
-- Installing: /usr/local/include/dlib/filtering/rls_filter.h
-- Installing: /usr/local/include/dlib/filtering/kalman_filter_abstract.h
-- Installing: /usr/local/include/dlib/filtering/kalman_filter.h
-- Installing: /usr/local/include/dlib/array.h
-- Installing: /usr/local/include/dlib/svm_threaded.h
-- Installing: /usr/local/include/dlib/conditioning_class
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_3.h
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_c.h
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_4.h
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_1.h
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_2.h
-- Installing: /usr/local/include/dlib/conditioning_class/conditioning_class_kernel_abstract.h
-- Installing: /usr/local/include/dlib/cmd_line_parser
-- Installing: /usr/local/include/dlib/cmd_line_parser/get_option.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_check_1.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_kernel_1.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_kernel_abstract.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_print_1.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_check_c.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/cmd_line_parser_kernel_c.h
-- Installing: /usr/local/include/dlib/cmd_line_parser/get_option_abstract.h
-- Installing: /usr/local/include/dlib/threads.h
-- Installing: /usr/local/include/dlib/server.h
-- Installing: /usr/local/include/dlib/geometry.h
-- Installing: /usr/local/include/dlib/cpp_tokenizer.h
-- Installing: /usr/local/include/dlib/set.h
-- Installing: /usr/local/include/dlib/config_reader
-- Installing: /usr/local/include/dlib/config_reader/config_reader_thread_safe_abstract.h
-- Installing: /usr/local/include/dlib/config_reader/config_reader_kernel_1.h
-- Installing: /usr/local/include/dlib/config_reader/config_reader_kernel_abstract.h
-- Installing: /usr/local/include/dlib/config_reader/config_reader_thread_safe_1.h
-- Installing: /usr/local/include/dlib/general_hash
-- Installing: /usr/local/include/dlib/general_hash/count_bits.h
-- Installing: /usr/local/include/dlib/general_hash/general_hash.h
-- Installing: /usr/local/include/dlib/general_hash/hash_abstract.h
-- Installing: /usr/local/include/dlib/general_hash/hash.h
-- Installing: /usr/local/include/dlib/general_hash/murmur_hash3.h
-- Installing: /usr/local/include/dlib/general_hash/murmur_hash3_abstract.h
-- Installing: /usr/local/include/dlib/general_hash/count_bits_abstract.h
-- Installing: /usr/local/include/dlib/general_hash/random_hashing.h
-- Installing: /usr/local/include/dlib/general_hash/random_hashing_abstract.h
-- Installing: /usr/local/include/dlib/binary_search_tree
-- Installing: /usr/local/include/dlib/binary_search_tree/binary_search_tree_kernel_2.h
-- Installing: /usr/local/include/dlib/binary_search_tree/binary_search_tree_kernel_1.h
-- Installing: /usr/local/include/dlib/binary_search_tree/binary_search_tree_kernel_c.h
-- Installing: /usr/local/include/dlib/binary_search_tree/binary_search_tree_kernel_abstract.h
-- Installing: /usr/local/include/dlib/md5
-- Installing: /usr/local/include/dlib/md5/md5_kernel_abstract.h
-- Installing: /usr/local/include/dlib/md5/md5_kernel_1.h
-- Installing: /usr/local/include/dlib/image_processing.h
-- Installing: /usr/local/include/dlib/optimization.h
-- Installing: /usr/local/include/dlib/tokenizer
-- Installing: /usr/local/include/dlib/tokenizer/tokenizer_kernel_1.h
-- Installing: /usr/local/include/dlib/tokenizer/tokenizer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/tokenizer/tokenizer_kernel_c.h
-- Installing: /usr/local/include/dlib/linker
-- Installing: /usr/local/include/dlib/linker/linker_kernel_abstract.h
-- Installing: /usr/local/include/dlib/linker/linker_kernel_1.h
-- Installing: /usr/local/include/dlib/data_io
-- Installing: /usr/local/include/dlib/data_io/libsvm_io.h
-- Installing: /usr/local/include/dlib/data_io/load_image_dataset.h
-- Installing: /usr/local/include/dlib/data_io/mnist.h
-- Installing: /usr/local/include/dlib/data_io/libsvm_io_abstract.h
-- Installing: /usr/local/include/dlib/data_io/load_image_dataset_abstract.h
-- Installing: /usr/local/include/dlib/data_io/image_dataset_metadata.h
-- Installing: /usr/local/include/dlib/data_io/mnist_abstract.h
-- Installing: /usr/local/include/dlib/rand.h
-- Installing: /usr/local/include/dlib/python.h
-- Installing: /usr/local/include/dlib/ref.h
-- Installing: /usr/local/include/dlib/hash.h
-- Installing: /usr/local/include/dlib/misc_api
-- Installing: /usr/local/include/dlib/misc_api/misc_api_kernel_abstract.h
-- Installing: /usr/local/include/dlib/misc_api/posix.h
-- Installing: /usr/local/include/dlib/misc_api/misc_api_kernel_2.h
-- Installing: /usr/local/include/dlib/misc_api/windows.h
-- Installing: /usr/local/include/dlib/misc_api/misc_api_kernel_1.h
-- Installing: /usr/local/include/dlib/misc_api/misc_api_shared.h
-- Installing: /usr/local/include/dlib/lzp_buffer.h
-- Installing: /usr/local/include/dlib/disjoint_subsets
-- Installing: /usr/local/include/dlib/disjoint_subsets/disjoint_subsets.h
-- Installing: /usr/local/include/dlib/disjoint_subsets/disjoint_subsets_abstract.h
-- Installing: /usr/local/include/dlib/sync_extension.h
-- Installing: /usr/local/include/dlib/manifold_regularization
-- Installing: /usr/local/include/dlib/manifold_regularization/linear_manifold_regularizer_abstract.h
-- Installing: /usr/local/include/dlib/manifold_regularization/linear_manifold_regularizer.h
-- Installing: /usr/local/include/dlib/xml_parser
-- Installing: /usr/local/include/dlib/xml_parser/xml_parser_kernel_interfaces.h
-- Installing: /usr/local/include/dlib/xml_parser/xml_parser_kernel_abstract.h
-- Installing: /usr/local/include/dlib/xml_parser/xml_parser_kernel_1.h
-- Installing: /usr/local/include/dlib/byte_orderer.h
-- Installing: /usr/local/include/dlib/threads
-- Installing: /usr/local/include/dlib/threads/auto_unlock_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/rmutex_extension.h
-- Installing: /usr/local/include/dlib/threads/parallel_for_extension.h
-- Installing: /usr/local/include/dlib/threads/thread_function_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/auto_mutex_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/posix.h
-- Installing: /usr/local/include/dlib/threads/threaded_object_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/thread_pool_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/rsignaler_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/threads_kernel.h
-- Installing: /usr/local/include/dlib/threads/threads_kernel_abstract.h
-- Installing: /usr/local/include/dlib/threads/multithreaded_object_extension.h
-- Installing: /usr/local/include/dlib/threads/create_new_thread_extension.h
-- Installing: /usr/local/include/dlib/threads/thread_specific_data_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/rmutex_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/auto_unlock_extension.h
-- Installing: /usr/local/include/dlib/threads/thread_pool_extension.h
-- Installing: /usr/local/include/dlib/threads/thread_specific_data_extension.h
-- Installing: /usr/local/include/dlib/threads/windows.h
-- Installing: /usr/local/include/dlib/threads/parallel_for_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/threads_kernel_shared.h
-- Installing: /usr/local/include/dlib/threads/threads_kernel_1.h
-- Installing: /usr/local/include/dlib/threads/multithreaded_object_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/async.h
-- Installing: /usr/local/include/dlib/threads/threaded_object_extension.h
-- Installing: /usr/local/include/dlib/threads/read_write_mutex_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/thread_function_extension.h
-- Installing: /usr/local/include/dlib/threads/rsignaler_extension.h
-- Installing: /usr/local/include/dlib/threads/create_new_thread_extension_abstract.h
-- Installing: /usr/local/include/dlib/threads/auto_mutex_extension.h
-- Installing: /usr/local/include/dlib/threads/threads_kernel_2.h
-- Installing: /usr/local/include/dlib/threads/read_write_mutex_extension.h
-- Installing: /usr/local/include/dlib/threads/async_abstract.h
-- Installing: /usr/local/include/dlib/tuple
-- Installing: /usr/local/include/dlib/tuple/tuple.h
-- Installing: /usr/local/include/dlib/tuple/tuple_abstract.h
-- Installing: /usr/local/include/dlib/sequence.h
-- Installing: /usr/local/include/dlib/bits
-- Installing: /usr/local/include/dlib/bits/c++config.h
-- Installing: /usr/local/include/dlib/graph_utils_threaded.h
-- Installing: /usr/local/include/dlib/byte_orderer
-- Installing: /usr/local/include/dlib/byte_orderer/byte_orderer_kernel_1.h
-- Installing: /usr/local/include/dlib/byte_orderer/byte_orderer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/graph
-- Installing: /usr/local/include/dlib/graph/graph_kernel_1.h
-- Installing: /usr/local/include/dlib/graph/graph_kernel_abstract.h
-- Installing: /usr/local/include/dlib/queue
-- Installing: /usr/local/include/dlib/queue/queue_sort_abstract.h
-- Installing: /usr/local/include/dlib/queue/queue_kernel_1.h
-- Installing: /usr/local/include/dlib/queue/queue_kernel_abstract.h
-- Installing: /usr/local/include/dlib/queue/queue_kernel_2.h
-- Installing: /usr/local/include/dlib/queue/queue_kernel_c.h
-- Installing: /usr/local/include/dlib/queue/queue_sort_1.h
-- Installing: /usr/local/include/dlib/tuple.h
-- Installing: /usr/local/include/dlib/manifold_regularization.h
-- Installing: /usr/local/include/dlib/statistics.h
-- Installing: /usr/local/include/dlib/sockstreambuf.h
-- Installing: /usr/local/include/dlib/type_safe_union
-- Installing: /usr/local/include/dlib/type_safe_union/type_safe_union_kernel.h
-- Installing: /usr/local/include/dlib/type_safe_union/type_safe_union_kernel_abstract.h
-- Installing: /usr/local/include/dlib/mlp
-- Installing: /usr/local/include/dlib/mlp/mlp_kernel_abstract.h
-- Installing: /usr/local/include/dlib/mlp/mlp_kernel_c.h
-- Installing: /usr/local/include/dlib/mlp/mlp_kernel_1.h
-- Installing: /usr/local/include/dlib/console_progress_indicator.h
-- Installing: /usr/local/include/dlib/http_client
-- Installing: /usr/local/include/dlib/http_client/http_client_abstract.h
-- Installing: /usr/local/include/dlib/http_client/http_client.h
-- Installing: /usr/local/include/dlib/dir_nav
-- Installing: /usr/local/include/dlib/dir_nav/posix.h
-- Installing: /usr/local/include/dlib/dir_nav/dir_nav_extensions_abstract.h
-- Installing: /usr/local/include/dlib/dir_nav/windows.h
-- Installing: /usr/local/include/dlib/dir_nav/dir_nav_extensions.h
-- Installing: /usr/local/include/dlib/dir_nav/dir_nav_kernel_2.h
-- Installing: /usr/local/include/dlib/dir_nav/dir_nav_kernel_abstract.h
-- Installing: /usr/local/include/dlib/dir_nav/dir_nav_kernel_1.h
-- Installing: /usr/local/include/dlib/bigint.h
-- Installing: /usr/local/include/dlib/static_map
-- Installing: /usr/local/include/dlib/static_map/static_map_kernel_abstract.h
-- Installing: /usr/local/include/dlib/static_map/static_map_kernel_1.h
-- Installing: /usr/local/include/dlib/static_map/static_map_kernel_c.h
-- Installing: /usr/local/include/dlib/memory_manager.h
-- Installing: /usr/local/include/dlib/iosockstream
-- Installing: /usr/local/include/dlib/iosockstream/iosockstream_abstract.h
-- Installing: /usr/local/include/dlib/iosockstream/iosockstream.h
-- Installing: /usr/local/include/dlib/numerical_integration
-- Installing: /usr/local/include/dlib/numerical_integration/integrate_function_adapt_simpson.h
-- Installing: /usr/local/include/dlib/numerical_integration/integrate_function_adapt_simpson_abstract.h
-- Installing: /usr/local/include/dlib/lsh
-- Installing: /usr/local/include/dlib/lsh/projection_hash.h
-- Installing: /usr/local/include/dlib/lsh/hashes_abstract.h
-- Installing: /usr/local/include/dlib/lsh/create_random_projection_hash_abstract.h
-- Installing: /usr/local/include/dlib/lsh/hashes.h
-- Installing: /usr/local/include/dlib/lsh/projection_hash_abstract.h
-- Installing: /usr/local/include/dlib/lsh/create_random_projection_hash.h
-- Installing: /usr/local/include/dlib/memory_manager_stateless
-- Installing: /usr/local/include/dlib/memory_manager_stateless/memory_manager_stateless_kernel_2.h
-- Installing: /usr/local/include/dlib/memory_manager_stateless/memory_manager_stateless_kernel_abstract.h
-- Installing: /usr/local/include/dlib/memory_manager_stateless/memory_manager_stateless_kernel_1.h
-- Installing: /usr/local/include/dlib/smart_pointers_thread_safe.h
-- Installing: /usr/local/include/dlib/reference_counter
-- Installing: /usr/local/include/dlib/reference_counter/reference_counter_kernel_abstract.h
-- Installing: /usr/local/include/dlib/reference_counter/reference_counter_kernel_1.h
-- Installing: /usr/local/include/dlib/graph_utils
-- Installing: /usr/local/include/dlib/graph_utils/graph_utils.h
-- Installing: /usr/local/include/dlib/graph_utils/find_k_nearest_neighbors_lsh.h
-- Installing: /usr/local/include/dlib/graph_utils/function_objects.h
-- Installing: /usr/local/include/dlib/graph_utils/sample_pair_abstract.h
-- Installing: /usr/local/include/dlib/graph_utils/sample_pair.h
-- Installing: /usr/local/include/dlib/graph_utils/find_k_nearest_neighbors_lsh_abstract.h
-- Installing: /usr/local/include/dlib/graph_utils/edge_list_graphs.h
-- Installing: /usr/local/include/dlib/graph_utils/ordered_sample_pair.h
-- Installing: /usr/local/include/dlib/graph_utils/ordered_sample_pair_abstract.h
-- Installing: /usr/local/include/dlib/graph_utils/edge_list_graphs_abstract.h
-- Installing: /usr/local/include/dlib/graph_utils/function_objects_abstract.h
-- Installing: /usr/local/include/dlib/graph_utils/graph_utils_abstract.h
-- Installing: /usr/local/include/dlib/map.h
-- Installing: /usr/local/include/dlib/config.h
-- Installing: /usr/local/include/dlib/unicode.h
-- Installing: /usr/local/include/dlib/sockets.h
-- Installing: /usr/local/include/dlib/dnn.h
-- Installing: /usr/local/include/dlib/bound_function_pointer.h
-- Installing: /usr/local/include/dlib/static_set.h
-- Installing: /usr/local/include/dlib/server
-- Installing: /usr/local/include/dlib/server/server_iostream.h
-- Installing: /usr/local/include/dlib/server/server_http_abstract.h
-- Installing: /usr/local/include/dlib/server/server_iostream_abstract.h
-- Installing: /usr/local/include/dlib/server/server_http.h
-- Installing: /usr/local/include/dlib/server/server_kernel.h
-- Installing: /usr/local/include/dlib/server/server_kernel_abstract.h
-- Installing: /usr/local/include/dlib/uintn.h
-- Installing: /usr/local/include/dlib/enable_if.h
-- Installing: /usr/local/include/dlib/sliding_buffer.h
-- Installing: /usr/local/include/dlib/misc_api.h
-- Installing: /usr/local/include/dlib/simd.h
-- Installing: /usr/local/include/dlib/sync_extension
-- Installing: /usr/local/include/dlib/sync_extension/sync_extension_kernel_abstract.h
-- Installing: /usr/local/include/dlib/sync_extension/sync_extension_kernel_1.h
-- Installing: /usr/local/include/dlib/memory_manager_global.h
-- Installing: /usr/local/include/dlib/memory_manager
-- Installing: /usr/local/include/dlib/memory_manager/memory_manager_kernel_2.h
-- Installing: /usr/local/include/dlib/memory_manager/memory_manager_kernel_1.h
-- Installing: /usr/local/include/dlib/memory_manager/memory_manager_kernel_3.h
-- Installing: /usr/local/include/dlib/memory_manager/memory_manager_kernel_abstract.h
-- Installing: /usr/local/include/dlib/binary_search_tree.h
-- Installing: /usr/local/include/dlib/simd
-- Installing: /usr/local/include/dlib/simd/simd_check.h
-- Installing: /usr/local/include/dlib/simd/simd4f.h
-- Installing: /usr/local/include/dlib/simd/simd8i.h
-- Installing: /usr/local/include/dlib/simd/simd4i.h
-- Installing: /usr/local/include/dlib/simd/simd8f.h
-- Installing: /usr/local/include/dlib/memory_manager_global
-- Installing: /usr/local/include/dlib/memory_manager_global/memory_manager_global_kernel_abstract.h
-- Installing: /usr/local/include/dlib/memory_manager_global/memory_manager_global_kernel_1.h
-- Installing: /usr/local/include/dlib/crc32.h
-- Installing: /usr/local/include/dlib/geometry
-- Installing: /usr/local/include/dlib/geometry/rectangle_abstract.h
-- Installing: /usr/local/include/dlib/geometry/point_transforms_abstract.h
-- Installing: /usr/local/include/dlib/geometry/vector_abstract.h
-- Installing: /usr/local/include/dlib/geometry/vector.h
-- Installing: /usr/local/include/dlib/geometry/drectangle_abstract.h
-- Installing: /usr/local/include/dlib/geometry/border_enumerator_abstract.h
-- Installing: /usr/local/include/dlib/geometry/drectangle.h
-- Installing: /usr/local/include/dlib/geometry/border_enumerator.h
-- Installing: /usr/local/include/dlib/geometry/rectangle.h
-- Installing: /usr/local/include/dlib/geometry/point_transforms.h
-- Installing: /usr/local/include/dlib/java
-- Installing: /usr/local/include/dlib/java/swig_api.h
-- Installing: /usr/local/include/dlib/java/jvector.h
-- Installing: /usr/local/include/dlib/numeric_constants.h
-- Installing: /usr/local/include/dlib/statistics
-- Installing: /usr/local/include/dlib/statistics/vector_normalizer_frobmetric_abstract.h
-- Installing: /usr/local/include/dlib/statistics/image_feature_sampling.h
-- Installing: /usr/local/include/dlib/statistics/random_subset_selector.h
-- Installing: /usr/local/include/dlib/statistics/dpca.h
-- Installing: /usr/local/include/dlib/statistics/dpca_abstract.h
-- Installing: /usr/local/include/dlib/statistics/statistics.h
-- Installing: /usr/local/include/dlib/statistics/statistics_abstract.h
-- Installing: /usr/local/include/dlib/statistics/sammon.h
-- Installing: /usr/local/include/dlib/statistics/random_subset_selector_abstract.h
-- Installing: /usr/local/include/dlib/statistics/cca.h
-- Installing: /usr/local/include/dlib/statistics/average_precision.h
-- Installing: /usr/local/include/dlib/statistics/running_gradient.h
-- Installing: /usr/local/include/dlib/statistics/lda_abstract.h
-- Installing: /usr/local/include/dlib/statistics/average_precision_abstract.h
-- Installing: /usr/local/include/dlib/statistics/image_feature_sampling_abstract.h
-- Installing: /usr/local/include/dlib/statistics/cca_abstract.h
-- Installing: /usr/local/include/dlib/statistics/vector_normalizer_frobmetric.h
-- Installing: /usr/local/include/dlib/statistics/lda.h
-- Installing: /usr/local/include/dlib/statistics/sammon_abstract.h
-- Installing: /usr/local/include/dlib/statistics/running_gradient_abstract.h
-- Installing: /usr/local/include/dlib/bayes_utils.h
-- Installing: /usr/local/include/dlib/entropy_decoder.h
-- Installing: /usr/local/include/dlib/control
-- Installing: /usr/local/include/dlib/control/mpc.h
-- Installing: /usr/local/include/dlib/control/lspi.h
-- Installing: /usr/local/include/dlib/control/lspi_abstract.h
-- Installing: /usr/local/include/dlib/control/mpc_abstract.h
-- Installing: /usr/local/include/dlib/control/approximate_linear_models.h
-- Installing: /usr/local/include/dlib/control/approximate_linear_models_abstract.h
-- Installing: /usr/local/include/dlib/travis
-- Installing: /usr/local/include/dlib/external
-- Installing: /usr/local/include/dlib/external/cblas
-- Installing: /usr/local/include/dlib/external/cblas/cblas_f77.h
-- Installing: /usr/local/include/dlib/external/cblas/cblas.h
-- Installing: /usr/local/include/dlib/external/libpng
-- Installing: /usr/local/include/dlib/external/libpng/pngdebug.h
-- Installing: /usr/local/include/dlib/external/libpng/pngstruct.h
-- Installing: /usr/local/include/dlib/external/libpng/pnginfo.h
-- Installing: /usr/local/include/dlib/external/libpng/pnglibconf.h
-- Installing: /usr/local/include/dlib/external/libpng/pngconf.h
-- Installing: /usr/local/include/dlib/external/libpng/png.h
-- Installing: /usr/local/include/dlib/external/libpng/arm
-- Installing: /usr/local/include/dlib/external/libpng/pngpriv.h
-- Installing: /usr/local/include/dlib/external/zlib
-- Installing: /usr/local/include/dlib/external/zlib/gzguts.h
-- Installing: /usr/local/include/dlib/external/zlib/zutil.h
-- Installing: /usr/local/include/dlib/external/zlib/inftrees.h
-- Installing: /usr/local/include/dlib/external/zlib/crc32.h
-- Installing: /usr/local/include/dlib/external/zlib/inflate.h
-- Installing: /usr/local/include/dlib/external/zlib/zconf.h
-- Installing: /usr/local/include/dlib/external/zlib/deflate.h
-- Installing: /usr/local/include/dlib/external/zlib/trees.h
-- Installing: /usr/local/include/dlib/external/zlib/inffixed.h
-- Installing: /usr/local/include/dlib/external/zlib/inffast.h
-- Installing: /usr/local/include/dlib/external/zlib/zlib.h
-- Installing: /usr/local/include/dlib/external/libjpeg
-- Installing: /usr/local/include/dlib/external/libjpeg/jdct.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jpeglib.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jerror.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jmorecfg.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jversion.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jpegint.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jdhuff.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jchuff.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jinclude.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jconfig.h
-- Installing: /usr/local/include/dlib/external/libjpeg/jmemsys.h
-- Installing: /usr/local/include/dlib/dir_nav.h
-- Installing: /usr/local/include/dlib/bound_function_pointer
-- Installing: /usr/local/include/dlib/bound_function_pointer/bound_function_pointer_kernel_1.h
-- Installing: /usr/local/include/dlib/bound_function_pointer/bound_function_pointer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/clustering.h
-- Installing: /usr/local/include/dlib/compress_stream.h
-- Installing: /usr/local/include/dlib/directed_graph.h
-- Installing: /usr/local/include/dlib/disjoint_subsets.h
-- Installing: /usr/local/include/dlib/serialize.h
-- Installing: /usr/local/include/dlib/dnn
-- Installing: /usr/local/include/dlib/dnn/loss_abstract.h
-- Installing: /usr/local/include/dlib/dnn/core.h
-- Installing: /usr/local/include/dlib/dnn/curand_dlibapi.h
-- Installing: /usr/local/include/dlib/dnn/input_abstract.h
-- Installing: /usr/local/include/dlib/dnn/cpu_dlib.h
-- Installing: /usr/local/include/dlib/dnn/core_abstract.h
-- Installing: /usr/local/include/dlib/dnn/utilities.h
-- Installing: /usr/local/include/dlib/dnn/cuda_errors.h
-- Installing: /usr/local/include/dlib/dnn/cuda_data_ptr.h
-- Installing: /usr/local/include/dlib/dnn/cublas_dlibapi.h
-- Installing: /usr/local/include/dlib/dnn/validation.h
-- Installing: /usr/local/include/dlib/dnn/cuda_dlib.h
-- Installing: /usr/local/include/dlib/dnn/tensor.h
-- Installing: /usr/local/include/dlib/dnn/gpu_data.h
-- Installing: /usr/local/include/dlib/dnn/layers.h
-- Installing: /usr/local/include/dlib/dnn/loss.h
-- Installing: /usr/local/include/dlib/dnn/trainer_abstract.h
-- Installing: /usr/local/include/dlib/dnn/trainer.h
-- Installing: /usr/local/include/dlib/dnn/cuda_utils.h
-- Installing: /usr/local/include/dlib/dnn/solvers_abstract.h
-- Installing: /usr/local/include/dlib/dnn/tensor_abstract.h
-- Installing: /usr/local/include/dlib/dnn/tensor_tools.h
-- Installing: /usr/local/include/dlib/dnn/layers_abstract.h
-- Installing: /usr/local/include/dlib/dnn/cusolver_dlibapi.h
-- Installing: /usr/local/include/dlib/dnn/gpu_data_abstract.h
-- Installing: /usr/local/include/dlib/dnn/solvers.h
-- Installing: /usr/local/include/dlib/dnn/input.h
-- Installing: /usr/local/include/dlib/dnn/cudnn_dlibapi.h
-- Installing: /usr/local/include/dlib/dnn/utilities_abstract.h
-- Installing: /usr/local/include/dlib/filtering.h
-- Installing: /usr/local/include/dlib/set_utils
-- Installing: /usr/local/include/dlib/set_utils/set_utils.h
-- Installing: /usr/local/include/dlib/set_utils/set_utils_abstract.h
-- Installing: /usr/local/include/dlib/platform.h
-- Installing: /usr/local/include/dlib/gui_widgets
-- Installing: /usr/local/include/dlib/gui_widgets/base_widgets.h
-- Installing: /usr/local/include/dlib/gui_widgets/style_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/base_widgets_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/nativefont.h
-- Installing: /usr/local/include/dlib/gui_widgets/drawable.h
-- Installing: /usr/local/include/dlib/gui_widgets/drawable_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/canvas_drawing_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/widgets.h
-- Installing: /usr/local/include/dlib/gui_widgets/fonts.h
-- Installing: /usr/local/include/dlib/gui_widgets/widgets_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/fonts_abstract.h
-- Installing: /usr/local/include/dlib/gui_widgets/canvas_drawing.h
-- Installing: /usr/local/include/dlib/gui_widgets/style.h
-- Installing: /usr/local/include/dlib/numerical_integration.h
-- Installing: /usr/local/include/dlib/linker.h
-- Installing: /usr/local/include/dlib/entropy_encoder
-- Installing: /usr/local/include/dlib/entropy_encoder/entropy_encoder_kernel_2.h
-- Installing: /usr/local/include/dlib/entropy_encoder/entropy_encoder_kernel_c.h
-- Installing: /usr/local/include/dlib/entropy_encoder/entropy_encoder_kernel_1.h
-- Installing: /usr/local/include/dlib/entropy_encoder/entropy_encoder_kernel_abstract.h
-- Installing: /usr/local/include/dlib/sqlite
-- Installing: /usr/local/include/dlib/sqlite/sqlite_abstract.h
-- Installing: /usr/local/include/dlib/sqlite/sqlite_tools.h
-- Installing: /usr/local/include/dlib/sqlite/sqlite_tools_abstract.h
-- Installing: /usr/local/include/dlib/sqlite/sqlite.h
-- Installing: /usr/local/include/dlib/bsp.h
-- Installing: /usr/local/include/dlib/config_reader.h
-- Installing: /usr/local/include/dlib/sliding_buffer
-- Installing: /usr/local/include/dlib/sliding_buffer/circular_buffer.h
-- Installing: /usr/local/include/dlib/sliding_buffer/sliding_buffer_kernel_1.h
-- Installing: /usr/local/include/dlib/sliding_buffer/sliding_buffer_kernel_c.h
-- Installing: /usr/local/include/dlib/sliding_buffer/sliding_buffer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/sliding_buffer/circular_buffer_abstract.h
-- Installing: /usr/local/include/dlib/hash_map.h
-- Installing: /usr/local/include/dlib/string.h
-- Installing: /usr/local/include/dlib/bit_stream
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_kernel_abstract.h
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_multi_1.h
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_kernel_c.h
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_multi_c.h
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_kernel_1.h
-- Installing: /usr/local/include/dlib/bit_stream/bit_stream_multi_abstract.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model.h
-- Installing: /usr/local/include/dlib/set
-- Installing: /usr/local/include/dlib/set/set_kernel_c.h
-- Installing: /usr/local/include/dlib/set/set_compare_1.h
-- Installing: /usr/local/include/dlib/set/set_compare_abstract.h
-- Installing: /usr/local/include/dlib/set/set_kernel_1.h
-- Installing: /usr/local/include/dlib/set/set_kernel_abstract.h
-- Installing: /usr/local/include/dlib/image_processing
-- Installing: /usr/local/include/dlib/image_processing/scan_image_boxes_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/box_overlap_testing.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_custom_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/render_face_detections_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/setup_hashed_features.h
-- Installing: /usr/local/include/dlib/image_processing/correlation_tracker_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_pyramid_tools_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/object_detector.h
-- Installing: /usr/local/include/dlib/image_processing/object_detector_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/correlation_tracker.h
-- Installing: /usr/local/include/dlib/image_processing/shape_predictor_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/full_object_detection.h
-- Installing: /usr/local/include/dlib/image_processing/render_face_detections.h
-- Installing: /usr/local/include/dlib/image_processing/box_overlap_testing_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/frontal_face_detector.h
-- Installing: /usr/local/include/dlib/image_processing/scan_fhog_pyramid_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_pyramid_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/full_object_detection_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/shape_predictor.h
-- Installing: /usr/local/include/dlib/image_processing/detection_template_tools_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_custom.h
-- Installing: /usr/local/include/dlib/image_processing/remove_unobtainable_rectangles_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/frontal_face_detector_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/setup_hashed_features_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/scan_fhog_pyramid.h
-- Installing: /usr/local/include/dlib/image_processing/generic_image.h
-- Installing: /usr/local/include/dlib/image_processing/shape_predictor_trainer_abstract.h
-- Installing: /usr/local/include/dlib/image_processing/remove_unobtainable_rectangles.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_pyramid.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_pyramid_tools.h
-- Installing: /usr/local/include/dlib/image_processing/detection_template_tools.h
-- Installing: /usr/local/include/dlib/image_processing/scan_image_boxes.h
-- Installing: /usr/local/include/dlib/image_processing/shape_predictor_trainer.h
-- Installing: /usr/local/include/dlib/graph.h
-- Installing: /usr/local/include/dlib/hash_table
-- Installing: /usr/local/include/dlib/hash_table/hash_table_kernel_1.h
-- Installing: /usr/local/include/dlib/hash_table/hash_table_kernel_abstract.h
-- Installing: /usr/local/include/dlib/hash_table/hash_table_kernel_2.h
-- Installing: /usr/local/include/dlib/hash_table/hash_table_kernel_c.h
-- Installing: /usr/local/include/dlib/stl_checked
-- Installing: /usr/local/include/dlib/stl_checked/std_vector_c.h
-- Installing: /usr/local/include/dlib/stl_checked/std_vector_c_abstract.h
-- Installing: /usr/local/include/dlib/python
-- Installing: /usr/local/include/dlib/python/pyassert.h
-- Installing: /usr/local/include/dlib/python/serialize_pickle.h
-- Installing: /usr/local/include/dlib/python/boost_python_utils.h
-- Installing: /usr/local/include/dlib/python/numpy.h
-- Installing: /usr/local/include/dlib/python/numpy_image.h
-- Installing: /usr/local/include/dlib/time_this.h
-- Installing: /usr/local/include/dlib/iosockstream.h
-- Installing: /usr/local/include/dlib/gui_core.h
-- Installing: /usr/local/include/dlib/logger
-- Installing: /usr/local/include/dlib/logger/extra_logger_headers.h
-- Installing: /usr/local/include/dlib/logger/logger_config_file.h
-- Installing: /usr/local/include/dlib/logger/logger_kernel_abstract.h
-- Installing: /usr/local/include/dlib/logger/logger_kernel_1.h
-- Installing: /usr/local/include/dlib/bridge
-- Installing: /usr/local/include/dlib/bridge/bridge_abstract.h
-- Installing: /usr/local/include/dlib/bridge/bridge.h
-- Installing: /usr/local/include/dlib/image_loader
-- Installing: /usr/local/include/dlib/image_loader/png_loader.h
-- Installing: /usr/local/include/dlib/image_loader/jpeg_loader_abstract.h
-- Installing: /usr/local/include/dlib/image_loader/image_loader_abstract.h
-- Installing: /usr/local/include/dlib/image_loader/load_image_abstract.h
-- Installing: /usr/local/include/dlib/image_loader/png_loader_abstract.h
-- Installing: /usr/local/include/dlib/image_loader/image_loader.h
-- Installing: /usr/local/include/dlib/image_loader/load_image.h
-- Installing: /usr/local/include/dlib/image_loader/jpeg_loader.h
-- Installing: /usr/local/include/dlib/timer.h
-- Installing: /usr/local/include/dlib/hash_set
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_abstract.h
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_1.h
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_c.h
-- Installing: /usr/local/include/dlib/timing.h
-- Installing: /usr/local/include/dlib/reference_counter.h
-- Installing: /usr/local/include/dlib/member_function_pointer
-- Installing: /usr/local/include/dlib/member_function_pointer/member_function_pointer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/member_function_pointer/make_mfp_abstract.h
-- Installing: /usr/local/include/dlib/member_function_pointer/make_mfp.h
-- Installing: /usr/local/include/dlib/member_function_pointer/member_function_pointer_kernel_1.h
-- Installing: /usr/local/include/dlib/array2d.h
-- Installing: /usr/local/include/dlib/gui_widgets.h
-- Installing: /usr/local/include/dlib/lsh.h
-- Installing: /usr/local/include/dlib/bigint
-- Installing: /usr/local/include/dlib/bigint/bigint_kernel_1.h
-- Installing: /usr/local/include/dlib/bigint/bigint_kernel_c.h
-- Installing: /usr/local/include/dlib/bigint/bigint_kernel_2.h
-- Installing: /usr/local/include/dlib/bigint/bigint_kernel_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint.h
-- Installing: /usr/local/include/dlib/hash_table.h
-- Installing: /usr/local/include/dlib/array
-- Installing: /usr/local/include/dlib/array/array_tools_abstract.h
-- Installing: /usr/local/include/dlib/array/array_kernel.h
-- Installing: /usr/local/include/dlib/array/array_kernel_abstract.h
-- Installing: /usr/local/include/dlib/array/array_tools.h
-- Installing: /usr/local/include/dlib/entropy_decoder
-- Installing: /usr/local/include/dlib/entropy_decoder/entropy_decoder_kernel_c.h
-- Installing: /usr/local/include/dlib/entropy_decoder/entropy_decoder_kernel_abstract.h
-- Installing: /usr/local/include/dlib/entropy_decoder/entropy_decoder_kernel_1.h
-- Installing: /usr/local/include/dlib/entropy_decoder/entropy_decoder_kernel_2.h
-- Installing: /usr/local/include/dlib/pixel.h
-- Installing: /usr/local/include/dlib/matrix.h
-- Installing: /usr/local/include/dlib/crc32
-- Installing: /usr/local/include/dlib/crc32/crc32_kernel_1.h
-- Installing: /usr/local/include/dlib/crc32/crc32_kernel_abstract.h
-- Installing: /usr/local/include/dlib/rand
-- Installing: /usr/local/include/dlib/rand/mersenne_twister.h
-- Installing: /usr/local/include/dlib/rand/rand_kernel_1.h
-- Installing: /usr/local/include/dlib/rand/rand_kernel_abstract.h
-- Installing: /usr/local/include/dlib/interfaces
-- Installing: /usr/local/include/dlib/interfaces/cmd_line_parser_option.h
-- Installing: /usr/local/include/dlib/interfaces/enumerable.h
-- Installing: /usr/local/include/dlib/interfaces/remover.h
-- Installing: /usr/local/include/dlib/interfaces/map_pair.h
-- Installing: /usr/local/include/dlib/hash_map
-- Installing: /usr/local/include/dlib/hash_map/hash_map_kernel_abstract.h
-- Installing: /usr/local/include/dlib/hash_map/hash_map_kernel_1.h
-- Installing: /usr/local/include/dlib/hash_map/hash_map_kernel_c.h
-- Installing: /usr/local/include/dlib/bridge.h
-- Installing: /usr/local/include/dlib/array2d
-- Installing: /usr/local/include/dlib/array2d/array2d_kernel_abstract.h
-- Installing: /usr/local/include/dlib/array2d/array2d_generic_image.h
-- Installing: /usr/local/include/dlib/array2d/array2d_kernel.h
-- Installing: /usr/local/include/dlib/array2d/serialize_pixel_overloads.h
-- Installing: /usr/local/include/dlib/stl_checked.h
-- Installing: /usr/local/include/dlib/graph_cuts
-- Installing: /usr/local/include/dlib/graph_cuts/find_max_factor_graph_potts_abstract.h
-- Installing: /usr/local/include/dlib/graph_cuts/graph_labeler.h
-- Installing: /usr/local/include/dlib/graph_cuts/min_cut_abstract.h
-- Installing: /usr/local/include/dlib/graph_cuts/min_cut.h
-- Installing: /usr/local/include/dlib/graph_cuts/graph_labeler_abstract.h
-- Installing: /usr/local/include/dlib/graph_cuts/general_potts_problem.h
-- Installing: /usr/local/include/dlib/graph_cuts/general_flow_graph.h
-- Installing: /usr/local/include/dlib/graph_cuts/find_max_factor_graph_potts.h
-- Installing: /usr/local/include/dlib/sparse_vector.h
-- Installing: /usr/local/include/dlib/quantum_computing.h
-- Installing: /usr/local/include/dlib/image_io.h
-- Installing: /usr/local/include/dlib/cpp_tokenizer
-- Installing: /usr/local/include/dlib/cpp_tokenizer/cpp_tokenizer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/cpp_tokenizer/cpp_tokenizer_kernel_1.h
-- Installing: /usr/local/include/dlib/cpp_tokenizer/cpp_tokenizer_kernel_c.h
-- Installing: /usr/local/include/dlib/static_map.h
-- Installing: /usr/local/include/dlib/stack
-- Installing: /usr/local/include/dlib/stack/stack_kernel_abstract.h
-- Installing: /usr/local/include/dlib/stack/stack_kernel_c.h
-- Installing: /usr/local/include/dlib/stack/stack_kernel_1.h
-- Installing: /usr/local/include/dlib/image_transforms.h
-- Installing: /usr/local/include/dlib/vectorstream
-- Installing: /usr/local/include/dlib/vectorstream/vectorstream_abstract.h
-- Installing: /usr/local/include/dlib/vectorstream/unserialize_abstract.h
-- Installing: /usr/local/include/dlib/vectorstream/unserialize.h
-- Installing: /usr/local/include/dlib/vectorstream/vectorstream.h
-- Installing: /usr/local/include/dlib/assert.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_6.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_abstract.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_2.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_4.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_3.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_5.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_1.h
-- Installing: /usr/local/include/dlib/entropy_encoder_model/entropy_encoder_model_kernel_c.h
-- Installing: /usr/local/include/dlib/quantum_computing
-- Installing: /usr/local/include/dlib/quantum_computing/quantum_computing_abstract.h
-- Installing: /usr/local/include/dlib/quantum_computing/quantum_computing.h
-- Installing: /usr/local/include/dlib/optimization
-- Installing: /usr/local/include/dlib/optimization/optimization_least_squares_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_bobyqa_abstract.h
-- Installing: /usr/local/include/dlib/optimization/find_max_parse_cky.h
-- Installing: /usr/local/include/dlib/optimization/find_max_factor_graph_nmplp_abstract.h
-- Installing: /usr/local/include/dlib/optimization/find_max_factor_graph_viterbi.h
-- Installing: /usr/local/include/dlib/optimization/optimization_abstract.h
-- Installing: /usr/local/include/dlib/optimization/find_max_parse_cky_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp2_using_smo.h
-- Installing: /usr/local/include/dlib/optimization/optimization.h
-- Installing: /usr/local/include/dlib/optimization/max_sum_submatrix_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_stop_strategies_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp3_using_smo.h
-- Installing: /usr/local/include/dlib/optimization/optimization_line_search.h
-- Installing: /usr/local/include/dlib/optimization/find_max_factor_graph_viterbi_abstract.h
-- Installing: /usr/local/include/dlib/optimization/max_cost_assignment.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp_using_smo.h
-- Installing: /usr/local/include/dlib/optimization/optimization_search_strategies_abstract.h
-- Installing: /usr/local/include/dlib/optimization/max_cost_assignment_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_trust_region_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_oca.h
-- Installing: /usr/local/include/dlib/optimization/optimization_trust_region.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp3_using_smo_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_least_squares.h
-- Installing: /usr/local/include/dlib/optimization/optimization_stop_strategies.h
-- Installing: /usr/local/include/dlib/optimization/find_optimal_parameters_abstract.h
-- Installing: /usr/local/include/dlib/optimization/find_max_factor_graph_nmplp.h
-- Installing: /usr/local/include/dlib/optimization/optimization_search_strategies.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp_using_smo_abstract.h
-- Installing: /usr/local/include/dlib/optimization/max_sum_submatrix.h
-- Installing: /usr/local/include/dlib/optimization/find_optimal_parameters.h
-- Installing: /usr/local/include/dlib/optimization/optimization_bobyqa.h
-- Installing: /usr/local/include/dlib/optimization/elastic_net.h
-- Installing: /usr/local/include/dlib/optimization/optimization_oca_abstract.h
-- Installing: /usr/local/include/dlib/optimization/elastic_net_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_line_search_abstract.h
-- Installing: /usr/local/include/dlib/optimization/optimization_solve_qp2_using_smo_abstract.h
-- Installing: /usr/local/include/dlib/cmd_line_parser.h
-- Installing: /usr/local/include/dlib/sqlite.h
-- Installing: /usr/local/include/dlib/smart_pointers
-- Installing: /usr/local/include/dlib/smart_pointers/shared_ptr_abstract.h
-- Installing: /usr/local/include/dlib/smart_pointers/weak_ptr.h
-- Installing: /usr/local/include/dlib/smart_pointers/shared_ptr_thread_safe_abstract.h
-- Installing: /usr/local/include/dlib/smart_pointers/weak_ptr_abstract.h
-- Installing: /usr/local/include/dlib/smart_pointers/shared_ptr.h
-- Installing: /usr/local/include/dlib/smart_pointers/shared_ptr_thread_safe.h
-- Installing: /usr/local/include/dlib/smart_pointers/scoped_ptr.h
-- Installing: /usr/local/include/dlib/static_set
-- Installing: /usr/local/include/dlib/static_set/static_set_compare_1.h
-- Installing: /usr/local/include/dlib/static_set/static_set_kernel_abstract.h
-- Installing: /usr/local/include/dlib/static_set/static_set_compare_abstract.h
-- Installing: /usr/local/include/dlib/static_set/static_set_kernel_1.h
-- Installing: /usr/local/include/dlib/static_set/static_set_kernel_c.h
-- Installing: /usr/local/include/dlib/matlab
-- Installing: /usr/local/include/dlib/matlab/subprocess_stream.h
-- Installing: /usr/local/include/dlib/matlab/call_matlab.h
-- Installing: /usr/local/include/dlib/sockstreambuf
-- Installing: /usr/local/include/dlib/sockstreambuf/sockstreambuf.h
-- Installing: /usr/local/include/dlib/sockstreambuf/sockstreambuf_abstract.h
-- Installing: /usr/local/include/dlib/sockstreambuf/sockstreambuf_unbuffered.h
-- Installing: /usr/local/include/dlib/mlp.h
-- Installing: /usr/local/include/dlib/timer
-- Installing: /usr/local/include/dlib/timer/timer.h
-- Installing: /usr/local/include/dlib/timer/timer_abstract.h
-- Installing: /usr/local/include/dlib/timer/timer_heavy.h
-- Installing: /usr/local/include/dlib/opencv
-- Installing: /usr/local/include/dlib/opencv/cv_image_abstract.h
-- Installing: /usr/local/include/dlib/opencv/to_open_cv.h
-- Installing: /usr/local/include/dlib/opencv/cv_image.h
-- Installing: /usr/local/include/dlib/opencv/to_open_cv_abstract.h
-- Installing: /usr/local/include/dlib/hash_set.h
-- Installing: /usr/local/include/dlib/float_details.h
-- Installing: /usr/local/include/dlib/xml_parser.h
-- Installing: /usr/local/include/dlib/conditioning_class.h
-- Installing: /usr/local/include/dlib/compress_stream
-- Installing: /usr/local/include/dlib/compress_stream/compress_stream_kernel_2.h
-- Installing: /usr/local/include/dlib/compress_stream/compress_stream_kernel_1.h
-- Installing: /usr/local/include/dlib/compress_stream/compress_stream_kernel_3.h
-- Installing: /usr/local/include/dlib/compress_stream/compress_stream_kernel_abstract.h
-- Installing: /usr/local/include/dlib/unicode
-- Installing: /usr/local/include/dlib/unicode/unicode.h
-- Installing: /usr/local/include/dlib/unicode/unicode_abstract.h
-- Installing: /usr/local/include/dlib/bayes_utils
-- Installing: /usr/local/include/dlib/bayes_utils/bayes_utils.h
-- Installing: /usr/local/include/dlib/bayes_utils/bayes_utils_abstract.h
-- Installing: /usr/local/include/dlib/data_io.h
-- Installing: /usr/local/include/dlib/timeout.h
-- Installing: /usr/local/include/dlib/clustering
-- Installing: /usr/local/include/dlib/clustering/modularity_clustering.h
-- Installing: /usr/local/include/dlib/clustering/chinese_whispers.h
-- Installing: /usr/local/include/dlib/clustering/modularity_clustering_abstract.h
-- Installing: /usr/local/include/dlib/clustering/spectral_cluster.h
-- Installing: /usr/local/include/dlib/clustering/chinese_whispers_abstract.h
-- Installing: /usr/local/include/dlib/clustering/bottom_up_cluster.h
-- Installing: /usr/local/include/dlib/clustering/spectral_cluster_abstract.h
-- Installing: /usr/local/include/dlib/clustering/bottom_up_cluster_abstract.h
-- Installing: /usr/local/include/dlib/is_kind.h
-- Installing: /usr/local/include/dlib/sockets
-- Installing: /usr/local/include/dlib/sockets/sockets_kernel_1.h
-- Installing: /usr/local/include/dlib/sockets/posix.h
-- Installing: /usr/local/include/dlib/sockets/sockets_extensions_abstract.h
-- Installing: /usr/local/include/dlib/sockets/sockets_kernel_abstract.h
-- Installing: /usr/local/include/dlib/sockets/sockets_extensions.h
-- Installing: /usr/local/include/dlib/sockets/windows.h
-- Installing: /usr/local/include/dlib/sockets/sockets_kernel_2.h
-- Installing: /usr/local/include/dlib/entropy_decoder_model.h
-- Installing: /usr/local/include/dlib/map
-- Installing: /usr/local/include/dlib/map/map_kernel_c.h
-- Installing: /usr/local/include/dlib/map/map_kernel_1.h
-- Installing: /usr/local/include/dlib/map/map_kernel_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint
-- Installing: /usr/local/include/dlib/image_keypoint/surf.h
-- Installing: /usr/local/include/dlib/image_keypoint/draw_surf_points_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/binned_vector_feature_image.h
-- Installing: /usr/local/include/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/hashed_feature_image_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/fine_hog_image_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/hog.h
-- Installing: /usr/local/include/dlib/image_keypoint/surf_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/poly_image.h
-- Installing: /usr/local/include/dlib/image_keypoint/hessian_pyramid_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/hashed_feature_image.h
-- Installing: /usr/local/include/dlib/image_keypoint/poly_image_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/draw_surf_points.h
-- Installing: /usr/local/include/dlib/image_keypoint/nearest_neighbor_feature_image.h
-- Installing: /usr/local/include/dlib/image_keypoint/binned_vector_feature_image_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/fine_hog_image.h
-- Installing: /usr/local/include/dlib/image_keypoint/build_separable_poly_filters.h
-- Installing: /usr/local/include/dlib/image_keypoint/hog_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/hessian_pyramid.h
-- Installing: /usr/local/include/dlib/error.h
-- Installing: /usr/local/include/dlib/unordered_pair.h
-- Installing: /usr/local/include/dlib/directed_graph
-- Installing: /usr/local/include/dlib/directed_graph/directed_graph_kernel_abstract.h
-- Installing: /usr/local/include/dlib/directed_graph/directed_graph_kernel_1.h
-- Installing: /usr/local/include/dlib/image_transforms
-- Installing: /usr/local/include/dlib/image_transforms/label_connected_blobs.h
-- Installing: /usr/local/include/dlib/image_transforms/spatial_filtering_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/interpolation.h
-- Installing: /usr/local/include/dlib/image_transforms/equalize_histogram.h
-- Installing: /usr/local/include/dlib/image_transforms/morphological_operations_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/random_color_transform.h
-- Installing: /usr/local/include/dlib/image_transforms/lbp_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/draw.h
-- Installing: /usr/local/include/dlib/image_transforms/image_pyramid_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/colormaps.h
-- Installing: /usr/local/include/dlib/image_transforms/image_pyramid.h
-- Installing: /usr/local/include/dlib/image_transforms/hough_transform_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/integral_image_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/fhog_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/edge_detector.h
-- Installing: /usr/local/include/dlib/image_transforms/hough_transform.h
-- Installing: /usr/local/include/dlib/image_transforms/segment_image.h
-- Installing: /usr/local/include/dlib/image_transforms/draw_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/spatial_filtering.h
-- Installing: /usr/local/include/dlib/image_transforms/equalize_histogram_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/assign_image.h
-- Installing: /usr/local/include/dlib/image_transforms/random_cropper.h
-- Installing: /usr/local/include/dlib/image_transforms/thresholding_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/random_cropper_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/segment_image_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/label_connected_blobs_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/integral_image.h
-- Installing: /usr/local/include/dlib/image_transforms/random_color_transform_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/edge_detector_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/assign_image_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/thresholding.h
-- Installing: /usr/local/include/dlib/image_transforms/colormaps_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/fhog.h
-- Installing: /usr/local/include/dlib/image_transforms/interpolation_abstract.h
-- Installing: /usr/local/include/dlib/image_transforms/morphological_operations.h
-- Installing: /usr/local/include/dlib/image_transforms/lbp.h
-- Installing: /usr/local/include/dlib/lz77_buffer
-- Installing: /usr/local/include/dlib/lz77_buffer/lz77_buffer_kernel_c.h
-- Installing: /usr/local/include/dlib/lz77_buffer/lz77_buffer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/lz77_buffer/lz77_buffer_kernel_1.h
-- Installing: /usr/local/include/dlib/lz77_buffer/lz77_buffer_kernel_2.h
-- Installing: /usr/local/include/dlib/sort.h
-- Installing: /usr/local/include/dlib/tokenizer.h
-- Installing: /usr/local/include/dlib/all
-- Installing: /usr/local/include/dlib/gui_core
-- Installing: /usr/local/include/dlib/gui_core/windows.h
-- Installing: /usr/local/include/dlib/gui_core/xlib.h
-- Installing: /usr/local/include/dlib/gui_core/gui_core_kernel_abstract.h
-- Installing: /usr/local/include/dlib/gui_core/gui_core_kernel_1.h
-- Installing: /usr/local/include/dlib/gui_core/gui_core_kernel_2.h
-- Installing: /usr/local/include/dlib/svm
-- Installing: /usr/local/include/dlib/svm/assignment_function.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_sequence_labeling_problem_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_multiclass_linear_trainer.h
-- Installing: /usr/local/include/dlib/svm/svm_c_ekm_trainer.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_regression_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/function_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_all_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm.h
-- Installing: /usr/local/include/dlib/svm/structural_assignment_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/linearly_independent_subset_finder.h
-- Installing: /usr/local/include/dlib/svm/svm_multiclass_linear_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_rank_trainer.h
-- Installing: /usr/local/include/dlib/svm/sort_basis_vectors.h
-- Installing: /usr/local/include/dlib/svm/svm_threaded.h
-- Installing: /usr/local/include/dlib/svm/svr_linear_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/active_learning.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_object_detection_trainer.h
-- Installing: /usr/local/include/dlib/svm/structural_track_association_trainer.h
-- Installing: /usr/local/include/dlib/svm/kernel_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_one_decision_function.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_object_detection_problem.h
-- Installing: /usr/local/include/dlib/svm/svm_abstract.h
-- Installing: /usr/local/include/dlib/svm/kernel.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_problem_threaded.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_problem_threaded_abstract.h
-- Installing: /usr/local/include/dlib/svm/num_nonnegative_weights.h
-- Installing: /usr/local/include/dlib/svm/kernel_matrix_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_one_trainer.h
-- Installing: /usr/local/include/dlib/svm/rr_trainer.h
-- Installing: /usr/local/include/dlib/svm/kcentroid_overloads.h
-- Installing: /usr/local/include/dlib/svm/svm_nu_trainer.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_sequence_labeler.h
-- Installing: /usr/local/include/dlib/svm/rbf_network_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_one_decision_function_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_assignment_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_problem.h
-- Installing: /usr/local/include/dlib/svm/pegasos_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_one_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_track_association_trainer.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_sequence_labeler_abstract.h
-- Installing: /usr/local/include/dlib/svm/ranking_tools.h
-- Installing: /usr/local/include/dlib/svm/structural_sequence_segmentation_trainer.h
-- Installing: /usr/local/include/dlib/svm/pegasos.h
-- Installing: /usr/local/include/dlib/svm/svm_c_trainer.h
-- Installing: /usr/local/include/dlib/svm/svm_c_linear_dcd_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/kcentroid.h
-- Installing: /usr/local/include/dlib/svm/sparse_kernel.h
-- Installing: /usr/local/include/dlib/svm/structural_track_association_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/empirical_kernel_map_abstract.h
-- Installing: /usr/local/include/dlib/svm/one_vs_all_decision_function.h
-- Installing: /usr/local/include/dlib/svm/null_trainer.h
-- Installing: /usr/local/include/dlib/svm/one_vs_all_trainer.h
-- Installing: /usr/local/include/dlib/svm/structural_object_detection_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/track_association_function_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_c_linear_trainer.h
-- Installing: /usr/local/include/dlib/svm/sparse_kernel_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_graph_labeling_trainer.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_graph_labeling_problem_abstract.h
-- Installing: /usr/local/include/dlib/svm/simplify_linear_decision_function_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_c_ekm_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/reduced.h
-- Installing: /usr/local/include/dlib/svm/kcentroid_abstract.h
-- Installing: /usr/local/include/dlib/svm/rbf_network.h
-- Installing: /usr/local/include/dlib/svm/structural_sequence_labeling_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_c_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/rls.h
-- Installing: /usr/local/include/dlib/svm/rvm_abstract.h
-- Installing: /usr/local/include/dlib/svm/rvm.h
-- Installing: /usr/local/include/dlib/svm/multiclass_tools.h
-- Installing: /usr/local/include/dlib/svm/structural_object_detection_trainer.h
-- Installing: /usr/local/include/dlib/svm/svm_rank_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svr_trainer.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_assignment_problem.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_distributed_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_distributed.h
-- Installing: /usr/local/include/dlib/svm/null_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/simplify_linear_decision_function.h
-- Installing: /usr/local/include/dlib/svm/krls_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_graph_labeling_problem.h
-- Installing: /usr/local/include/dlib/svm/rls_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_threaded_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_c_linear_dcd_trainer.h
-- Installing: /usr/local/include/dlib/svm/roc_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_one_class_trainer.h
-- Installing: /usr/local/include/dlib/svm/svm_nu_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/sequence_labeler_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_assignment_problem_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_sequence_segmentation_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/linearly_independent_subset_finder_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_multiclass_trainer.h
-- Installing: /usr/local/include/dlib/svm/feature_ranking.h
-- Installing: /usr/local/include/dlib/svm/reduced_abstract.h
-- Installing: /usr/local/include/dlib/svm/kkmeans.h
-- Installing: /usr/local/include/dlib/svm/rr_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/roc_trainer.h
-- Installing: /usr/local/include/dlib/svm/krr_trainer.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_sequence_segmenter.h
-- Installing: /usr/local/include/dlib/svm/ranking_tools_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_object_detection_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/krls.h
-- Installing: /usr/local/include/dlib/svm/one_vs_all_decision_function_abstract.h
-- Installing: /usr/local/include/dlib/svm/sequence_labeler.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_assignment_trainer.h
-- Installing: /usr/local/include/dlib/svm/active_learning_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_sequence_segmenter_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_assignment_trainer.h
-- Installing: /usr/local/include/dlib/svm/sequence_segmenter_abstract.h
-- Installing: /usr/local/include/dlib/svm/krr_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/sparse_vector.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_object_detection_problem_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_sequence_labeling_problem.h
-- Installing: /usr/local/include/dlib/svm/svm_one_class_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/sequence_segmenter.h
-- Installing: /usr/local/include/dlib/svm/assignment_function_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_graph_labeling_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svm_c_linear_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/sparse_vector_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_graph_labeling_trainer.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_regression_trainer.h
-- Installing: /usr/local/include/dlib/svm/null_df.h
-- Installing: /usr/local/include/dlib/svm/structural_svm_problem_abstract.h
-- Installing: /usr/local/include/dlib/svm/multiclass_tools_abstract.h
-- Installing: /usr/local/include/dlib/svm/kernel_matrix.h
-- Installing: /usr/local/include/dlib/svm/empirical_kernel_map.h
-- Installing: /usr/local/include/dlib/svm/kkmeans_abstract.h
-- Installing: /usr/local/include/dlib/svm/sort_basis_vectors_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_track_association_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/track_association_function.h
-- Installing: /usr/local/include/dlib/svm/structural_sequence_labeling_trainer.h
-- Installing: /usr/local/include/dlib/svm/svr_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/cross_validate_multiclass_trainer_abstract.h
-- Installing: /usr/local/include/dlib/svm/svr_linear_trainer.h
-- Installing: /usr/local/include/dlib/svm/function.h
-- Installing: /usr/local/include/dlib/svm/feature_ranking_abstract.h
-- Installing: /usr/local/include/dlib/svm/structural_graph_labeling_trainer_abstract.h
-- Installing: /usr/local/include/dlib/queue.h
-- Installing: /usr/local/include/dlib/smart_pointers.h
-- Installing: /usr/local/include/dlib/timeout
-- Installing: /usr/local/include/dlib/timeout/timeout.h
-- Installing: /usr/local/include/dlib/timeout/timeout_abstract.h
-- Installing: /usr/local/include/dlib/cpp_pretty_printer.h
-- Installing: /usr/local/include/dlib/image_saver
-- Installing: /usr/local/include/dlib/image_saver/save_png_abstract.h
-- Installing: /usr/local/include/dlib/image_saver/save_png.h
-- Installing: /usr/local/include/dlib/image_saver/dng_shared.h
-- Installing: /usr/local/include/dlib/image_saver/image_saver_abstract.h
-- Installing: /usr/local/include/dlib/image_saver/save_jpeg_abstract.h
-- Installing: /usr/local/include/dlib/image_saver/image_saver.h
-- Installing: /usr/local/include/dlib/image_saver/save_jpeg.h
-- Installing: /usr/local/include/dlib/windows_magic.h
-- Installing: /usr/local/include/dlib/base64.h
-- Installing: /usr/local/include/dlib/test
-- Installing: /usr/local/include/dlib/test/create_iris_datafile.h
-- Installing: /usr/local/include/dlib/test/gui
-- Installing: /usr/local/include/dlib/test/tester.h
-- Installing: /usr/local/include/dlib/test/tools
-- Installing: /usr/local/include/dlib/test/binary_search_tree.h
-- Installing: /usr/local/include/dlib/test/checkerboard.h
-- Installing: /usr/local/include/dlib/test/cmd_line_parser.h
-- Installing: /usr/local/include/dlib/test/blas_bindings
-- Installing: /usr/local/include/dlib/test/optimization_test_functions.h
-- Installing: /usr/local/include/dlib/test/conditioning_class.h
-- Installing: /usr/local/include/dlib/test/examples
-- Installing: /usr/local/include/dlib/type_safe_union.h
-- Installing: /usr/local/include/dlib/matrix
-- Installing: /usr/local/include/dlib/matrix/matrix_assign_fwd.h
-- Installing: /usr/local/include/dlib/matrix/matrix_utilities.h
-- Installing: /usr/local/include/dlib/matrix/matrix_exp_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_subexp.h
-- Installing: /usr/local/include/dlib/matrix/matrix_fft.h
-- Installing: /usr/local/include/dlib/matrix/matrix_lu.h
-- Installing: /usr/local/include/dlib/matrix/matrix_data_layout.h
-- Installing: /usr/local/include/dlib/matrix/matrix_fwd.h
-- Installing: /usr/local/include/dlib/matrix/matrix_expressions.h
-- Installing: /usr/local/include/dlib/matrix/matrix_math_functions.h
-- Installing: /usr/local/include/dlib/matrix/matrix_eigenvalue.h
-- Installing: /usr/local/include/dlib/matrix/matrix_fft_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_assign.h
-- Installing: /usr/local/include/dlib/matrix/matrix_la.h
-- Installing: /usr/local/include/dlib/matrix/matrix_la_abstract.h
-- Installing: /usr/local/include/dlib/matrix/symmetric_matrix_cache.h
-- Installing: /usr/local/include/dlib/matrix/matrix_mat_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_utilities_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_trsm.h
-- Installing: /usr/local/include/dlib/matrix/matrix_read_from_istream.h
-- Installing: /usr/local/include/dlib/matrix/matrix_conv.h
-- Installing: /usr/local/include/dlib/matrix/matrix_mat.h
-- Installing: /usr/local/include/dlib/matrix/matrix_conj_trans.h
-- Installing: /usr/local/include/dlib/matrix/matrix_blas_bindings.h
-- Installing: /usr/local/include/dlib/matrix/matrix_data_layout_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix.h
-- Installing: /usr/local/include/dlib/matrix/matrix_generic_image.h
-- Installing: /usr/local/include/dlib/matrix/matrix_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_conv_abstract.h
-- Installing: /usr/local/include/dlib/matrix/cblas_constants.h
-- Installing: /usr/local/include/dlib/matrix/matrix_exp.h
-- Installing: /usr/local/include/dlib/matrix/lapack
-- Installing: /usr/local/include/dlib/matrix/lapack/fortran_id.h
-- Installing: /usr/local/include/dlib/matrix/lapack/gesdd.h
-- Installing: /usr/local/include/dlib/matrix/lapack/ormqr.h
-- Installing: /usr/local/include/dlib/matrix/lapack/geev.h
-- Installing: /usr/local/include/dlib/matrix/lapack/potrf.h
-- Installing: /usr/local/include/dlib/matrix/lapack/syevr.h
-- Installing: /usr/local/include/dlib/matrix/lapack/geqrf.h
-- Installing: /usr/local/include/dlib/matrix/lapack/gesvd.h
-- Installing: /usr/local/include/dlib/matrix/lapack/gees.h
-- Installing: /usr/local/include/dlib/matrix/lapack/syev.h
-- Installing: /usr/local/include/dlib/matrix/lapack/getrf.h
-- Installing: /usr/local/include/dlib/matrix/matrix_cholesky.h
-- Installing: /usr/local/include/dlib/matrix/matrix_math_functions_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_subexp_abstract.h
-- Installing: /usr/local/include/dlib/matrix/matrix_op.h
-- Installing: /usr/local/include/dlib/matrix/matrix_default_mul.h
-- Installing: /usr/local/include/dlib/matrix/matrix_qr.h
-- Installing: /usr/local/include/dlib/matrix/symmetric_matrix_cache_abstract.h
-- Installing: /usr/local/include/dlib/logger.h
-- Installing: /usr/local/include/dlib/noncopyable.h
-- Installing: /usr/local/include/dlib/bsp
-- Installing: /usr/local/include/dlib/bsp/bsp_abstract.h
-- Installing: /usr/local/include/dlib/bsp/bsp.h
-- Installing: /usr/local/include/dlib/cpp_pretty_printer
-- Installing: /usr/local/include/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_2.h
-- Installing: /usr/local/include/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_1.h
-- Installing: /usr/local/include/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_abstract.h
-- Installing: /usr/local/include/dlib/vectorstream.h
-- Installing: /usr/local/include/dlib/control.h
-- Installing: /usr/local/include/dlib/config.h
-- Installing: /usr/local/include/dlib/revision.h
-- Installing: /usr/local/lib/cmake/dlib/dlib.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlib-release.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlibConfig.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlibConfigVersion.cmake
-- Installing: /usr/local/lib/pkgconfig/dlib-1.pc
map479@map479-DQ57TM:~/dlib/build$

```



#### testing



```
map479@map479-DQ57TM:~/dlib/build$ cd ../examples/ && mkdir build && cd build && cmake ..
-- The C compiler identification is GNU 5.4.0
-- The CXX compiler identification is GNU 5.4.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- C++11 activated.
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Looking for pthread_create
-- Looking for pthread_create - not found
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Looking for XOpenDisplay in /usr/lib/x86_64-linux-gnu/libX11.so;/usr/lib/x86_64-linux-gnu/libXext.so
-- Looking for XOpenDisplay in /usr/lib/x86_64-linux-gnu/libX11.so;/usr/lib/x86_64-linux-gnu/libXext.so - found
-- Looking for gethostbyname
-- Looking for gethostbyname - found
-- Looking for connect
-- Looking for connect - found
-- Looking for remove
-- Looking for remove - found
-- Looking for shmat
-- Looking for shmat - found
-- Looking for IceConnectionNumber in ICE
-- Looking for IceConnectionNumber in ICE - found
-- Found X11: /usr/lib/x86_64-linux-gnu/libX11.so
-- Looking for png_create_read_struct
-- Looking for png_create_read_struct - found
-- Looking for jpeg_read_header
-- Looking for jpeg_read_header - found
-- Searching for BLAS and LAPACK
-- Found PkgConfig: /usr/bin/pkg-config (found version "0.29.1")
-- Checking for module 'cblas'
--   No package 'cblas' found
-- Checking for module 'lapack'
--   Found lapack, version 3.10.2
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of void*
-- Check size of void* - done
-- Found LAPACK library
-- Found ATLAS BLAS library
-- Looking for cblas_ddot
-- Looking for cblas_ddot - found
CUDA_TOOLKIT_ROOT_DIR not found or specified
-- Could NOT find CUDA (missing:  CUDA_TOOLKIT_ROOT_DIR CUDA_NVCC_EXECUTABLE CUDA_INCLUDE_DIRS CUDA_CUDART_LIBRARY) (Required is at least version "7.5")
-- *** cuDNN V5.0 OR GREATER NOT FOUND.  DLIB WILL NOT USE CUDA. ***
-- *** If you have cuDNN then set CMAKE_PREFIX_PATH to include cuDNN's folder.
-- Configuring done
-- Generating done
-- Build files have been written to: /home/map479/dlib/examples/build
map479@map479-DQ57TM:~/dlib/examples/build$

```






```
$ cmake --build . --config Release
Scanning dependencies of target dlib
[  1%] Building CXX object dlib_build/CMakeFiles/dlib.dir/base64/base64_kernel_1.cpp.o
[  1%] Building CXX object dlib_build/CMakeFiles/dlib.dir/bigint/bigint_kernel_1.cpp.o
[  2%] Building CXX object dlib_build/CMakeFiles/dlib.dir/bigint/bigint_kernel_2.cpp.o
[  2%] Building CXX object dlib_build/CMakeFiles/dlib.dir/bit_stream/bit_stream_kernel_1.cpp.o
[  2%] Building CXX object dlib_build/CMakeFiles/dlib.dir/entropy_decoder/entropy_decoder_kernel_1.cpp.o
[  3%] Building CXX object dlib_build/CMakeFiles/dlib.dir/entropy_decoder/entropy_decoder_kernel_2.cpp.o
[  3%] Building CXX object dlib_build/CMakeFiles/dlib.dir/entropy_encoder/entropy_encoder_kernel_1.cpp.o
[  4%] Building CXX object dlib_build/CMakeFiles/dlib.dir/entropy_encoder/entropy_encoder_kernel_2.cpp.o
[  4%] Building CXX object dlib_build/CMakeFiles/dlib.dir/md5/md5_kernel_1.cpp.o
[  4%] Building CXX object dlib_build/CMakeFiles/dlib.dir/tokenizer/tokenizer_kernel_1.cpp.o
[  5%] Building CXX object dlib_build/CMakeFiles/dlib.dir/unicode/unicode.cpp.o
[  5%] Building CXX object dlib_build/CMakeFiles/dlib.dir/data_io/image_dataset_metadata.cpp.o
[  6%] Building CXX object dlib_build/CMakeFiles/dlib.dir/data_io/mnist.cpp.o
[  6%] Building CXX object dlib_build/CMakeFiles/dlib.dir/dnn/cpu_dlib.cpp.o
[  6%] Building CXX object dlib_build/CMakeFiles/dlib.dir/dnn/tensor_tools.cpp.o
[  7%] Building CXX object dlib_build/CMakeFiles/dlib.dir/sockets/sockets_kernel_1.cpp.o
[  7%] Building CXX object dlib_build/CMakeFiles/dlib.dir/bsp/bsp.cpp.o
[  8%] Building CXX object dlib_build/CMakeFiles/dlib.dir/dir_nav/dir_nav_kernel_1.cpp.o
[  8%] Building CXX object dlib_build/CMakeFiles/dlib.dir/dir_nav/dir_nav_kernel_2.cpp.o
[  9%] Building CXX object dlib_build/CMakeFiles/dlib.dir/dir_nav/dir_nav_extensions.cpp.o
[  9%] Building CXX object dlib_build/CMakeFiles/dlib.dir/linker/linker_kernel_1.cpp.o
[  9%] Building CXX object dlib_build/CMakeFiles/dlib.dir/logger/extra_logger_headers.cpp.o
[ 10%] Building CXX object dlib_build/CMakeFiles/dlib.dir/logger/logger_kernel_1.cpp.o
[ 10%] Building CXX object dlib_build/CMakeFiles/dlib.dir/logger/logger_config_file.cpp.o
[ 11%] Building CXX object dlib_build/CMakeFiles/dlib.dir/misc_api/misc_api_kernel_1.cpp.o
[ 11%] Building CXX object dlib_build/CMakeFiles/dlib.dir/misc_api/misc_api_kernel_2.cpp.o
[ 11%] Building CXX object dlib_build/CMakeFiles/dlib.dir/sockets/sockets_extensions.cpp.o
[ 12%] Building CXX object dlib_build/CMakeFiles/dlib.dir/sockets/sockets_kernel_2.cpp.o
[ 12%] Building CXX object dlib_build/CMakeFiles/dlib.dir/sockstreambuf/sockstreambuf.cpp.o
[ 13%] Building CXX object dlib_build/CMakeFiles/dlib.dir/sockstreambuf/sockstreambuf_unbuffered.cpp.o
[ 13%] Building CXX object dlib_build/CMakeFiles/dlib.dir/server/server_kernel.cpp.o
[ 13%] Building CXX object dlib_build/CMakeFiles/dlib.dir/server/server_iostream.cpp.o
[ 14%] Building CXX object dlib_build/CMakeFiles/dlib.dir/server/server_http.cpp.o
[ 14%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/multithreaded_object_extension.cpp.o
[ 15%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/threaded_object_extension.cpp.o
[ 15%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/threads_kernel_1.cpp.o
[ 15%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/threads_kernel_2.cpp.o
[ 16%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/threads_kernel_shared.cpp.o
[ 16%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/thread_pool_extension.cpp.o
[ 17%] Building CXX object dlib_build/CMakeFiles/dlib.dir/threads/async.cpp.o
[ 17%] Building CXX object dlib_build/CMakeFiles/dlib.dir/timer/timer.cpp.o
[ 17%] Building CXX object dlib_build/CMakeFiles/dlib.dir/stack_trace.cpp.o
[ 18%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/fonts.cpp.o
[ 18%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/widgets.cpp.o
[ 19%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/drawable.cpp.o
[ 19%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/canvas_drawing.cpp.o
[ 19%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/style.cpp.o
[ 20%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_widgets/base_widgets.cpp.o
[ 20%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_core/gui_core_kernel_1.cpp.o
[ 21%] Building CXX object dlib_build/CMakeFiles/dlib.dir/gui_core/gui_core_kernel_2.cpp.o
[ 21%] Building CXX object dlib_build/CMakeFiles/dlib.dir/image_loader/png_loader.cpp.o
[ 21%] Building CXX object dlib_build/CMakeFiles/dlib.dir/image_saver/save_png.cpp.o
[ 22%] Building CXX object dlib_build/CMakeFiles/dlib.dir/image_loader/jpeg_loader.cpp.o
[ 22%] Building CXX object dlib_build/CMakeFiles/dlib.dir/image_saver/save_jpeg.cpp.o
[ 23%] Linking CXX static library libdlib.a
[ 23%] Built target dlib
Scanning dependencies of target linear_manifold_regularizer_ex
[ 23%] Building CXX object CMakeFiles/linear_manifold_regularizer_ex.dir/linear_manifold_regularizer_ex.cpp.o
[ 24%] Linking CXX executable linear_manifold_regularizer_ex
[ 24%] Built target linear_manifold_regularizer_ex
Scanning dependencies of target mpc_ex
[ 24%] Building CXX object CMakeFiles/mpc_ex.dir/mpc_ex.cpp.o
[ 25%] Linking CXX executable mpc_ex
[ 25%] Built target mpc_ex
Scanning dependencies of target rvm_ex
[ 25%] Building CXX object CMakeFiles/rvm_ex.dir/rvm_ex.cpp.o
[ 26%] Linking CXX executable rvm_ex
[ 26%] Built target rvm_ex
Scanning dependencies of target krr_classification_ex
[ 26%] Building CXX object CMakeFiles/krr_classification_ex.dir/krr_classification_ex.cpp.o
[ 26%] Linking CXX executable krr_classification_ex
[ 26%] Built target krr_classification_ex
Scanning dependencies of target iosockstream_ex
[ 27%] Building CXX object CMakeFiles/iosockstream_ex.dir/iosockstream_ex.cpp.o
[ 27%] Linking CXX executable iosockstream_ex
[ 27%] Built target iosockstream_ex
Scanning dependencies of target integrate_function_adapt_simp_ex
[ 27%] Building CXX object CMakeFiles/integrate_function_adapt_simp_ex.dir/integrate_function_adapt_simp_ex.cpp.o
[ 27%] Linking CXX executable integrate_function_adapt_simp_ex
[ 27%] Built target integrate_function_adapt_simp_ex
Scanning dependencies of target image_ex
[ 27%] Building CXX object CMakeFiles/image_ex.dir/image_ex.cpp.o
[ 28%] Linking CXX executable image_ex
[ 28%] Built target image_ex
Scanning dependencies of target gui_api_ex
[ 29%] Building CXX object CMakeFiles/gui_api_ex.dir/gui_api_ex.cpp.o
[ 29%] Linking CXX executable gui_api_ex
[ 29%] Built target gui_api_ex
Scanning dependencies of target video_tracking_ex
[ 29%] Building CXX object CMakeFiles/video_tracking_ex.dir/video_tracking_ex.cpp.o
[ 30%] Linking CXX executable video_tracking_ex
[ 30%] Built target video_tracking_ex
Scanning dependencies of target logger_custom_output_ex
[ 30%] Building CXX object CMakeFiles/logger_custom_output_ex.dir/logger_custom_output_ex.cpp.o
[ 30%] Linking CXX executable logger_custom_output_ex
[ 30%] Built target logger_custom_output_ex
Scanning dependencies of target file_to_code_ex
[ 30%] Building CXX object CMakeFiles/file_to_code_ex.dir/file_to_code_ex.cpp.o
[ 30%] Linking CXX executable file_to_code_ex
[ 30%] Built target file_to_code_ex
Scanning dependencies of target fhog_ex
[ 30%] Building CXX object CMakeFiles/fhog_ex.dir/fhog_ex.cpp.o
[ 31%] Linking CXX executable fhog_ex
[ 31%] Built target fhog_ex
Scanning dependencies of target rank_features_ex
[ 32%] Building CXX object CMakeFiles/rank_features_ex.dir/rank_features_ex.cpp.o
[ 32%] Linking CXX executable rank_features_ex
[ 32%] Built target rank_features_ex
Scanning dependencies of target face_detection_ex
[ 33%] Building CXX object CMakeFiles/face_detection_ex.dir/face_detection_ex.cpp.o
[ 33%] Linking CXX executable face_detection_ex
[ 33%] Built target face_detection_ex
Scanning dependencies of target dir_nav_ex
[ 33%] Building CXX object CMakeFiles/dir_nav_ex.dir/dir_nav_ex.cpp.o
[ 33%] Linking CXX executable dir_nav_ex
[ 33%] Built target dir_nav_ex
Scanning dependencies of target empirical_kernel_map_ex
[ 33%] Building CXX object CMakeFiles/empirical_kernel_map_ex.dir/empirical_kernel_map_ex.cpp.o
[ 33%] Linking CXX executable empirical_kernel_map_ex
[ 33%] Built target empirical_kernel_map_ex
Scanning dependencies of target multithreaded_object_ex
[ 34%] Building CXX object CMakeFiles/multithreaded_object_ex.dir/multithreaded_object_ex.cpp.o
[ 34%] Linking CXX executable multithreaded_object_ex
[ 34%] Built target multithreaded_object_ex
Scanning dependencies of target dnn_introduction_ex
[ 34%] Building CXX object CMakeFiles/dnn_introduction_ex.dir/dnn_introduction_ex.cpp.o
[ 35%] Linking CXX executable dnn_introduction_ex
[ 35%] Built target dnn_introduction_ex
Scanning dependencies of target hough_transform_ex
[ 35%] Building CXX object CMakeFiles/hough_transform_ex.dir/hough_transform_ex.cpp.o
[ 36%] Linking CXX executable hough_transform_ex
[ 36%] Built target hough_transform_ex
Scanning dependencies of target krls_ex
[ 36%] Building CXX object CMakeFiles/krls_ex.dir/krls_ex.cpp.o
[ 37%] Linking CXX executable krls_ex
[ 37%] Built target krls_ex
Scanning dependencies of target queue_ex
[ 37%] Building CXX object CMakeFiles/queue_ex.dir/queue_ex.cpp.o
[ 38%] Linking CXX executable queue_ex
[ 38%] Built target queue_ex
Scanning dependencies of target dnn_mmod_ex
[ 38%] Building CXX object CMakeFiles/dnn_mmod_ex.dir/dnn_mmod_ex.cpp.o
[ 39%] Linking CXX executable dnn_mmod_ex
[ 39%] Built target dnn_mmod_ex
Scanning dependencies of target krr_regression_ex
[ 40%] Building CXX object CMakeFiles/krr_regression_ex.dir/krr_regression_ex.cpp.o
[ 40%] Linking CXX executable krr_regression_ex
[ 40%] Built target krr_regression_ex
Scanning dependencies of target bayes_net_gui_ex
[ 40%] Building CXX object CMakeFiles/bayes_net_gui_ex.dir/bayes_net_gui_ex.cpp.o
[ 41%] Linking CXX executable bayes_net_gui_ex
[ 41%] Built target bayes_net_gui_ex
Scanning dependencies of target dnn_introduction2_ex
[ 41%] Building CXX object CMakeFiles/dnn_introduction2_ex.dir/dnn_introduction2_ex.cpp.o
[ 42%] Linking CXX executable dnn_introduction2_ex
[ 42%] Built target dnn_introduction2_ex
Scanning dependencies of target face_landmark_detection_ex
[ 43%] Building CXX object CMakeFiles/face_landmark_detection_ex.dir/face_landmark_detection_ex.cpp.o
[ 43%] Linking CXX executable face_landmark_detection_ex
[ 43%] Built target face_landmark_detection_ex
Scanning dependencies of target bsp_ex
[ 44%] Building CXX object CMakeFiles/bsp_ex.dir/bsp_ex.cpp.o
[ 44%] Linking CXX executable bsp_ex
[ 44%] Built target bsp_ex
Scanning dependencies of target learning_to_track_ex
[ 45%] Building CXX object CMakeFiles/learning_to_track_ex.dir/learning_to_track_ex.cpp.o
[ 45%] Linking CXX executable learning_to_track_ex
[ 45%] Built target learning_to_track_ex
Scanning dependencies of target fhog_object_detector_ex
[ 45%] Building CXX object CMakeFiles/fhog_object_detector_ex.dir/fhog_object_detector_ex.cpp.o
[ 46%] Linking CXX executable fhog_object_detector_ex
[ 46%] Built target fhog_object_detector_ex
Scanning dependencies of target assignment_learning_ex
[ 47%] Building CXX object CMakeFiles/assignment_learning_ex.dir/assignment_learning_ex.cpp.o
[ 47%] Linking CXX executable assignment_learning_ex
[ 47%] Built target assignment_learning_ex
Scanning dependencies of target kkmeans_ex
[ 48%] Building CXX object CMakeFiles/kkmeans_ex.dir/kkmeans_ex.cpp.o
[ 48%] Linking CXX executable kkmeans_ex
[ 48%] Built target kkmeans_ex
Scanning dependencies of target svm_pegasos_ex
[ 48%] Building CXX object CMakeFiles/svm_pegasos_ex.dir/svm_pegasos_ex.cpp.o
[ 48%] Linking CXX executable svm_pegasos_ex
[ 48%] Built target svm_pegasos_ex
Scanning dependencies of target svm_ex
[ 48%] Building CXX object CMakeFiles/svm_ex.dir/svm_ex.cpp.o
[ 49%] Linking CXX executable svm_ex
[ 49%] Built target svm_ex
Scanning dependencies of target custom_trainer_ex
[ 49%] Building CXX object CMakeFiles/custom_trainer_ex.dir/custom_trainer_ex.cpp.o
[ 50%] Linking CXX executable custom_trainer_ex
[ 50%] Built target custom_trainer_ex
Scanning dependencies of target logger_ex_2
[ 51%] Building CXX object CMakeFiles/logger_ex_2.dir/logger_ex_2.cpp.o
[ 51%] Linking CXX executable logger_ex_2
[ 51%] Built target logger_ex_2
Scanning dependencies of target std_allocator_ex
[ 52%] Building CXX object CMakeFiles/std_allocator_ex.dir/std_allocator_ex.cpp.o
[ 52%] Linking CXX executable std_allocator_ex
[ 52%] Built target std_allocator_ex
Scanning dependencies of target random_cropper_ex
[ 52%] Building CXX object CMakeFiles/random_cropper_ex.dir/random_cropper_ex.cpp.o
[ 52%] Linking CXX executable random_cropper_ex
[ 52%] Built target random_cropper_ex
Scanning dependencies of target matrix_expressions_ex
[ 52%] Building CXX object CMakeFiles/matrix_expressions_ex.dir/matrix_expressions_ex.cpp.o
[ 53%] Linking CXX executable matrix_expressions_ex
[ 53%] Built target matrix_expressions_ex
Scanning dependencies of target krls_filter_ex
[ 53%] Building CXX object CMakeFiles/krls_filter_ex.dir/krls_filter_ex.cpp.o
[ 54%] Linking CXX executable krls_filter_ex
[ 54%] Built target krls_filter_ex
Scanning dependencies of target bridge_ex
[ 54%] Building CXX object CMakeFiles/bridge_ex.dir/bridge_ex.cpp.o
[ 54%] Linking CXX executable bridge_ex
[ 54%] Built target bridge_ex
Scanning dependencies of target svm_c_ex
[ 54%] Building CXX object CMakeFiles/svm_c_ex.dir/svm_c_ex.cpp.o
[ 55%] Linking CXX executable svm_c_ex
[ 55%] Built target svm_c_ex
Scanning dependencies of target svm_rank_ex
[ 56%] Building CXX object CMakeFiles/svm_rank_ex.dir/svm_rank_ex.cpp.o
[ 56%] Linking CXX executable svm_rank_ex
[ 56%] Built target svm_rank_ex
Scanning dependencies of target dnn_metric_learning_on_images_ex
[ 57%] Building CXX object CMakeFiles/dnn_metric_learning_on_images_ex.dir/dnn_metric_learning_on_images_ex.cpp.o
[ 57%] Linking CXX executable dnn_metric_learning_on_images_ex
[ 57%] Built target dnn_metric_learning_on_images_ex
Scanning dependencies of target 3d_point_cloud_ex
[ 57%] Building CXX object CMakeFiles/3d_point_cloud_ex.dir/3d_point_cloud_ex.cpp.o
[ 57%] Linking CXX executable 3d_point_cloud_ex
[ 57%] Built target 3d_point_cloud_ex
Scanning dependencies of target logger_ex
[ 58%] Building CXX object CMakeFiles/logger_ex.dir/logger_ex.cpp.o
[ 58%] Linking CXX executable logger_ex
[ 58%] Built target logger_ex
Scanning dependencies of target webcam_face_pose_ex
[ 58%] Building CXX object CMakeFiles/webcam_face_pose_ex.dir/webcam_face_pose_ex.cpp.o
[ 59%] Linking CXX executable webcam_face_pose_ex
[ 59%] Built target webcam_face_pose_ex
Scanning dependencies of target svm_sparse_ex
[ 60%] Building CXX object CMakeFiles/svm_sparse_ex.dir/svm_sparse_ex.cpp.o
[ 60%] Linking CXX executable svm_sparse_ex
[ 60%] Built target svm_sparse_ex
Scanning dependencies of target kcentroid_ex
[ 61%] Building CXX object CMakeFiles/kcentroid_ex.dir/kcentroid_ex.cpp.o
[ 61%] Linking CXX executable kcentroid_ex
[ 61%] Built target kcentroid_ex
Scanning dependencies of target dnn_inception_ex
[ 62%] Building CXX object CMakeFiles/dnn_inception_ex.dir/dnn_inception_ex.cpp.o
[ 62%] Linking CXX executable dnn_inception_ex
[ 62%] Built target dnn_inception_ex
Scanning dependencies of target dnn_mmod_face_detection_ex
[ 62%] Building CXX object CMakeFiles/dnn_mmod_face_detection_ex.dir/dnn_mmod_face_detection_ex.cpp.o
[ 63%] Linking CXX executable dnn_mmod_face_detection_ex
[ 63%] Built target dnn_mmod_face_detection_ex
Scanning dependencies of target bayes_net_ex
[ 64%] Building CXX object CMakeFiles/bayes_net_ex.dir/bayes_net_ex.cpp.o
[ 64%] Linking CXX executable bayes_net_ex
[ 64%] Built target bayes_net_ex
Scanning dependencies of target bayes_net_from_disk_ex
[ 64%] Building CXX object CMakeFiles/bayes_net_from_disk_ex.dir/bayes_net_from_disk_ex.cpp.o
[ 65%] Linking CXX executable bayes_net_from_disk_ex
[ 65%] Built target bayes_net_from_disk_ex
Scanning dependencies of target config_reader_ex
[ 65%] Building CXX object CMakeFiles/config_reader_ex.dir/config_reader_ex.cpp.o
[ 66%] Linking CXX executable config_reader_ex
[ 66%] Built target config_reader_ex
Scanning dependencies of target compress_stream_ex
[ 67%] Building CXX object CMakeFiles/compress_stream_ex.dir/compress_stream_ex.cpp.o
[ 67%] Linking CXX executable compress_stream_ex
[ 67%] Built target compress_stream_ex
Scanning dependencies of target using_custom_kernels_ex
[ 68%] Building CXX object CMakeFiles/using_custom_kernels_ex.dir/using_custom_kernels_ex.cpp.o
[ 68%] Linking CXX executable using_custom_kernels_ex
[ 68%] Built target using_custom_kernels_ex
Scanning dependencies of target max_cost_assignment_ex
[ 68%] Building CXX object CMakeFiles/max_cost_assignment_ex.dir/max_cost_assignment_ex.cpp.o
[ 68%] Linking CXX executable max_cost_assignment_ex
[ 68%] Built target max_cost_assignment_ex
Scanning dependencies of target member_function_pointer_ex
[ 69%] Building CXX object CMakeFiles/member_function_pointer_ex.dir/member_function_pointer_ex.cpp.o
[ 69%] Linking CXX executable member_function_pointer_ex
[ 69%] Built target member_function_pointer_ex
Scanning dependencies of target train_shape_predictor_ex
[ 70%] Building CXX object CMakeFiles/train_shape_predictor_ex.dir/train_shape_predictor_ex.cpp.o
[ 70%] Linking CXX executable train_shape_predictor_ex
[ 70%] Built target train_shape_predictor_ex
Scanning dependencies of target mlp_ex
[ 71%] Building CXX object CMakeFiles/mlp_ex.dir/mlp_ex.cpp.o
[ 71%] Linking CXX executable mlp_ex
[ 71%] Built target mlp_ex
Scanning dependencies of target thread_pool_ex
[ 72%] Building CXX object CMakeFiles/thread_pool_ex.dir/thread_pool_ex.cpp.o
[ 72%] Linking CXX executable thread_pool_ex
[ 72%] Built target thread_pool_ex
Scanning dependencies of target parallel_for_ex
[ 72%] Building CXX object CMakeFiles/parallel_for_ex.dir/parallel_for_ex.cpp.o
[ 72%] Linking CXX executable parallel_for_ex
[ 72%] Built target parallel_for_ex
Scanning dependencies of target svm_struct_ex
[ 72%] Building CXX object CMakeFiles/svm_struct_ex.dir/svm_struct_ex.cpp.o
[ 73%] Linking CXX executable svm_struct_ex
[ 73%] Built target svm_struct_ex
Scanning dependencies of target multiclass_classification_ex
[ 73%] Building CXX object CMakeFiles/multiclass_classification_ex.dir/multiclass_classification_ex.cpp.o
[ 73%] Linking CXX executable multiclass_classification_ex
[ 73%] Built target multiclass_classification_ex
Scanning dependencies of target object_detector_advanced_ex
[ 74%] Building CXX object CMakeFiles/object_detector_advanced_ex.dir/object_detector_advanced_ex.cpp.o
[ 74%] Linking CXX executable object_detector_advanced_ex
[ 74%] Built target object_detector_advanced_ex
Scanning dependencies of target running_stats_ex
[ 75%] Building CXX object CMakeFiles/running_stats_ex.dir/running_stats_ex.cpp.o
[ 75%] Linking CXX executable running_stats_ex
[ 75%] Built target running_stats_ex
Scanning dependencies of target object_detector_ex
[ 76%] Building CXX object CMakeFiles/object_detector_ex.dir/object_detector_ex.cpp.o
[ 76%] Linking CXX executable object_detector_ex
[ 76%] Built target object_detector_ex
Scanning dependencies of target one_class_classifiers_ex
[ 76%] Building CXX object CMakeFiles/one_class_classifiers_ex.dir/one_class_classifiers_ex.cpp.o
[ 77%] Linking CXX executable one_class_classifiers_ex
[ 77%] Built target one_class_classifiers_ex
Scanning dependencies of target optimization_ex
[ 77%] Building CXX object CMakeFiles/optimization_ex.dir/optimization_ex.cpp.o
[ 78%] Linking CXX executable optimization_ex
[ 78%] Built target optimization_ex
Scanning dependencies of target graph_labeling_ex
[ 79%] Building CXX object CMakeFiles/graph_labeling_ex.dir/graph_labeling_ex.cpp.o
[ 79%] Linking CXX executable graph_labeling_ex
[ 79%] Built target graph_labeling_ex
Scanning dependencies of target pipe_ex
[ 80%] Building CXX object CMakeFiles/pipe_ex.dir/pipe_ex.cpp.o
[ 80%] Linking CXX executable pipe_ex
[ 80%] Built target pipe_ex
Scanning dependencies of target pipe_ex_2
[ 81%] Building CXX object CMakeFiles/pipe_ex_2.dir/pipe_ex_2.cpp.o
[ 81%] Linking CXX executable pipe_ex_2
[ 81%] Built target pipe_ex_2
Scanning dependencies of target dnn_face_recognition_ex
[ 81%] Building CXX object CMakeFiles/dnn_face_recognition_ex.dir/dnn_face_recognition_ex.cpp.o
[ 81%] Linking CXX executable dnn_face_recognition_ex
[ 81%] Built target dnn_face_recognition_ex
Scanning dependencies of target quantum_computing_ex
[ 81%] Building CXX object CMakeFiles/quantum_computing_ex.dir/quantum_computing_ex.cpp.o
[ 82%] Linking CXX executable quantum_computing_ex
[ 82%] Built target quantum_computing_ex
Scanning dependencies of target rvm_regression_ex
[ 82%] Building CXX object CMakeFiles/rvm_regression_ex.dir/rvm_regression_ex.cpp.o
[ 83%] Linking CXX executable rvm_regression_ex
[ 83%] Built target rvm_regression_ex
Scanning dependencies of target matrix_ex
[ 83%] Building CXX object CMakeFiles/matrix_ex.dir/matrix_ex.cpp.o
[ 84%] Linking CXX executable matrix_ex
[ 84%] Built target matrix_ex
Scanning dependencies of target sequence_labeler_ex
[ 84%] Building CXX object CMakeFiles/sequence_labeler_ex.dir/sequence_labeler_ex.cpp.o
[ 84%] Linking CXX executable sequence_labeler_ex
[ 84%] Built target sequence_labeler_ex
Scanning dependencies of target sequence_segmenter_ex
[ 85%] Building CXX object CMakeFiles/sequence_segmenter_ex.dir/sequence_segmenter_ex.cpp.o
[ 85%] Linking CXX executable sequence_segmenter_ex
[ 85%] Built target sequence_segmenter_ex
Scanning dependencies of target server_http_ex
[ 86%] Building CXX object CMakeFiles/server_http_ex.dir/server_http_ex.cpp.o
[ 86%] Linking CXX executable server_http_ex
[ 86%] Built target server_http_ex
Scanning dependencies of target sockets_ex
[ 86%] Building CXX object CMakeFiles/sockets_ex.dir/sockets_ex.cpp.o
[ 87%] Linking CXX executable sockets_ex
[ 87%] Built target sockets_ex
Scanning dependencies of target least_squares_ex
[ 87%] Building CXX object CMakeFiles/least_squares_ex.dir/least_squares_ex.cpp.o
[ 88%] Linking CXX executable least_squares_ex
[ 88%] Built target least_squares_ex
Scanning dependencies of target dnn_imagenet_train_ex
[ 89%] Building CXX object CMakeFiles/dnn_imagenet_train_ex.dir/dnn_imagenet_train_ex.cpp.o
[ 89%] Linking CXX executable dnn_imagenet_train_ex
[ 89%] Built target dnn_imagenet_train_ex
Scanning dependencies of target sockstreambuf_ex
[ 89%] Building CXX object CMakeFiles/sockstreambuf_ex.dir/sockstreambuf_ex.cpp.o
[ 89%] Linking CXX executable sockstreambuf_ex
[ 89%] Built target sockstreambuf_ex
Scanning dependencies of target surf_ex
[ 90%] Building CXX object CMakeFiles/surf_ex.dir/surf_ex.cpp.o
[ 90%] Linking CXX executable surf_ex
[ 90%] Built target surf_ex
Scanning dependencies of target dnn_imagenet_ex
[ 91%] Building CXX object CMakeFiles/dnn_imagenet_ex.dir/dnn_imagenet_ex.cpp.o
[ 91%] Linking CXX executable dnn_imagenet_ex
[ 91%] Built target dnn_imagenet_ex
Scanning dependencies of target dnn_mmod_dog_hipsterizer
[ 92%] Building CXX object CMakeFiles/dnn_mmod_dog_hipsterizer.dir/dnn_mmod_dog_hipsterizer.cpp.o
[ 92%] Linking CXX executable dnn_mmod_dog_hipsterizer
[ 92%] Built target dnn_mmod_dog_hipsterizer
Scanning dependencies of target server_iostream_ex
[ 92%] Building CXX object CMakeFiles/server_iostream_ex.dir/server_iostream_ex.cpp.o
[ 93%] Linking CXX executable server_iostream_ex
[ 93%] Built target server_iostream_ex
Scanning dependencies of target thread_function_ex
[ 93%] Building CXX object CMakeFiles/thread_function_ex.dir/thread_function_ex.cpp.o
[ 93%] Linking CXX executable thread_function_ex
[ 93%] Built target thread_function_ex
Scanning dependencies of target threaded_object_ex
[ 94%] Building CXX object CMakeFiles/threaded_object_ex.dir/threaded_object_ex.cpp.o
[ 94%] Linking CXX executable threaded_object_ex
[ 94%] Built target threaded_object_ex
Scanning dependencies of target threads_ex
[ 94%] Building CXX object CMakeFiles/threads_ex.dir/threads_ex.cpp.o
[ 95%] Linking CXX executable threads_ex
[ 95%] Built target threads_ex
Scanning dependencies of target svr_ex
[ 95%] Building CXX object CMakeFiles/svr_ex.dir/svr_ex.cpp.o
[ 96%] Linking CXX executable svr_ex
[ 96%] Built target svr_ex
Scanning dependencies of target timer_ex
[ 96%] Building CXX object CMakeFiles/timer_ex.dir/timer_ex.cpp.o
[ 97%] Linking CXX executable timer_ex
[ 97%] Built target timer_ex
Scanning dependencies of target train_object_detector
[ 97%] Building CXX object CMakeFiles/train_object_detector.dir/train_object_detector.cpp.o
[ 97%] Linking CXX executable train_object_detector
[ 97%] Built target train_object_detector
Scanning dependencies of target xml_parser_ex
[ 97%] Building CXX object CMakeFiles/xml_parser_ex.dir/xml_parser_ex.cpp.o
[ 98%] Linking CXX executable xml_parser_ex
[ 98%] Built target xml_parser_ex

Scanning dependencies of target model_selection_ex
[ 98%] Building CXX object CMakeFiles/model_selection_ex.dir/model_selection_ex.cpp.o
[ 99%] Linking CXX executable model_selection_ex
[ 99%] Built target model_selection_ex
Scanning dependencies of target dnn_metric_learning_ex
[ 99%] Building CXX object CMakeFiles/dnn_metric_learning_ex.dir/dnn_metric_learning_ex.cpp.o
[ 99%] Linking CXX executable dnn_metric_learning_ex
[ 99%] Built target dnn_metric_learning_ex
Scanning dependencies of target sqlite_ex
[100%] Building CXX object CMakeFiles/sqlite_ex.dir/sqlite_ex.cpp.o
[100%] Linking CXX executable sqlite_ex
[100%] Built target sqlite_ex


```
