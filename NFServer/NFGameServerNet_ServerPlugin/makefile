#------------------------------------------------------------------------------#
# This makefile was generated by 'cbp2make' tool rev.147                       #
#------------------------------------------------------------------------------#


WORKDIR = `pwd`

CC = gcc
CXX = g++
AR = ar
LD = g++
WINDRES = windres

INC = 
CFLAGS = 
RESINC = 
LIBDIR = 
LIB = 
LDFLAGS = 
SolutionDir = ../../


INC_DEBUG_X64 = $(INC) -I$(SolutionDir) -I$(SolutionDir)/Dependencies/ -I$(SolutionDir)/Dependencies/libevent/ -I$(SolutionDir)/Dependencies/libevent/include/ -I$(SolutionDir)/Dependencies/libevent/compat/ -I$(SolutionDir)/Dependencies/protobuf/src/ -I$(SolutionDir)/Dependencies/Theron/Include/
CFLAGS_DEBUG_X64 = $(CFLAGS) -std=c++11 -g -fPIC -D_DEBUG -D_USRDLL -DELPP_NO_DEFAULT_LOG_FILE
RESINC_DEBUG_X64 = $(RESINC)
RCFLAGS_DEBUG_X64 = $(RCFLAGS)
LIBDIR_DEBUG_X64 = $(LIBDIR) -L$(SolutionDir)/_Out/Comm/Debug/ -L$(SolutionDir)/Dependencies/lib/Debug/
LIB_DEBUG_X64 = $(LIB)$(SolutionDir)/_Out/Comm/Debug/NFMessageDefine_d.a $(SolutionDir)/_Out/Comm/Debug/NFNet_d.a $(SolutionDir)/Dependencies/lib/Debug/libevent.a $(SolutionDir)/Dependencies/lib/Debug/libevent_core.a $(SolutionDir)/Dependencies/lib/Debug/libprotobuf.a
LDFLAGS_DEBUG_X64 = $(LDFLAGS)
OBJDIR_DEBUG_X64 = .objs/Debug
DEP_DEBUG_X64 = 
OUT_DEBUG_X64 = $(SolutionDir)/_Out/Comm/Debug/NFGameServerNet_ServerPlugin_d.so

INC_RELEASE_X64 = $(INC) -I$(SolutionDir) -I$(SolutionDir)/Dependencies/ -I$(SolutionDir)/Dependencies/libevent/ -I$(SolutionDir)/Dependencies/libevent/include/ -I$(SolutionDir)/Dependencies/libevent/compat/ -I$(SolutionDir)/Dependencies/protobuf/src/ -I$(SolutionDir)/Dependencies/Theron/Include/
CFLAGS_RELEASE_X64 = $(CFLAGS) -std=c++11 -fPIC -D_USRDLL -DELPP_NO_DEFAULT_LOG_FILE
RESINC_RELEASE_X64 = $(RESINC)
RCFLAGS_RELEASE_X64 = $(RCFLAGS)
LIBDIR_RELEASE_X64 = $(LIBDIR) -L$(SolutionDir)/_Out/Comm/Release/ -L$(SolutionDir)/Dependencies/lib/Release/
LIB_RELEASE_X64 = $(LIB)$(SolutionDir)/_Out/Comm/Release/NFMessageDefine.a $(SolutionDir)/_Out/Comm/Release/NFNet.a $(SolutionDir)/Dependencies/lib/Release/libevent.a $(SolutionDir)/Dependencies/lib/Release/libevent_core.a $(SolutionDir)/Dependencies/lib/Release/libprotobuf.a
LDFLAGS_RELEASE_X64 = $(LDFLAGS)
OBJDIR_RELEASE_X64 = .objs/Release
DEP_RELEASE_X64 = 
OUT_RELEASE_X64 = $(SolutionDir)/_Out/Comm/Release/NFGameServerNet_ServerPlugin.so

OBJ_DEBUG_X64 = $(OBJDIR_DEBUG_X64)/NFCGameServerNet_ServerModule.o $(OBJDIR_DEBUG_X64)/NFGameServerNet_ServerPlugin.o $(OBJDIR_DEBUG_X64)/dllmain.o

OBJ_RELEASE_X64 = $(OBJDIR_RELEASE_X64)/NFCGameServerNet_ServerModule.o $(OBJDIR_RELEASE_X64)/NFGameServerNet_ServerPlugin.o $(OBJDIR_RELEASE_X64)/dllmain.o

all: debug_x64 release_x64

clean: clean_debug_x64 clean_release_x64

