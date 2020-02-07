주요 참조 링크
- https://github.com/ros/ros_comm/issues/1357
- https://github.com/mikepurvis/ros-install-osx


소스 컴파일 설치 

- 주요 환경 : python 2.7, opencv 4.1.2

- 컴파일 옵션 (jongchulseon 은 제 노트북에 한정된 경로입니다. 각자의 환경에 맞게 수정하시면 됩니다. )

./src/catkin/bin/catkin_make_isolated --install -DCMAKE_BUILD_TYPE=Release -DCMAKE_PREFIX_PATH="/usr/local/opt/qt;/Users/jongchulseon/Development/lunar_barebone/install_isolated" -DCMAKE_FIND_FRAMEWORK=LAST -DPYTHON_INCLUDE_DIR="/usr/local/Cellar/python@2/2.7.16/Frameworks/Python.framework/Headers" -DPYTHON_LIBRARY="/usr/local/Cellar/python@2/2.7.16/Frameworks/Python.framework/Versions/2.7/lib/libpython2.7.dylib" -DCMAKE_MACOSX_RPATH=ON -DCMAKE_INSTALL_RPATH="/Users/jongchulseon/Development/lunar_barebone/install_isolated/lib" -DCMAKE_CXX_FLAGS="-std=c++11"

./src/catkin/bin/catkin_make_isolated --install -DCMAKE_BUILD_TYPE=Release -DCMAKE_PREFIX_PATH="/usr/local/opt/qt;/Users/jongchulseon/Development/lunar_barebone/install_isolated" -DCMAKE_FIND_FRAMEWORK=LAST -DPYTHON_INCLUDE_DIR="/usr/local/Cellar/python@2/2.7.16/Frameworks/Python.framework/Headers" -DPYTHON_LIBRARY="/usr/local/Cellar/python@2/2.7.16/Frameworks/Python.framework/Versions/2.7/lib/libpython2.7.dylib" -DCMAKE_MACOSX_RPATH=ON -DCMAKE_INSTALL_RPATH="/Users/jongchulseon/Development/lunar_barebone/install_isolated/lib" -DCMAKE_CXX_FLAGS="-std=c++14"