before_debug_x64: 
	test -d $(SolutionDir)/_Out/Comm/Debug || mkdir -p $(SolutionDir)/_Out/Comm/Debug
	test -d $(OBJDIR_DEBUG_X64) || mkdir -p $(OBJDIR_DEBUG_X64)

after_debug_x64: 
	cp -f $(SolutionDir)/_Out/Comm/Debug/NFGameServerNet_ServerPlugin_d.so $(SolutionDir)/_Out/Server/Debug/NFGameServer1/

debug_x64: before_debug_x64 out_debug_x64 after_debug_x64

out_debug_x64: before_debug_x64 $(OBJ_DEBUG_X64) $(DEP_DEBUG_X64)
	$(LD) -shared $(LIBDIR_DEBUG_X64) $(OBJ_DEBUG_X64)  -o $(OUT_DEBUG_X64) $(LDFLAGS_DEBUG_X64) $(LIB_DEBUG_X64)

$(OBJDIR_DEBUG_X64)/NFCGameServerNet_ServerModule.o: NFCGameServerNet_ServerModule.cpp
	$(CXX) $(CFLAGS_DEBUG_X64) $(INC_DEBUG_X64) -c NFCGameServerNet_ServerModule.cpp -o $(OBJDIR_DEBUG_X64)/NFCGameServerNet_ServerModule.o

$(OBJDIR_DEBUG_X64)/NFGameServerNet_ServerPlugin.o: NFGameServerNet_ServerPlugin.cpp
	$(CXX) $(CFLAGS_DEBUG_X64) $(INC_DEBUG_X64) -c NFGameServerNet_ServerPlugin.cpp -o $(OBJDIR_DEBUG_X64)/NFGameServerNet_ServerPlugin.o

$(OBJDIR_DEBUG_X64)/dllmain.o: dllmain.cpp
	$(CXX) $(CFLAGS_DEBUG_X64) $(INC_DEBUG_X64) -c dllmain.cpp -o $(OBJDIR_DEBUG_X64)/dllmain.o

clean_debug_x64: 
	rm -f $(OBJ_DEBUG_X64) $(OUT_DEBUG_X64)
	rm -rf $(SolutionDir)/_Out/Comm/Debug
	rm -rf $(OBJDIR_DEBUG_X64)

before_release_x64: 
	test -d $(SolutionDir)/_Out/Comm/Release || mkdir -p $(SolutionDir)/_Out/Comm/Release
	test -d $(OBJDIR_RELEASE_X64) || mkdir -p $(OBJDIR_RELEASE_X64)

after_release_x64: 
	cp -f $(SolutionDir)/_Out/Comm/Release/NFGameServerNet_ServerPlugin.so $(SolutionDir)/_Out/Server/Release/NFGameServer1/

release_x64: before_release_x64 out_release_x64 after_release_x64

out_release_x64: before_release_x64 $(OBJ_RELEASE_X64) $(DEP_RELEASE_X64)
	$(LD) -shared $(LIBDIR_RELEASE_X64) $(OBJ_RELEASE_X64)  -o $(OUT_RELEASE_X64) $(LDFLAGS_RELEASE_X64) $(LIB_RELEASE_X64)

$(OBJDIR_RELEASE_X64)/NFCGameServerNet_ServerModule.o: NFCGameServerNet_ServerModule.cpp
	$(CXX) $(CFLAGS_RELEASE_X64) $(INC_RELEASE_X64) -c NFCGameServerNet_ServerModule.cpp -o $(OBJDIR_RELEASE_X64)/NFCGameServerNet_ServerModule.o

$(OBJDIR_RELEASE_X64)/NFGameServerNet_ServerPlugin.o: NFGameServerNet_ServerPlugin.cpp
	$(CXX) $(CFLAGS_RELEASE_X64) $(INC_RELEASE_X64) -c NFGameServerNet_ServerPlugin.cpp -o $(OBJDIR_RELEASE_X64)/NFGameServerNet_ServerPlugin.o

$(OBJDIR_RELEASE_X64)/dllmain.o: dllmain.cpp
	$(CXX) $(CFLAGS_RELEASE_X64) $(INC_RELEASE_X64) -c dllmain.cpp -o $(OBJDIR_RELEASE_X64)/dllmain.o

clean_release_x64: 
	rm -f $(OBJ_RELEASE_X64) $(OUT_RELEASE_X64)
	rm -rf $(SolutionDir)/_Out/Comm/Release
	rm -rf $(OBJDIR_RELEASE_X64)

.PHONY: before_debug_x64 after_debug_x64 clean_debug_x64 before_release_x64 after_release_x64 clean_release_x64

